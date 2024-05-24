# Comparing `tmp/oasees_sdk-0.2.9.tar.gz` & `tmp/oasees_sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oasees_sdk-0.2.9.tar", max compression
+gzip compressed data, was "oasees_sdk-0.3.0.tar", max compression
```

## Comparing `oasees_sdk-0.2.9.tar` & `oasees_sdk-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       10 2024-04-22 11:03:39.624851 oasees_sdk-0.2.9/README.md
--rw-r--r--   0        0        0      619 2024-05-15 17:13:12.624962 oasees_sdk-0.2.9/pyproject.toml
--rw-r--r--   0        0        0    21810 2024-05-15 17:12:36.925152 oasees_sdk-0.2.9/src/oasees_sdk/cli/cli.py
--rw-r--r--   0        0        0       18 2024-05-10 14:31:20.743803 oasees_sdk-0.2.9/src/oasees_sdk/oasees_sdk/__init__.py
--rw-r--r--   0        0        0      887 2024-05-10 14:31:20.755803 oasees_sdk-0.2.9/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py
--rw-r--r--   0        0        0     1934 2024-05-10 14:31:20.699804 oasees_sdk-0.2.9/src/oasees_sdk/oasees_sdk/deploy_pipeline.py
--rw-r--r--   0        0        0    10073 2024-05-15 15:54:37.450395 oasees_sdk-0.2.9/src/oasees_sdk/oasees_sdk/sdk.py
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 oasees_sdk-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0       10 2024-04-22 11:03:39.624851 oasees_sdk-0.3.0/README.md
+-rw-r--r--   0        0        0      619 2024-05-24 12:48:06.033290 oasees_sdk-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    33010 2024-05-24 12:42:12.847073 oasees_sdk-0.3.0/src/oasees_sdk/cli/cli.py
+-rw-r--r--   0        0        0       18 2024-05-10 14:31:20.743803 oasees_sdk-0.3.0/src/oasees_sdk/oasees_sdk/__init__.py
+-rw-r--r--   0        0        0      887 2024-05-10 14:31:20.755803 oasees_sdk-0.3.0/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py
+-rw-r--r--   0        0        0     1934 2024-05-10 14:31:20.699804 oasees_sdk-0.3.0/src/oasees_sdk/oasees_sdk/deploy_pipeline.py
+-rw-r--r--   0        0        0    10095 2024-05-24 12:42:10.295086 oasees_sdk-0.3.0/src/oasees_sdk/oasees_sdk/sdk.py
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 oasees_sdk-0.3.0/PKG-INFO
```

### Comparing `oasees_sdk-0.2.9/pyproject.toml` & `oasees_sdk-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "oasees_sdk"
-version = "0.2.9"
+version = "0.3.0"
 description = "Oasees SDK"
 authors = [
     "Example Author <author@example.com>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `oasees_sdk-0.2.9/src/oasees_sdk/cli/cli.py` & `oasees_sdk-0.3.0/src/oasees_sdk/cli/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import subprocess
+import time
 import click
 import getpass
 import json
 import ipfshttpclient
 import requests
 import web3
 import socket
 import os
 from dotenv import load_dotenv
 import yaml
+from kubernetes import client,config
 
 ipfs_manifest_str = """apiVersion: apps/v1
 kind: Deployment
 metadata:
   name: ipfs-kubo-deployment
 spec:
   replicas: 1
@@ -61,14 +63,15 @@
     - name: api
       port: 5002
       targetPort: 5001
       protocol: TCP
       nodePort: 31005
 """
 
+SDK_PATH = "/home/" + getpass.getuser() + "/.oasees_sdk"
 
 @click.group(invoke_without_command=True)
 @click.pass_context
 def cli(ctx):
     if not ctx.invoked_subcommand:
         bash_script = r'''
         Y='\x1b[38;2;252;220;132m'
@@ -118,15 +121,15 @@
         cli(['--help'])
 
 @cli.command()
 def init_cluster():
     '''Creates a new kubernetes cluster with the current machine as its master, and registers it to the blockchain.'''
     config_setup()
     try:
-        with open('/home/'+getpass.getuser()+'/config.json', 'r') as f:
+        with open('/home/'+getpass.getuser()+'/.oasees_sdk/config.json', 'r') as f:
             config = json.load(f)
 
         w3 = web3.Web3(web3.HTTPProvider("http://{}:8545".format(config['BLOCKCHAIN_IP'])))
         from web3.middleware import geth_poa_middleware
         w3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
         response = requests.get('http://{}:6001/ipfs_portal_contracts'.format(config['PROVIDER_IP']))
@@ -150,21 +153,23 @@
         echo = subprocess.run(['sudo','sh', '-c','echo "mirrors:\n  docker.io:\n  registry.k8s.io:" > /etc/rancher/k3s/registries.yaml'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         curl = subprocess.Popen(['curl','-sfL', 'https://get.k3s.io'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         result = subprocess.check_output(['sh','-s','-','--write-kubeconfig-mode','644', '--write-kubeconfig', '/home/'+getpass.getuser()+'/.kube/config','--embedded-registry'], stdin=curl.stdout)
         click.echo(result)
         curl.wait()
 
 
+        time.sleep(3)
 
         with open('/home/'+getpass.getuser()+'/.kube/config', 'r') as f:
             cluster_config = yaml.safe_load(f)
 
         result = subprocess.run(['kubectl','get','nodes','-o','custom-columns=IP:.status.addresses[].address','--no-headers'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         ip = result.stdout.strip().split('\n')
 
+        click.echo(ip[0])
         cluster_config['clusters'][0]['cluster']['server'] = "https://{}:6443".format(ip[0])
 
         echo = subprocess.Popen(['echo', ipfs_manifest_str], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         result = subprocess.check_output(['kubectl','apply','-f','-'], stdin=echo.stdout)
         click.echo(result)
         echo.wait()
 
@@ -185,26 +190,45 @@
         signed_transaction = w3.eth.account.sign_transaction(transaction, private_key=deployer_key)
         transaction_hash = w3.eth.send_raw_transaction(signed_transaction.rawTransaction)
         txn_receipt = w3.eth.wait_for_transaction_receipt(transaction_hash)
         tx_json = json.loads(w3.to_json(txn_receipt))
 
         token_id=int(tx_json['logs'][2]['data'],16)
 
+
+
+
+        dao_args = {
+            "DAO_NAME": socket.gethostname(),
+            "DAO_DESC": "A Cluster created with Oasees SDK.",
+            "MIN_DELAY":0,
+            "VOTING_PERIOD":10,
+	        "VOTING_DELAY":0,
+            "QUORUM_PERCENTAGE":50,
+            "dao_app_name":"flask1"
+        }
+
+
+        ZERO_ADDRESS = '0x0000000000000000000000000000000000000000' 
+
+        DAO_NAME = dao_args['DAO_NAME']
+        DAO_DESC = dao_args['DAO_DESC']
+
         dao_info = {
-            "dao_name": socket.gethostname(),
-            "dao_desc": "A Cluster created with Oasees SDK.",
-            "dao_nft_address":nft_address,
-            "dao_nft_abi":nft_abi,
-	        "dao_nft_id":token_id
+            "dao_name": DAO_NAME,
+            "dao_desc": DAO_DESC,
+            "dao_app_name":"flask1"
         }
 
+
         dao_info_hash = client.add_json(dao_info)
         client.close()
+        
 
-        transaction = marketplace_contract.functions.makeDao(nft_address,100,dao_info_hash,token_id,True).build_transaction({
+        transaction = marketplace_contract.functions.makeDao(nft_address,0,dao_info_hash,token_id,True).build_transaction({
 		'value':0,
 		'chainId': 31337, 
 		'gas': 2000000,  
 		'gasPrice': w3.eth.gas_price,  
 		'nonce': w3.eth.get_transaction_count(deployer_account)
 	    })
 
@@ -215,14 +239,15 @@
 
         results = marketplace_contract.caller({'from': deployer_account}).getJoinedDaos()
         for dao in results:
             if (dao[6]):
                 update_cluster_id(dao[4])
                 break
 
+
         click.echo("Cluster successfully deployed.")
 
     except FileNotFoundError:
         click.echo("Error: K3s cluster could not be deployed.")
 
 
 
@@ -272,16 +297,17 @@
         curl.wait()
     except FileNotFoundError:
         click.echo("Error: K3S cluster could not be joined.\n")
             
 
 @cli.command()
 def get_config():
+    '''Prints out the SDK's current configuration file.'''
     try:
-        with open('/home/'+getpass.getuser()+'/config.json', "r") as f:
+        with open('/home/'+getpass.getuser()+'/.oasees_sdk/config.json', "r") as f:
             config = json.load(f)
             click.echo(config)
     except FileNotFoundError:
         click.echo("Error: Config file doesn't exist in the cli program's directory.")
 
 @cli.command()
 def get_nodes():
@@ -299,15 +325,15 @@
     try:
         result = subprocess.run(['kubectl','get','nodes','-l','!node-role.kubernetes.io/master','-o','custom-columns=NAME:.metadata.name','--no-headers'],  stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         node_names = result.stdout.strip().split('\n')
 
         result = subprocess.run(['kubectl','get','nodes','-l','!node-role.kubernetes.io/master','-o','custom-columns=IP:.status.addresses[].address','--no-headers'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         node_ips = result.stdout.strip().split('\n')
         
-        with open('/home/'+getpass.getuser()+'/config.json', 'r') as f:
+        with open('/home/'+getpass.getuser()+'/.oasees_sdk/config.json', 'r') as f:
             config = json.load(f)
 
         w3 = web3.Web3(web3.HTTPProvider("http://{}:8545".format(config['BLOCKCHAIN_IP'])))
         from web3.middleware import geth_poa_middleware
         w3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
 
@@ -324,25 +350,27 @@
         nft_contract = w3.eth.contract(address=nft_address, abi=nft_abi)
 
         deployer_account = w3.to_checksum_address(config['ACCOUNT'])
         deployer_key = config['KEY']
 
         new_nodes_names = []
         new_nodes_ips = []
-        with open('/home/'+getpass.getuser()+'/config.json','r') as f:
+        with open('/home/'+getpass.getuser()+'/.oasees_sdk/config.json','r') as f:
             config = json.load(f)
         
         agents = config['agents']
         for i in range(len(node_names)):
             if(node_names[i] not in agents.keys()):
                 new_nodes_names.append(node_names[i])
                 new_nodes_ips.append(node_ips[i])
 
         for i in range(len(new_nodes_names)):
             new_acc = w3.eth.account.create()
+            new_acc_address = new_acc.address
+            new_acc_pkey = w3.to_hex(new_acc.key)
             agents[new_nodes_names[i]] = [new_acc.address, w3.to_hex(new_acc.key)]
 
             device_name = new_nodes_names[i]
             device_content = {
                 "account": new_acc.address,
                 "name": device_name,
                 "device_endpoint": "http://"+new_nodes_ips[i]+":8001"
@@ -389,88 +417,356 @@
 
 
             signed_transaction = w3.eth.account.sign_transaction(transaction, private_key=config['KEY'])
             transaction_hash = w3.eth.send_raw_transaction(signed_transaction.rawTransaction)
             txn_receipt = w3.eth.wait_for_transaction_receipt(transaction_hash)
 
 
+            transaction = {
+                'to': new_acc_address,
+                'from': config['ACCOUNT'],
+                'value': w3.to_wei(1,'ether'),
+                'gas': 21000,  # Standard gas limit for a simple transfer
+                'gasPrice': w3.to_wei('1', 'gwei'),  # Gas price in Wei
+                'nonce': w3.eth.get_transaction_count(config['ACCOUNT']),
+                'chainId': 31337  # Default chain ID for Hardhat
+            }
+            private_key = config['KEY']  # Replace with the private key of the sender
+            signed_transaction = w3.eth.account.sign_transaction(transaction, private_key)
 
-            transaction = marketplace_contract.functions.registerDeviceToDao(new_acc.address,config['OASEES_CLUSTER_ID']).build_transaction({
-            'value':0,
-            'chainId': 31337, 
-            'gas': 2000000,  
-            'gasPrice': w3.eth.gas_price,  
-            'nonce': w3.eth.get_transaction_count(deployer_account)
-            })
-
-            signed_transaction = w3.eth.account.sign_transaction(transaction, private_key=deployer_key)
-            transaction_hash = w3.eth.send_raw_transaction(signed_transaction.rawTransaction)
-            txn_receipt = w3.eth.wait_for_transaction_receipt(transaction_hash)
+            # Send the transaction
+            tx_hash = w3.eth.send_raw_transaction(signed_transaction.rawTransaction)
+            # Wait for the transaction to be mined
+            tx_receipt = w3.eth.wait_for_transaction_receipt(tx_hash)
+            #print(f"Transaction receipt: {tx_receipt}")
+
+            deploy_agent(new_nodes_names[i],new_acc_address,new_acc_pkey)
+
+            if(config['DAO_TOKEN_ID']!=-1):
+                dao_content_hash = nft_contract.functions.tokenURI(config['DAO_TOKEN_ID']).call()
+                client = ipfshttpclient.connect("/ip4/{}/tcp/5001".format(config['IPFS_IP']))
+                dao_content = client.cat(dao_content_hash)
+                dao_content = dao_content.decode("UTF-8")
+                dao_content = json.loads(dao_content)
+
+                token_contract = w3.eth.contract(address=dao_content['token_address'], abi=dao_content['token_abi'])
+
+
+                transaction = token_contract.functions.transfer(new_acc_address,20).build_transaction({
+                    'from':config['ACCOUNT'],
+                    'value':0,
+                    'chainId': 31337, 
+                    'gas': 2000000,  
+                    'gasPrice': w3.eth.gas_price,  
+                    'nonce': w3.eth.get_transaction_count(deployer_account)
+                })
+
+                signed_transaction = w3.eth.account.sign_transaction(transaction, private_key=deployer_key)
+                transaction_hash = w3.eth.send_raw_transaction(signed_transaction.rawTransaction)
+                txn_receipt = w3.eth.wait_for_transaction_receipt(transaction_hash)
+
+                transaction = marketplace_contract.functions.registerDeviceToDao(new_acc.address,config['OASEES_CLUSTER_ID']).build_transaction({
+                    'value':0,
+                    'chainId': 31337, 
+                    'gas': 2000000,  
+                    'gasPrice': w3.eth.gas_price,  
+                    'nonce': w3.eth.get_transaction_count(deployer_account)
+                 })
+
+                signed_transaction = w3.eth.account.sign_transaction(transaction, private_key=deployer_key)
+                transaction_hash = w3.eth.send_raw_transaction(signed_transaction.rawTransaction)
+                txn_receipt = w3.eth.wait_for_transaction_receipt(transaction_hash)
+            else :
+                transaction = marketplace_contract.functions.registerDeviceToCluster(new_acc.address,config['OASEES_CLUSTER_ID']).build_transaction({
+                    'value':0,
+                    'chainId': 31337, 
+                    'gas': 2000000,  
+                    'gasPrice': w3.eth.gas_price,  
+                    'nonce': w3.eth.get_transaction_count(deployer_account)
+                 })
+
+                signed_transaction = w3.eth.account.sign_transaction(transaction, private_key=deployer_key)
+                transaction_hash = w3.eth.send_raw_transaction(signed_transaction.rawTransaction)
+                txn_receipt = w3.eth.wait_for_transaction_receipt(transaction_hash)
 
-            
 
         
         config['agents'] = agents
 
-        with open('/home/'+getpass.getuser()+'/config.json', 'w') as f:
+        with open('/home/'+getpass.getuser()+'/.oasees_sdk/config.json', 'w') as f:
             json.dump(config, f)
 
         if(len(new_nodes_names)>0):
             click.echo("Registered the latest node(s) on the blockchain.")
         else:
             click.echo("All nodes have already been registered.")
 
     except FileNotFoundError:
         click.echo("Error: Process could not be completed.")
 
 
+@cli.command()
+@click.argument('dao_content_hash', type=str)
+def apply_dao_logic(dao_content_hash):
+    with open('/home/'+getpass.getuser()+'/.oasees_sdk/config.json', 'r') as f:
+        config = json.load(f)
+
+    client = ipfshttpclient.connect("/ip4/{}/tcp/5001".format(config['IPFS_IP']))
+    dao_content = client.cat(dao_content_hash)
+    dao_content = dao_content.decode("UTF-8")
+    dao_content = json.loads(dao_content)
+
+
+    w3 = web3.Web3(web3.HTTPProvider("http://{}:8545".format(config['BLOCKCHAIN_IP'])))
+    from web3.middleware import geth_poa_middleware
+    w3.middleware_onion.inject(geth_poa_middleware, layer=0)
+
+    token_provider_contract = w3.eth.contract(address=dao_content['token_provider_address'], abi=dao_content['token_provider_abi'])
+    token_contract = w3.eth.contract(address=dao_content['token_address'], abi=dao_content['token_abi'])
+
+    deployer_account = web3.Web3.to_checksum_address(config['ACCOUNT'])
+    deployer_key = config['KEY']
+
+
+
+    response = requests.get('http://{}:6001/ipfs_portal_contracts'.format(config['PROVIDER_IP']))
+    response = response.json()
+    portal_contracts = response["portal_contracts"]
+
+    marketplace_address = portal_contracts["marketplace_address"]
+    marketplace_abi = portal_contracts["marketplace_abi"]
+    marketplace_contract = w3.eth.contract(address=marketplace_address, abi=marketplace_abi)
+
+    nft_address = portal_contracts["nft_address"]
+    nft_abi = portal_contracts["nft_abi"]
+
+    nft_contract = w3.eth.contract(address=nft_address, abi=nft_abi)
+
+
+    transaction = nft_contract.functions.mint(dao_content_hash).build_transaction({
+		'chainId': 31337,
+		'gas': 2000000,
+		'gasPrice': w3.eth.gas_price,
+		'nonce': w3.eth.get_transaction_count(deployer_account)
+	    })
+
+    signed_transaction = w3.eth.account.sign_transaction(transaction, private_key=deployer_key)
+    transaction_hash = w3.eth.send_raw_transaction(signed_transaction.rawTransaction)
+    txn_receipt = w3.eth.wait_for_transaction_receipt(transaction_hash)
+    tx_json = json.loads(w3.to_json(txn_receipt))
+
+    token_id=int(tx_json['logs'][2]['data'],16)
+
+    transaction = marketplace_contract.functions.applyDao(config['OASEES_CLUSTER_ID'],token_id).build_transaction({
+        'from':config['ACCOUNT'],
+        'value':0,
+        'chainId': 31337, 
+        'gas': 2000000,  
+        'gasPrice': w3.eth.gas_price,  
+        'nonce': w3.eth.get_transaction_count(config['ACCOUNT'])
+    })
+
+    signed_transaction = w3.eth.account.sign_transaction(transaction, private_key=config['KEY'])
+    transaction_hash = w3.eth.send_raw_transaction(signed_transaction.rawTransaction)
+    txn_receipt = w3.eth.wait_for_transaction_receipt(transaction_hash)
+    
+
+    
+
+
+    tx = token_provider_contract.functions.getTokens().build_transaction({
+        "gasPrice": w3.eth.gas_price,
+        "chainId": 31337,
+        "from": deployer_account,
+        "nonce": w3.eth.get_transaction_count(deployer_account)
+    })
+
+    signed_tx = w3.eth.account.sign_transaction(tx, private_key=deployer_key)
+    tx_hash = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
+    txn_receipt = w3.eth.wait_for_transaction_receipt(tx_hash)
+
+    tx = token_contract.functions.delegate(config['ACCOUNT']).build_transaction({
+        "gasPrice": w3.eth.gas_price,
+        "chainId": 31337,
+        "from": deployer_account,
+        "nonce": w3.eth.get_transaction_count(deployer_account)
+    })
+
+    signed_tx = w3.eth.account.sign_transaction(tx, private_key=deployer_key)
+    tx_hash = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
+    txn_receipt = w3.eth.wait_for_transaction_receipt(tx_hash)
+
+
+    for entry in config['agents']:
+        agent = config['agents'][entry]
+
+        transaction = token_contract.functions.transfer(agent[0],20).build_transaction({
+            'from':config['ACCOUNT'],
+            'value':0,
+            'chainId': 31337, 
+            'gas': 2000000,  
+            'gasPrice': w3.eth.gas_price,  
+            'nonce': w3.eth.get_transaction_count(deployer_account)
+        })
+
+        signed_transaction = w3.eth.account.sign_transaction(transaction, private_key=deployer_key)
+        transaction_hash = w3.eth.send_raw_transaction(signed_transaction.rawTransaction)
+        txn_receipt = w3.eth.wait_for_transaction_receipt(transaction_hash)
+
+    config['DAO_TOKEN_ID'] = token_id
+    with open('/home/'+getpass.getuser()+'/.oasees_sdk/config.json','w') as f:
+        json.dump(config,f)
+
+
+
+def deploy_agent(node_name,account,pkey):
+    config.load_kube_config()
+
+
+    # Create an API client for the AppsV1Api
+    api_instance = client.AppsV1Api()
+
+    with open('/home/'+getpass.getuser()+'/.oasees_sdk/config.json', 'r') as f:
+        sdk_config = json.load(f)
+
+    
+    # Define the container
+    env_vars = [
+        client.V1EnvVar(name="MARKETPLACE_ADDRESS", value="0x5FbDB2315678afecb367f032d93F642f64180aa3"),
+        client.V1EnvVar(name="NFT_ADDRESS", value="0xe7f1725E7734CE288F8367e1Bb143E90bb3F0512"),
+        client.V1EnvVar(name="IPFS_HOST", value=sdk_config['IPFS_IP']),
+        client.V1EnvVar(name="BLOCK_CHAIN_IP", value=sdk_config['BLOCKCHAIN_IP']),
+        client.V1EnvVar(name="ACCOUNT", value=account),
+        client.V1EnvVar(name="SECRET_KEY", value=pkey),
+        client.V1EnvVar(name="DEVICE_NAME", value=node_name)
+    ]
+
+    # Define the container
+    container = client.V1Container(
+        name="blockchain-agent",
+        image="andreasoikonomakis/oasees-blockchain-agent",
+        ports=[client.V1ContainerPort(container_port=5000)],
+        env=env_vars
+    )
+
+    # Define the pod template
+    template = client.V1PodTemplateSpec(
+        metadata=client.V1ObjectMeta(labels={"app": "blockchain-agent"}),
+        spec=client.V1PodSpec(
+            containers=[container],
+            node_name=node_name
+        )
+    )
+
+    # Define the deployment spec
+    spec = client.V1DeploymentSpec(
+        replicas=1,
+        selector=client.V1LabelSelector(
+            match_labels={"app": "blockchain-agent"}
+        ),
+        template=template
+    )
+
+    # Define the deployment
+    deployment = client.V1Deployment(
+        api_version="apps/v1",
+        kind="Deployment",
+        metadata=client.V1ObjectMeta(name="blockchain-agent-" + node_name),
+        spec=spec
+    )
+
+    # Create the deployment
+    api_response = api_instance.create_namespaced_deployment(
+        body=deployment,
+        namespace="default"
+    )
+    print(f"Deployment created. Status='{api_response.status}'")
+
+
+
+    api_instance = client.CoreV1Api()
+
+    service_spec = client.V1ServiceSpec(
+        type="ClusterIP",
+        ports=[client.V1ServicePort(port=80, target_port=5000)],
+        selector={"app": "blockchain-agent"}
+    )
+
+    # Define the service
+    service = client.V1Service(
+        api_version="v1",
+        kind="Service",
+        metadata=client.V1ObjectMeta(name="blockchain-agent-" + node_name),
+        spec=service_spec
+    )
+
+    # Create the service
+    api_response = api_instance.create_namespaced_service(
+        body=service,
+        namespace="default"
+    )
+
+
+
+
 def reset_config():
-    with open('/home/'+getpass.getuser()+'/config.json', 'r') as f:
+    with open('/home/'+getpass.getuser()+'/.oasees_sdk/config.json', 'r') as f:
         config = json.load(f)
     
     config['OASEES_CLUSTER_ID'] = -1
     config['agents'] = {}
+    config['DAO_TOKEN_ID'] = -1
 
-    with open('/home/'+getpass.getuser()+'/config.json', 'w') as f:
+    with open('/home/'+getpass.getuser()+'/.oasees_sdk/config.json', 'w') as f:
+        json.dump(config,f)
+
+@cli.command()
+def config_full_reset():
+    config = {}
+    with open('/home/'+getpass.getuser()+'/.oasees_sdk/config.json', 'w') as f:
         json.dump(config,f)
 
 
 def update_cluster_id(id):
     try:
-        with open('/home/'+getpass.getuser()+'/config.json', 'r') as f:
+        with open('/home/'+getpass.getuser()+'/.oasees_sdk/config.json', 'r') as f:
             config = json.load(f)
         
         config['OASEES_CLUSTER_ID'] = id
 
-        with open('/home/'+getpass.getuser()+'/config.json', 'w') as f:
+        with open('/home/'+getpass.getuser()+'/.oasees_sdk/config.json', 'w') as f:
             json.dump(config,f)
     except FileNotFoundError:
         click.echo("Error: Config file doesn't exist in the cli program's directory.")
 
 
 def config_exists():
+    if not os.path.isdir(SDK_PATH):
+        os.makedirs(SDK_PATH)
+
     default_config = {'BLOCKCHAIN_IP':'', 'PROVIDER_IP':'', 'IPFS_IP':'', 'ACCOUNT': '', 'KEY':'', 'OASEES_CLUSTER_ID': -1, 'agents':{}}
     try:
-        with open('/home/'+getpass.getuser()+'/config.json','r') as f:
+        with open('/home/'+getpass.getuser()+'/.oasees_sdk/config.json','r') as f:
             config = json.load(f)
             
         for key in default_config.keys():
             if key not in config.keys():
-                with open('/home/'+getpass.getuser()+'/config.json', 'w') as f:
+                with open('/home/'+getpass.getuser()+'/.oasees_sdk/config.json', 'w') as f:
                     json.dump(default_config,f)
                 break
 
     except FileNotFoundError:
-        with open('/home/'+getpass.getuser()+'/config.json', 'w') as f:
+        with open('/home/'+getpass.getuser()+'/.oasees_sdk/config.json', 'w') as f:
             config = default_config
             json.dump(config,f)
 
+
 def config_setup():
     try:
-        with open('/home/'+getpass.getuser()+'/config.json', 'r') as f:
+        with open('/home/'+getpass.getuser()+'/.oasees_sdk/config.json', 'r') as f:
             config = json.load(f)
 
         changed = False
 
         if (not config['BLOCKCHAIN_IP'] or not config['PROVIDER_IP'] or not config['IPFS_IP']):
             host_ip = input("Provide the ip of the host that the OASEES stack is running on: ")
             config['BLOCKCHAIN_IP'] = host_ip
@@ -482,28 +778,35 @@
             account = input("Provide your account's blockchain address: ")
             key = input("Provide your blockchain account's private key: ")
             config['ACCOUNT'] = account
             config['KEY'] = key
             changed = True
 
         if(changed):
-            with open('/home/'+getpass.getuser()+'/config.json', 'w') as f:
+            with open('/home/'+getpass.getuser()+'/.oasees_sdk/config.json', 'w') as f:
                 json.dump(config,f)
 
     except FileNotFoundError:
         click.echo("Error: config file not found.")
     
-@cli.command()
-def new_cluster():
-    mkdir_1 = subprocess.run(['sudo','mkdir','/etc/rancher'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
-    mkdir_2 = subprocess.run(['sudo','mkdir','/etc/rancher/k3s'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
-    echo = subprocess.run(['sudo','sh', '-c','echo "mirrors:\n  docker.io:\n  registry.k8s.io:" > /etc/rancher/k3s/registries.yaml'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
-    curl = subprocess.Popen(['curl','-sfL', 'https://get.k3s.io'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
-    result = subprocess.check_output(['sh','-s','-','--write-kubeconfig-mode','644', '--write-kubeconfig', '/home/'+getpass.getuser()+'/.kube/config','--embedded-registry'], stdin=curl.stdout)
-    click.echo(result)
-    curl.wait()
-
-    echo = subprocess.Popen(['echo', ipfs_manifest_str], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
-    result = subprocess.check_output(['kubectl','apply','-f','-'], stdin=echo.stdout)
-    click.echo(result)
-    echo.wait()
+
+
+
+
+
+# @cli.command()
+# def new_cluster():
+#     mkdir_1 = subprocess.run(['sudo','mkdir','/etc/rancher'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+#     mkdir_2 = subprocess.run(['sudo','mkdir','/etc/rancher/k3s'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+#     echo = subprocess.run(['sudo','sh', '-c','echo "mirrors:\n  docker.io:\n  registry.k8s.io:" > /etc/rancher/k3s/registries.yaml'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+#     curl = subprocess.Popen(['curl','-sfL', 'https://get.k3s.io'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+#     result = subprocess.check_output(['sh','-s','-','--write-kubeconfig-mode','644', '--write-kubeconfig', '/home/'+getpass.getuser()+'/.kube/config','--embedded-registry'], stdin=curl.stdout)
+#     click.echo(result)
+#     curl.wait()
+
+#     echo = subprocess.Popen(['echo', ipfs_manifest_str], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+#     result = subprocess.check_output(['kubectl','apply','-f','-'], stdin=echo.stdout)
+#     click.echo(result)
+#     echo.wait()
+
+
 config_exists()
```

### Comparing `oasees_sdk-0.2.9/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py` & `oasees_sdk-0.3.0/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.2.9/src/oasees_sdk/oasees_sdk/deploy_pipeline.py` & `oasees_sdk-0.3.0/src/oasees_sdk/oasees_sdk/deploy_pipeline.py`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.2.9/src/oasees_sdk/oasees_sdk/sdk.py` & `oasees_sdk-0.3.0/src/oasees_sdk/oasees_sdk/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,20 +107,21 @@
 
 
 def __get_config():
     results = __marketplace.caller({'from':__ACCOUNT_ADDRESS}).getJoinedDaos()
 
     client = ipfshttpclient.connect(f"/ip4/{__IPFS_HOST}/tcp/5001") 
     for r in results:
-        token_id = r[5]
-        content_hash = __nft.functions.tokenURI(token_id).call()
-
-        content = client.cat(content_hash)
-        content = content.decode("UTF-8")
-        config = yaml.safe_load(content)
+        if(r[6]):
+            token_id = r[5]
+            content_hash = __nft.functions.tokenURI(token_id).call()
+
+            content = client.cat(content_hash)
+            content = content.decode("UTF-8")
+            config = yaml.safe_load(content)
 
     with open('config', 'w') as f:
         yaml.safe_dump(config,f)
 
     client.close()
 
 
@@ -321,10 +322,7 @@
     box = f'╔{"═" * (width + indent * 2)}╗\n'  # upper_border
     if title:
         box += f'║{space}{title:<{width}}{space}║\n'  # title
         box += f'║{space}{"-" * len(title):<{width}}{space}║\n'  # underscore
     box += ''.join([f'║{space}{line:<{width}}{space}║\n' for line in lines])
     box += f'╚{"═" * (width + indent * 2)}╝'  # lower_border
     print(box)
-
-
-instructions()
```

### Comparing `oasees_sdk-0.2.9/PKG-INFO` & `oasees_sdk-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oasees_sdk
-Version: 0.2.9
+Version: 0.3.0
 Summary: Oasees SDK
 Author: Example Author
 Author-email: author@example.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

