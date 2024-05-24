# Comparing `tmp/quantfreedom-0.1.4.6.tar.gz` & `tmp/quantfreedom-0.2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantfreedom-0.1.4.6.tar", max compression
+gzip compressed data, was "quantfreedom-0.2.0.0.tar", max compression
```

## Comparing `quantfreedom-0.1.4.6.tar` & `quantfreedom-0.2.0.0.tar`

### file list

```diff
@@ -1,191 +1,31 @@
--rw-r--r--   0        0        0    11558 2023-12-05 17:44:20.643060 quantfreedom-0.1.4.6/LICENSE
--rw-r--r--   0        0        0      721 2024-03-24 18:04:13.439885 quantfreedom-0.1.4.6/pyproject.toml
--rw-r--r--   0        0        0      827 2023-12-26 15:12:55.073550 quantfreedom-0.1.4.6/quantfreedom/__init__.py
--rw-r--r--   0        0        0     1779 2023-12-26 15:12:55.073770 quantfreedom-0.1.4.6/quantfreedom/custom_logger.py
--rw-r--r--   0        0        0     2687 2023-12-05 17:44:20.648061 quantfreedom-0.1.4.6/quantfreedom/email_sender.py
--rw-r--r--   0        0        0    11451 2024-03-24 02:18:58.987176 quantfreedom-0.1.4.6/quantfreedom/enums.py
--rw-r--r--   0        0        0        0 2023-12-06 17:38:34.919615 quantfreedom-0.1.4.6/quantfreedom/exchanges/__init__.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.648061 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/__init__.py
--rw-r--r--   0        0        0    10728 2024-03-23 20:59:39.307695 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex.py
--rw-r--r--   0        0        0    15275 2024-03-24 02:14:39.987367 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/__init__.py
--rw-r--r--   0        0        0    10330 2023-12-05 17:44:20.650062 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/_websocket_stream.py
--rw-r--r--   0        0        0     5063 2023-12-05 17:44:20.650062 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/abi/erc20.json
--rw-r--r--   0        0        0    66315 2023-12-05 17:44:20.650062 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/abi/starkware-perpetuals.json
--rw-r--r--   0        0        0     1646 2023-12-05 17:44:20.650062 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/constants.py
--rw-r--r--   0        0        0      908 2023-12-05 17:44:20.651062 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/errors.py
--rw-r--r--   0        0        0    17272 2023-12-05 17:44:20.651062 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/eth.py
--rw-r--r--   0        0        0      414 2023-12-05 17:44:20.651062 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/eth_signing/__init__.py
--rw-r--r--   0        0        0     1938 2023-12-05 17:44:20.651062 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/eth_signing/eth_prive_action.py
--rw-r--r--   0        0        0     2673 2023-12-05 17:44:20.652063 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/eth_signing/onboarding_action.py
--rw-r--r--   0        0        0     4020 2023-12-05 17:44:20.652063 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/eth_signing/sign_off_chain_action.py
--rw-r--r--   0        0        0     3445 2023-12-05 17:44:20.652063 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/eth_signing/signers.py
--rw-r--r--   0        0        0     2864 2023-12-05 17:44:20.652063 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/eth_signing/util.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.653063 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/examples/__init__.py
--rw-r--r--   0        0        0     6220 2023-12-05 17:44:20.653063 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/examples/account_value.py
--rw-r--r--   0        0        0      151 2023-12-05 17:44:20.653063 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/examples/constants.py
--rw-r--r--   0        0        0     2058 2023-12-05 17:44:20.653063 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/examples/demo_deposit.py
--rw-r--r--   0        0        0     3050 2023-12-05 17:44:20.654063 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/examples/demo_private.py
--rw-r--r--   0        0        0     3344 2023-12-05 17:44:20.656063 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/examples/demo_private_v2.py
--rw-r--r--   0        0        0     1144 2023-12-05 17:44:20.656063 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/examples/demo_public.py
--rw-r--r--   0        0        0     1609 2023-12-05 17:44:20.656063 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/examples/demo_register.py
--rw-r--r--   0        0        0     1656 2023-12-05 17:44:20.657063 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/examples/demo_register_mul_address.py
--rw-r--r--   0        0        0     1647 2023-12-05 17:44:20.657063 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/examples/demo_register_v2.py
--rw-r--r--   0        0        0      662 2023-12-05 17:44:20.657063 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/examples/demo_sign.py
--rw-r--r--   0        0        0     4873 2023-12-05 17:44:20.657063 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/examples/demo_stark_key_sign.py
--rw-r--r--   0        0        0     1104 2023-12-05 17:44:20.658064 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/examples/demo_ws.py
--rw-r--r--   0        0        0     3047 2023-12-05 17:44:20.658064 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/examples/demo_ws_depthdata.py
--rw-r--r--   0        0        0     5544 2023-12-05 17:44:20.658064 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/examples/test_onboarding.py
--rw-r--r--   0        0        0     1358 2023-12-05 17:44:20.658064 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/exceptions.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.658893 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/helpers/__init__.py
--rw-r--r--   0        0        0      367 2023-12-05 17:44:20.658893 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/helpers/db.py
--rw-r--r--   0        0        0     2926 2023-12-05 17:44:20.658893 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/helpers/request_helpers.py
--rw-r--r--   0        0        0     1105 2024-03-24 02:15:05.168748 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/helpers/requests.py
--rw-r--r--   0        0        0      867 2023-12-05 17:44:20.659888 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/helpers/util.py
--rw-r--r--   0        0        0    28754 2023-12-05 17:44:20.659888 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/http_private.py
--rw-r--r--   0        0        0    30608 2023-12-05 17:44:20.659888 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/http_private_stark_key_sign.py
--rw-r--r--   0        0        0     3100 2023-12-05 17:44:20.660888 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/http_public.py
--rw-r--r--   0        0        0      132 2023-12-05 17:44:20.660888 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/models.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.660888 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/starkex/__init__.py
--rw-r--r--   0        0        0     4828 2024-03-24 02:15:02.314897 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/starkex/conditional_transfer.py
--rw-r--r--   0        0        0     1552 2024-03-24 02:11:58.153141 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/starkex/constants.py
--rw-r--r--   0        0        0     6268 2023-12-05 17:44:20.661888 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/starkex/helpers.py
--rw-r--r--   0        0        0     7092 2024-03-24 02:14:59.965059 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/starkex/order.py
--rw-r--r--   0        0        0     1319 2023-12-05 17:44:20.661888 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/starkex/signable.py
--rw-r--r--   0        0        0      293 2023-12-05 17:44:20.662888 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/starkex/starkex_resources/__init__.py
--rw-r--r--   0        0        0     3240 2023-12-05 17:44:20.662888 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/starkex/starkex_resources/cpp_signature.py
--rw-r--r--   0        0        0     3727 2023-12-05 17:44:20.662888 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/starkex/starkex_resources/math_utils.py
--rw-r--r--   0        0        0   104759 2023-12-05 17:44:20.663889 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/starkex/starkex_resources/pedersen_params.json
--rw-r--r--   0        0        0     1632 2024-03-24 02:12:51.511192 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/starkex/starkex_resources/proxy.py
--rw-r--r--   0        0        0    10549 2024-03-24 02:12:17.788151 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/starkex/starkex_resources/python_signature.py
--rw-r--r--   0        0        0     4387 2024-03-24 02:14:56.902179 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/starkex/transfer.py
--rw-r--r--   0        0        0     3012 2024-03-24 02:14:29.863407 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/starkex/withdrawal.py
--rw-r--r--   0        0        0     4712 2023-12-05 17:44:20.664888 quantfreedom-0.1.4.6/quantfreedom/exchanges/apex_exchange/apex_github/websocket_api.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.664888 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/__init__.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.664888 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/__init__.py
--rw-r--r--   0        0        0       23 2023-12-05 17:44:20.664888 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/__version__.py
--rw-r--r--   0        0        0     6710 2023-12-05 17:44:20.665888 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/api.py
--rw-r--r--   0        0        0     7413 2023-12-05 17:44:20.665888 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/cm_futures/__init__.py
--rw-r--r--   0        0        0    28825 2023-12-05 17:44:20.665888 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/cm_futures/account.py
--rw-r--r--   0        0        0     1434 2023-12-05 17:44:20.666888 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/cm_futures/data_stream.py
--rw-r--r--   0        0        0    20651 2023-12-05 17:44:20.666888 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/cm_futures/market.py
--rw-r--r--   0        0        0      492 2023-12-05 17:44:20.666888 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/cm_futures/portfolio_margin.py
--rw-r--r--   0        0        0     1420 2023-12-05 17:44:20.666888 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/error.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.667888 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/lib_usdm/__init__.py
--rw-r--r--   0        0        0      587 2023-12-05 17:44:20.667888 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/lib_usdm/authentication.py
--rw-r--r--   0        0        0     2141 2023-12-05 17:44:20.667888 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/lib_usdm/utils.py
--rw-r--r--   0        0        0     8206 2023-12-05 17:44:20.667888 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/um_futures/__init__.py
--rw-r--r--   0        0        0    32563 2023-12-05 17:44:20.668888 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/um_futures/account.py
--rw-r--r--   0        0        0     1438 2023-12-05 17:44:20.668888 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/um_futures/data_stream.py
--rw-r--r--   0        0        0    18944 2023-12-05 17:44:20.668888 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/um_futures/market.py
--rw-r--r--   0        0        0      480 2023-12-05 17:44:20.668888 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/um_futures/portfolio_margin.py
--rw-r--r--   0        0        0      384 2023-12-05 17:44:20.669889 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/agg_trades.py
--rw-r--r--   0        0        0      386 2023-12-05 17:44:20.669889 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/asset_index.py
--rw-r--r--   0        0        0      392 2023-12-05 17:44:20.669889 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/blvt_kline.py
--rw-r--r--   0        0        0      387 2023-12-05 17:44:20.670889 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/book_ticker.py
--rw-r--r--   0        0        0      410 2023-12-05 17:44:20.670889 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/continuous_klines.py
--rw-r--r--   0        0        0      397 2023-12-05 17:44:20.670889 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/depth.py
--rw-r--r--   0        0        0      378 2023-12-05 17:44:20.670889 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/exchange_info.py
--rw-r--r--   0        0        0      404 2023-12-05 17:44:20.671889 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/funding_rate.py
--rw-r--r--   0        0        0      485 2023-12-05 17:44:20.671889 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/historical_trades.py
--rw-r--r--   0        0        0      387 2023-12-05 17:44:20.671889 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/index_info.py
--rw-r--r--   0        0        0      418 2023-12-05 17:44:20.671889 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/index_price_kline.py
--rw-r--r--   0        0        0      388 2023-12-05 17:44:20.672890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/klines.py
--rw-r--r--   0        0        0      377 2023-12-05 17:44:20.672890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/mark_price.py
--rw-r--r--   0        0        0      417 2023-12-05 17:44:20.672890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/mark_price_klines.py
--rw-r--r--   0        0        0      389 2023-12-05 17:44:20.672890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/open_interest.py
--rw-r--r--   0        0        0      417 2023-12-05 17:44:20.673890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/open_interest_hist.py
--rw-r--r--   0        0        0      369 2023-12-05 17:44:20.673890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/ping.py
--rw-r--r--   0        0        0      404 2023-12-05 17:44:20.673890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/taker_long_short_ratio.py
--rw-r--r--   0        0        0      400 2023-12-05 17:44:20.673890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/ticker_24hr_price_change.py
--rw-r--r--   0        0        0      388 2023-12-05 17:44:20.673890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/ticker_price.py
--rw-r--r--   0        0        0      371 2023-12-05 17:44:20.674890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/time.py
--rw-r--r--   0        0        0      406 2023-12-05 17:44:20.674890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/top_long_short_account_ratio.py
--rw-r--r--   0        0        0      428 2023-12-05 17:44:20.674890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/top_long_short_position_ratio.py
--rw-r--r--   0        0        0      393 2023-12-05 17:44:20.674890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/market/trades.py
--rw-r--r--   0        0        0      383 2023-12-05 17:44:20.675890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/portfolio_margin/pm_exchange_info.py
--rw-r--r--   0        0        0      412 2023-12-05 17:44:20.675890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/stream/close_listen_key.py
--rw-r--r--   0        0        0      394 2023-12-05 17:44:20.675890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/stream/new_listen_key.py
--rw-r--r--   0        0        0      412 2023-12-05 17:44:20.676890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/stream/renew_listen_key.py
--rw-r--r--   0        0        0      797 2023-12-05 17:44:20.676890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/aysnc_download_info.py
--rw-r--r--   0        0        0      873 2023-12-05 17:44:20.676890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/cancel_batch_orders.py
--rw-r--r--   0        0        0      815 2023-12-05 17:44:20.676890 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/cancel_open_orders.py
--rw-r--r--   0        0        0      825 2023-12-05 17:44:20.677891 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/cancel_order.py
--rw-r--r--   0        0        0      824 2023-12-05 17:44:20.677891 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/change_leverage.py
--rw-r--r--   0        0        0      815 2023-12-05 17:44:20.677891 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/change_margin_type.py
--rw-r--r--   0        0        0      828 2023-12-05 17:44:20.677891 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/change_multi_asset_mode.py
--rw-r--r--   0        0        0      824 2023-12-05 17:44:20.678891 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/change_position_mode.py
--rw-r--r--   0        0        0      839 2023-12-05 17:44:20.678891 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/countdown_cancel_order.py
--rw-r--r--   0        0        0      836 2023-12-05 17:44:20.678891 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/download_transactions_asyn.py
--rw-r--r--   0        0        0     1060 2023-12-05 17:44:20.678891 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/get_account.py
--rw-r--r--   0        0        0      815 2023-12-05 17:44:20.679891 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/get_account_trades.py
--rw-r--r--   0        0        0      809 2023-12-05 17:44:20.679891 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/get_adl_quantile.py
--rw-r--r--   0        0        0      811 2023-12-05 17:44:20.679891 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/get_all_orders.py
--rw-r--r--   0        0        0      797 2023-12-05 17:44:20.679891 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/get_api_trading_status.py
--rw-r--r--   0        0        0      786 2023-12-05 17:44:20.680891 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/get_balance.py
--rw-r--r--   0        0        0      812 2023-12-05 17:44:20.680891 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/get_commission_rate.py
--rw-r--r--   0        0        0      791 2023-12-05 17:44:20.680891 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/get_force_orders.py
--rw-r--r--   0        0        0      797 2023-12-05 17:44:20.680891 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/get_income_history.py
--rw-r--r--   0        0        0      814 2023-12-05 17:44:20.681892 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/get_leverage_brackets.py
--rw-r--r--   0        0        0      799 2023-12-05 17:44:20.681892 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/get_multi_asset_mode.py
--rw-r--r--   0        0        0      833 2023-12-05 17:44:20.681892 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/get_open_orders.py
--rw-r--r--   0        0        0      807 2023-12-05 17:44:20.681892 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/get_orders.py
--rw-r--r--   0        0        0      822 2023-12-05 17:44:20.682892 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/get_position_margin_history.py
--rw-r--r--   0        0        0      796 2023-12-05 17:44:20.682892 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/get_position_mode.py
--rw-r--r--   0        0        0      794 2023-12-05 17:44:20.682892 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/get_position_risk.py
--rw-r--r--   0        0        0      846 2023-12-05 17:44:20.682892 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/modify_isolated_position_margin.py
--rw-r--r--   0        0        0      868 2023-12-05 17:44:20.683892 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/modify_order.py
--rw-r--r--   0        0        0     1170 2023-12-05 17:44:20.683892 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/new_batch_order.py
--rw-r--r--   0        0        0      929 2023-12-05 17:44:20.683892 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/new_order.py
--rw-r--r--   0        0        0      934 2023-12-05 17:44:20.683892 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/new_order_testing.py
--rw-r--r--   0        0        0      826 2023-12-05 17:44:20.684892 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/usdm_examples/trade/query_order.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.684892 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/websocket/__init__.py
--rw-r--r--   0        0        0     3724 2023-12-05 17:44:20.684892 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/websocket/binance_socket_manager.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.685892 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/websocket/cm_futures/__init__.py
--rw-r--r--   0        0        0    11762 2023-12-05 17:44:20.685892 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/websocket/cm_futures/websocket_client.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.685892 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/websocket/um_futures/__init__.py
--rw-r--r--   0        0        0     9487 2023-12-05 17:44:20.685892 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/websocket/um_futures/websocket_client.py
--rw-r--r--   0        0        0     3563 2023-12-05 17:44:20.686893 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_github/usdm_futures/websocket/websocket_client.py
--rw-r--r--   0        0        0     3495 2024-03-10 16:55:05.215677 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_us.py
--rw-r--r--   0        0        0    10067 2024-03-11 02:55:55.349875 quantfreedom-0.1.4.6/quantfreedom/exchanges/binance_exchange/binance_usdm.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.687893 quantfreedom-0.1.4.6/quantfreedom/exchanges/bybit_exchange/__init__.py
--rw-r--r--   0        0        0    36385 2024-03-24 17:00:35.618237 quantfreedom-0.1.4.6/quantfreedom/exchanges/bybit_exchange/bybit.py
--rw-r--r--   0        0        0    28826 2024-03-23 22:43:52.992460 quantfreedom-0.1.4.6/quantfreedom/exchanges/bybit_exchange/bybit_live_mode.py
--rw-r--r--   0        0        0     5715 2024-03-24 16:24:53.177767 quantfreedom-0.1.4.6/quantfreedom/exchanges/exchange.py
--rw-r--r--   0        0        0     1492 2023-12-26 15:12:55.077772 quantfreedom-0.1.4.6/quantfreedom/exchanges/live_exchange.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.697895 quantfreedom-0.1.4.6/quantfreedom/exchanges/mufex_exchange/__init__.py
--rw-r--r--   0        0        0    38613 2024-03-24 16:22:56.807587 quantfreedom-0.1.4.6/quantfreedom/exchanges/mufex_exchange/mufex.py
--rw-r--r--   0        0        0    28833 2024-03-23 22:42:07.807811 quantfreedom-0.1.4.6/quantfreedom/exchanges/mufex_exchange/mufex_live_mode.py
--rw-r--r--   0        0        0    10738 2024-03-24 13:12:52.470991 quantfreedom-0.1.4.6/quantfreedom/helper_funcs.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.699807 quantfreedom-0.1.4.6/quantfreedom/indicators/__init__.py
--rw-r--r--   0        0        0    22701 2024-03-09 15:31:30.638083 quantfreedom-0.1.4.6/quantfreedom/indicators/tv_indicators.py
--rw-r--r--   0        0        0    28472 2024-03-23 22:41:56.959998 quantfreedom-0.1.4.6/quantfreedom/live_mode.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.700775 quantfreedom-0.1.4.6/quantfreedom/nb_funcs/__init__.py
--rw-r--r--   0        0        0     2100 2023-12-26 15:12:55.081772 quantfreedom-0.1.4.6/quantfreedom/nb_funcs/nb_custom_logger.py
--rw-r--r--   0        0        0    18350 2024-03-23 22:42:08.610773 quantfreedom-0.1.4.6/quantfreedom/nb_funcs/nb_helper_funcs.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.700775 quantfreedom-0.1.4.6/quantfreedom/nb_funcs/nb_indicators/__init__.py
--rw-r--r--   0        0        0    11216 2023-12-05 17:44:20.701775 quantfreedom-0.1.4.6/quantfreedom/nb_funcs/nb_indicators/nb_indicators.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.701775 quantfreedom-0.1.4.6/quantfreedom/nb_funcs/nb_order_handler/__init__.py
--rw-r--r--   0        0        0     2920 2024-03-23 22:42:09.289469 quantfreedom-0.1.4.6/quantfreedom/nb_funcs/nb_order_handler/nb_decrease_position.py
--rw-r--r--   0        0        0    26364 2024-03-23 22:42:09.972568 quantfreedom-0.1.4.6/quantfreedom/nb_funcs/nb_order_handler/nb_increase_position.py
--rw-r--r--   0        0        0    10882 2023-12-05 17:44:20.702775 quantfreedom-0.1.4.6/quantfreedom/nb_funcs/nb_order_handler/nb_leverage.py
--rw-r--r--   0        0        0    15351 2024-03-23 22:42:55.016579 quantfreedom-0.1.4.6/quantfreedom/nb_funcs/nb_order_handler/nb_stop_loss.py
--rw-r--r--   0        0        0     4817 2024-03-23 22:42:55.668518 quantfreedom-0.1.4.6/quantfreedom/nb_funcs/nb_order_handler/nb_take_profit.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.702775 quantfreedom-0.1.4.6/quantfreedom/nb_funcs/nb_simulate/__init__.py
--rw-r--r--   0        0        0    12921 2023-12-05 17:44:20.703775 quantfreedom-0.1.4.6/quantfreedom/nb_funcs/nb_simulate/nb_sim_base.py
--rw-r--r--   0        0        0    29177 2024-03-23 22:42:56.287516 quantfreedom-0.1.4.6/quantfreedom/nb_funcs/nb_simulate/nb_sim_df.py
--rw-r--r--   0        0        0    23405 2024-03-23 22:42:57.088517 quantfreedom-0.1.4.6/quantfreedom/nb_funcs/nb_simulate/nb_sim_or.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.703775 quantfreedom-0.1.4.6/quantfreedom/nb_funcs/nb_strategies/__init__.py
--rw-r--r--   0        0        0     4988 2023-12-05 17:44:20.704775 quantfreedom-0.1.4.6/quantfreedom/nb_funcs/nb_strategies/nb_strategy.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.704775 quantfreedom-0.1.4.6/quantfreedom/order_handler/__init__.py
--rw-r--r--   0        0        0    28491 2024-03-24 15:39:09.493083 quantfreedom-0.1.4.6/quantfreedom/order_handler/increase_position.py
--rw-r--r--   0        0        0     9620 2024-03-23 23:09:16.703498 quantfreedom-0.1.4.6/quantfreedom/order_handler/leverage.py
--rw-r--r--   0        0        0    16758 2024-03-24 15:23:24.562425 quantfreedom-0.1.4.6/quantfreedom/order_handler/order.py
--rw-r--r--   0        0        0     9914 2023-12-26 15:12:55.084773 quantfreedom-0.1.4.6/quantfreedom/order_handler/stop_loss.py
--rw-r--r--   0        0        0     5489 2024-03-23 22:59:34.795758 quantfreedom-0.1.4.6/quantfreedom/order_handler/take_profit.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.705776 quantfreedom-0.1.4.6/quantfreedom/plotting/__init__.py
--rw-r--r--   0        0        0    20633 2024-02-22 15:37:26.901060 quantfreedom-0.1.4.6/quantfreedom/plotting/plotting_base.py
--rw-r--r--   0        0        0    25042 2024-03-24 15:25:35.127696 quantfreedom-0.1.4.6/quantfreedom/simulate.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.706776 quantfreedom-0.1.4.6/quantfreedom/strategies/__init__.py
--rw-r--r--   0        0        0     3518 2024-03-03 17:21:06.415740 quantfreedom-0.1.4.6/quantfreedom/strategies/strategy.py
--rw-r--r--   0        0        0     3118 2023-12-26 15:12:55.087773 quantfreedom-0.1.4.6/quantfreedom/utils.py
--rw-r--r--   0        0        0     1007 1970-01-01 00:00:00.000000 quantfreedom-0.1.4.6/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-12-05 17:44:20.643060 quantfreedom-0.2.0.0/LICENSE
+-rw-r--r--   0        0        0     2134 2024-05-19 15:27:32.666161 quantfreedom-0.2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1363 2024-05-19 14:11:30.926838 quantfreedom-0.2.0.0/quantfreedom/__init__.py
+-rw-r--r--   0        0        0      222 2024-05-16 14:35:07.370622 quantfreedom-0.2.0.0/quantfreedom/backtesters/__init__.py
+-rw-r--r--   0        0        0    11920 2024-05-22 16:37:44.092927 quantfreedom-0.2.0.0/quantfreedom/backtesters/bt_live.py
+-rw-r--r--   0        0        0    26622 2024-05-22 16:38:16.972085 quantfreedom-0.2.0.0/quantfreedom/backtesters/bt_regular.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:17:05.091942 quantfreedom-0.2.0.0/quantfreedom/core/__init__.py
+-rw-r--r--   0        0        0    12777 2024-05-19 14:11:08.879829 quantfreedom-0.2.0.0/quantfreedom/core/enums.py
+-rw-r--r--   0        0        0    21711 2024-05-17 14:31:43.097467 quantfreedom-0.2.0.0/quantfreedom/core/plotting_base.py
+-rw-r--r--   0        0        0    11179 2024-05-22 15:39:50.177126 quantfreedom-0.2.0.0/quantfreedom/core/strategy.py
+-rw-r--r--   0        0        0      294 2024-05-14 13:37:33.155122 quantfreedom-0.2.0.0/quantfreedom/exchanges/__init__.py
+-rw-r--r--   0        0        0     6099 2024-05-19 14:14:16.992505 quantfreedom-0.2.0.0/quantfreedom/exchanges/binance_usdm.py
+-rw-r--r--   0        0        0    38437 2024-05-14 16:11:25.497110 quantfreedom-0.2.0.0/quantfreedom/exchanges/bybit.py
+-rw-r--r--   0        0        0     6870 2024-05-16 19:00:06.369046 quantfreedom-0.2.0.0/quantfreedom/exchanges/exchange.py
+-rw-r--r--   0        0        0    41125 2024-05-06 16:11:37.496638 quantfreedom-0.2.0.0/quantfreedom/exchanges/mufex.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:45:24.956684 quantfreedom-0.2.0.0/quantfreedom/helpers/__init__.py
+-rw-r--r--   0        0        0     7914 2024-05-05 13:17:05.095785 quantfreedom-0.2.0.0/quantfreedom/helpers/bsc_scan.py
+-rw-r--r--   0        0        0     2078 2024-05-15 14:15:07.568687 quantfreedom-0.2.0.0/quantfreedom/helpers/custom_logger.py
+-rw-r--r--   0        0        0     2687 2024-05-17 15:07:48.934089 quantfreedom-0.2.0.0/quantfreedom/helpers/email_sender.py
+-rw-r--r--   0        0        0    12014 2024-05-24 16:31:44.154454 quantfreedom-0.2.0.0/quantfreedom/helpers/helper_funcs.py
+-rw-r--r--   0        0        0     3794 2024-05-17 15:07:55.283120 quantfreedom-0.2.0.0/quantfreedom/helpers/utils.py
+-rw-r--r--   0        0        0        0 2023-12-05 17:44:20.699807 quantfreedom-0.2.0.0/quantfreedom/indicators/__init__.py
+-rw-r--r--   0        0        0    22925 2024-05-22 14:26:53.128699 quantfreedom-0.2.0.0/quantfreedom/indicators/tv_indicators.py
+-rw-r--r--   0        0        0        0 2023-12-05 17:44:20.704775 quantfreedom-0.2.0.0/quantfreedom/order_handler/__init__.py
+-rw-r--r--   0        0        0    28538 2024-05-19 14:14:54.910441 quantfreedom-0.2.0.0/quantfreedom/order_handler/increase_position.py
+-rw-r--r--   0        0        0     9848 2024-05-17 15:08:35.463005 quantfreedom-0.2.0.0/quantfreedom/order_handler/leverage.py
+-rw-r--r--   0        0        0    17107 2024-05-17 15:08:53.075942 quantfreedom-0.2.0.0/quantfreedom/order_handler/order.py
+-rw-r--r--   0        0        0    10626 2024-05-17 15:08:55.366393 quantfreedom-0.2.0.0/quantfreedom/order_handler/stop_loss.py
+-rw-r--r--   0        0        0     5671 2024-05-17 15:08:56.215120 quantfreedom-0.2.0.0/quantfreedom/order_handler/take_profit.py
+-rw-r--r--   0        0        0      203 2024-04-04 19:41:17.532684 quantfreedom-0.2.0.0/README.md
+-rw-r--r--   0        0        0     2310 1970-01-01 00:00:00.000000 quantfreedom-0.2.0.0/PKG-INFO
```

### Comparing `quantfreedom-0.1.4.6/LICENSE` & `quantfreedom-0.2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.1.4.6/quantfreedom/custom_logger.py` & `quantfreedom-0.2.0.0/quantfreedom/helpers/custom_logger.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,64 @@
-from datetime import datetime
-import os, logging
-import time
-
-FORMATTER = "%(asctime)s - %(levelname)s - %(filename)s - %(funcName)s() - %(lineno)d - %(message)s"
+from datetime import datetime, timezone
+from logging import getLogger, Formatter, FileHandler
+from os.path import join, exists
+from os import makedirs
+from time import gmtime
 
 
 def set_loggers(
-    log_folder: str,
+    disable_logger: bool,
+    log_path: str = None,
+    logger_level: str = "INFO",
 ):
-    logging.Formatter.converter = time.gmtime
-    # creating images folder
-    complete_path = os.path.join(log_folder, "logs", "images")
-    isExist = os.path.exists(complete_path)
-    if not isExist:
-        os.makedirs(complete_path)
-
-    # Info logs
-    complete_path = os.path.join(log_folder, "logs")
-    isExist = os.path.exists(complete_path)
-    if not isExist:
-        os.makedirs(complete_path)
-    filename = os.path.join(complete_path, f'info_{datetime.utcnow().strftime("%m-%d-%Y_%H-%M-%S")}.log')
-    logger = logging.getLogger("info")
-    logger.setLevel(logging.DEBUG)
-    logger.addHandler(create_logging_handler(filename, FORMATTER))
-    logger.info("Testing info log")
-
-    complete_path = os.path.join(log_folder, "logs", "trades")
-    isExist = os.path.exists(complete_path)
-    if not isExist:
-        os.makedirs(complete_path)
-    filename = os.path.join(complete_path, f'trades_{datetime.utcnow().strftime("%m-%d-%Y_%H-%M-%S")}.log')
-    logger = logging.getLogger("trades")
-    logger.setLevel(logging.INFO)
-    logger.addHandler(create_logging_handler(filename, FORMATTER))
-    logger.info("Testing trades log")
+    if disable_logger:
+        getLogger().disabled = True
+    else:
+        try:
+            Formatter.converter = gmtime
+            log_folder_path = join(log_path, "z_logs")
+
+            isExist = exists(log_folder_path)
+            if not isExist:
+                makedirs(log_folder_path)
+
+            file_format = f'info_{datetime.now(tz=timezone.utc).strftime("%Y-%m-%d_%H-%M-%S")}.log'
+            filename = join(log_folder_path, file_format)
+
+            logger = getLogger()
+            logger.disabled = False
+            logger.setLevel(logger_level.upper())
+            logger.addHandler(create_logging_handler(filename=filename))
+            logger.info("Testing info log")
+
+        except:  # this is for the aws lambda function
+            logger = getLogger()
+            logger.disabled = False
+            logger.setLevel(logger_level.upper())
+
+            log_handler = logger.handlers[0]
+            log_format = "\n" + "%(levelname)s - %(filename)s - %(funcName)s() - %(lineno)d - %(message)s"
+            log_handler.setFormatter(
+                Formatter(
+                    fmt=log_format,
+                    datefmt="%Y-%m-%d %H:%M:%S",
+                )
+            )
+
+            pass
 
 
-def create_logging_handler(filename: str, FORMATTER: str):
+def create_logging_handler(filename: str):
     handler = None
     try:
-        handler = logging.FileHandler(
-            filename=filename,
-            mode="w",
+        handler = FileHandler(filename=filename, mode="w")
+        log_format = "%(asctime)s - %(levelname)s - %(filename)s - %(funcName)s() - %(lineno)d - %(message)s"
+        handler.setFormatter(
+            Formatter(
+                fmt=log_format,
+                datefmt="%Y-%m-%d %H:%M:%S",
+            )
         )
-        handler.setFormatter(logging.Formatter(fmt=FORMATTER))
     except Exception as e:
-        print(f"Couldnt init logging system with file [{filename}]. Desc=[{e}]")
+        raise Exception(f"Couldnt create logging handler. Desc=[{e}]")
 
     return handler
```

### Comparing `quantfreedom-0.1.4.6/quantfreedom/email_sender.py` & `quantfreedom-0.2.0.0/quantfreedom/helpers/email_sender.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     ):
         subject = "Plotting"
         body = f"We are about to plot"
         self._send_email(subject=subject, body=body)
 
     def email_pnl(self, pnl: float):
         subject = "Updated PNL"
-        body = f"We got a new pnl ... i hope it is positive ${round(pnl, 3)}"
+        body = f"We got a new pnl ... i hope it is positive ${round(pnl, 2)}"
         self._send_email(subject=subject, body=body)
 
     def email_error_msg(self, msg):
         subject = "There's been an error"
         body = msg
         self._send_email(subject=subject, body=body)
```

### Comparing `quantfreedom-0.1.4.6/quantfreedom/enums.py` & `quantfreedom-0.2.0.0/quantfreedom/core/enums.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,71 @@
-from typing import NamedTuple
 import numpy as np
+from typing import NamedTuple, Optional
+
+
+class CurrentFootprintCandleTuple(NamedTuple):
+    open_dateime: Optional[np.datetime64] = None
+    open_timestamp: Optional[int] = None
+    close_dateime: Optional[np.datetime64] = None
+    close_timestamp: Optional[int] = None
+    durations_seconds: Optional[float] = None
+    open_price: Optional[float] = None
+    high_price: Optional[float] = None
+    low_price: Optional[float] = None
+    close_price: Optional[float] = None
+    usdt_volume: Optional[float] = None
+    asset_volume: Optional[float] = None
+
+
+class FootprintCandlesTuple(NamedTuple):
+    candle_open_datetimes: Optional[np.ndarray] = None
+    candle_open_timestamps: Optional[np.ndarray] = None
+    candle_close_datetimes: Optional[np.ndarray] = None
+    candle_close_timestamps: Optional[np.ndarray] = None
+    candle_durations_seconds: Optional[np.ndarray] = None
+    candle_open_prices: Optional[np.ndarray] = None
+    candle_high_prices: Optional[np.ndarray] = None
+    candle_low_prices: Optional[np.ndarray] = None
+    candle_close_prices: Optional[np.ndarray] = None
+    candle_usdt_volumes: Optional[np.ndarray] = None
+    candle_asset_volumes: Optional[np.ndarray] = None
+    candle_trade_counts: Optional[np.ndarray] = None
+    candle_deltas: Optional[np.ndarray] = None
+    candle_delta_percents: Optional[np.ndarray] = None
+    candle_buy_volumes: Optional[np.ndarray] = None
+    candle_buy_counts: Optional[np.ndarray] = None
+    candle_sell_volumes: Optional[np.ndarray] = None
+    candle_sell_counts: Optional[np.ndarray] = None
+    candle_cvds: Optional[np.ndarray] = None
+    candle_pocs: Optional[np.ndarray] = None
+    candle_high_lows: Optional[np.ndarray] = None
+    prices_tuple: Optional[tuple] = None
+    prices_buy_vol_tuple: Optional[tuple] = None
+    prices_buy_count_tuple: Optional[tuple] = None
+    prices_sell_vol_tuple: Optional[tuple] = None
+    prices_sell_count_tuple: Optional[tuple] = None
+    prices_delta_tuple: Optional[tuple] = None
+    prices_delta_percent_tuple: Optional[tuple] = None
+    prices_volume_tuple: Optional[tuple] = None
+    prices_trade_count_tuple: Optional[tuple] = None
 
 
 class CandleBodyTypeT(NamedTuple):
-    Timestamp: int = 0
-    Open: int = 1
-    High: int = 2
-    Low: int = 3
-    Close: int = 4
-    Volume: int = 5
-    Nothing: int = 6
+    OpenDatetime: int = 0
+    OpenTimestamp: int = 1
+    CloseDatetime: int = 2
+    CloseTimestamp: int = 3
+    DurationSeconds: int = 4
+    Open: int = 5
+    High: int = 6
+    Low: int = 7
+    Close: int = 8
+    UsdtVolume: int = 9
+    AssetVolume: int = 10
+    Nothing: int = 11
 
 
 CandleBodyType = CandleBodyTypeT()
 
 
 class IncreasePositionTypeT(NamedTuple):
     """
@@ -171,16 +223,15 @@
 ############################################################
 ############################################################
 ############################################################
 
 
 class AccountState(NamedTuple):
     # where we are at
-    ind_set_index: int
-    dos_index: int
+    set_idx: int
     bar_index: int
     timestamp: int
     # account info
     available_balance: float
     cash_borrowed: float
     cash_used: float
     equity: float
@@ -198,51 +249,35 @@
     ----------
     gains_pct_filter : float = -np.inf
         Will not record any strategies whos gains % result is below gains_pct_filter
     qf_filter : float = -np.inf
         Will not record any strategies whos qf score result is below the qf filter. qf_score is between -1 to 1,
     total_trade_filter : int = -1
         Will not record any strategies whos total trades result is below total trades filter.
-    record_size : int = 10000
-        The amount of records you want to to save. Keep this number as low as possible to save memory.
 
     """
 
     gains_pct_filter: float = -np.inf
     qf_filter: float = -np.inf
     total_trade_filter: int = -1
-    record_size: int = 10000
-
-
-class DynamicOrderSettingsArrays(NamedTuple):
-    max_trades: np.array
-    account_pct_risk_per_trade: np.array
-    risk_reward: np.array
-    sl_based_on_add_pct: np.array
-    sl_based_on_lookback: np.array
-    sl_bcb_type: np.array
-    sl_to_be_cb_type: np.array
-    sl_to_be_when_pct: np.array
-    trail_sl_bcb_type: np.array
-    trail_sl_by_pct: np.array
-    trail_sl_when_pct: np.array
 
 
 class DynamicOrderSettings(NamedTuple):
-    max_trades: int
-    account_pct_risk_per_trade: float
-    risk_reward: float
-    sl_based_on_add_pct: float
-    sl_based_on_lookback: int
-    sl_bcb_type: int
-    sl_to_be_cb_type: int
-    sl_to_be_when_pct: float
-    trail_sl_bcb_type: int
-    trail_sl_by_pct: float
-    trail_sl_when_pct: float
+    account_pct_risk_per_trade: np.ndarray
+    max_trades: np.ndarray
+    risk_reward: np.ndarray
+    sl_based_on_add_pct: np.ndarray
+    sl_based_on_lookback: np.ndarray
+    sl_bcb_type: np.ndarray
+    sl_to_be_cb_type: np.ndarray
+    sl_to_be_when_pct: np.ndarray
+    trail_sl_bcb_type: np.ndarray
+    trail_sl_by_pct: np.ndarray
+    trail_sl_when_pct: np.ndarray
+    settings_index: np.ndarray = np.array([0])
 
 
 class ExchangeSettings(NamedTuple):
     asset_tick_step: int
     leverage_mode: int
     leverage_tick_step: int
     limit_fee_pct: float
@@ -288,52 +323,36 @@
     trail_sl_bool: bool
     z_or_e_type: str
 
 
 class RejectedOrder(Exception):
     def __init__(
         self,
-        order_status: OrderStatus = None,
         msg: str = None,
     ):
-        self.order_status = order_status
         self.msg = msg
 
 
 class DecreasePosition(Exception):
     def __init__(
         self,
-        order_status: OrderStatus = None,
-        exit_price: float = None,
-        exit_fee_pct: float = None,
+        order_status: OrderStatus = None,  # type: ignore
+        exit_price: Optional[float] = None,
+        exit_fee_pct: Optional[float] = None,
         msg: str = None,
     ):
         self.order_status = order_status
         self.exit_price = exit_price
         self.exit_fee_pct = exit_fee_pct
         self.msg = msg
 
 
-class MoveStopLoss(Exception):
-    def __init__(
-        self,
-        order_status: OrderStatus = None,
-        sl_price: float = None,
-        can_move_sl_to_be: bool = None,
-        msg: str = None,
-    ):
-        self.order_status = order_status
-        self.sl_price = sl_price
-        self.can_move_sl_to_be = can_move_sl_to_be
-        self.msg = msg
-
-
 order_settings_array_dt = np.dtype(
     [
-        ("or_set_idx", np.int_),
+        ("set_idx", np.int_),
         ("increase_position_type", np.int_),
         ("leverage_type", np.int_),
         ("max_equity_risk_pct", np.float_),
         ("long_or_short", np.int_),
         ("account_pct_risk_per_trade", np.float_),
         ("risk_reward", np.float_),
         ("sl_based_on_add_pct", np.float_),
@@ -354,16 +373,15 @@
     ],
     align=True,
 )
 
 
 or_dt = np.dtype(
     [
-        ("ind_set_idx", np.int_),
-        ("or_set_idx", np.int_),
+        ("set_idx", np.int_),
         ("bar_idx", np.int_),
         ("timestamp", np.int64),
         ("order_status", np.int_),
         ("equity", np.float_),
         ("available_balance", np.float_),
         ("cash_borrowed", np.float_),
         ("cash_used", np.float_),
@@ -386,21 +404,20 @@
         ("tp_price", np.float_),
     ],
     align=True,
 )
 
 strat_df_array_dt = np.dtype(
     [
-        ("ind_set_idx", np.int_),
-        ("dos_index", np.int_),
+        ("set_idx", np.int_),
         ("total_trades", np.float_),
         ("wins", np.int_),
         ("losses", np.int_),
         ("gains_pct", np.float_),
         ("win_rate", np.float_),
         ("qf_score", np.float_),
         ("fees_paid", np.float_),
-        ("ending_eq", np.float_),
         ("total_pnl", np.float_),
+        ("ending_eq", np.float_),
     ],
     align=True,
 )
```

### Comparing `quantfreedom-0.1.4.6/quantfreedom/exchanges/bybit_exchange/bybit.py` & `quantfreedom-0.2.0.0/quantfreedom/exchanges/bybit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,45 @@
+from typing import Optional
 import hashlib
 import hmac
 import inspect
 import numpy as np
 from time import sleep, time
 from datetime import datetime, timezone
 from requests import get, post
-from quantfreedom.enums import ExchangeSettings, LeverageModeType, PositionModeType, TriggerDirectionType
+from quantfreedom.core.enums import (
+    ExchangeSettings,
+    FootprintCandlesTuple,
+    LeverageModeType,
+    PositionModeType,
+    TriggerDirectionType,
+)
 
 from quantfreedom.exchanges.exchange import UNIVERSAL_TIMEFRAMES, Exchange
 
 BYBIT_TIMEFRAMES = ["1", "5", "15", "30", "60", "120", "240", "360", "720", "D", "W"]
 
 
 class Bybit(Exchange):
     def __init__(
         # Exchange Vars
         self,
-        use_test_net: bool,
+        use_testnet: bool,
         api_key: str = None,
         secret_key: str = None,
     ):
         """
         main docs page https://bybit-exchange.github.io/docs/v5/intro
         [upgrade to unified account](https://www.bybit.com/en/help-center/article/UTA-guide#cb)
         """
         if api_key:
             self.api_key = api_key
             self.secret_key = secret_key
 
-        if use_test_net:
+        if use_testnet:
             self.url_start = "https://api-testnet.bybit.com"
         else:
             self.url_start = "https://api.bybit.com"
             self.ws_url_start = "wss://stream.bybit.com/v5/public"
 
     """
     ################################################################
@@ -124,15 +131,15 @@
         self,
         symbol: str,
         timeframe: str,
         since_datetime: datetime = None,
         until_datetime: datetime = None,
         candles_to_dl: int = 1000,
         category: str = "linear",
-    ):
+    ) -> FootprintCandlesTuple:
         """
         Summary
         -------
         [Bybit candle docs](https://bybit-exchange.github.io/docs/v5/market/kline)
 
         Explainer Video
         ---------------
@@ -176,56 +183,77 @@
             "symbol": symbol,
             "interval": ex_timeframe,
             "start": since_timestamp,
             "end": until_timestamp,
             "limit": 1000,
         }
 
+        waiter_timestamp = until_timestamp + 5000 - (self.timeframe_in_ms * 2)
+        # add 5 seconds back so it is a flat time, then subtract the timeframe * two
+
         while params["end"] - self.timeframe_in_ms > since_timestamp:
             try:
                 response: dict = get(url=self.url_start + end_point, params=params).json()
                 new_candles = response["result"]["list"]
+
+                first_candle_timestamp = int(new_candles[0][0])
                 last_candle_timestamp = int(new_candles[-1][0])
-                if last_candle_timestamp == params["start"]:
+
+                if first_candle_timestamp == waiter_timestamp:
+                    # checking to see if the first candle we download is one candle behind what we should be downloading
+                    # if it is then we are trying to dl candles too soon and need to wait to try again
+                    print("sleeping .2 seconds")
                     sleep(0.2)
                 else:
                     candles_list.extend(new_candles)
                     # add 2 sec so we don't download the same candle two times
                     params["end"] = last_candle_timestamp - 2000
-                1 + 1
 
             except Exception as e:
                 raise Exception(f"Bybit get_candles {response.get('message')} - > {e}")
 
         candles = np.flip(np.array(candles_list, dtype=np.float_)[:, :-1], axis=0)
+        open_timestamps = candles[:, 0].astype(np.int64)
+
+        Footprint_Candles_Tuple = FootprintCandlesTuple(
+            candle_open_datetimes=open_timestamps.astype("datetime64[ms]"),
+            candle_open_timestamps=open_timestamps,
+            candle_durations_seconds=np.full(candles.shape[0], int(self.timeframe_in_ms / 1000)),
+            candle_open_prices=candles[:, 1],
+            candle_high_prices=candles[:, 2],
+            candle_low_prices=candles[:, 3],
+            candle_close_prices=candles[:, 4],
+            candle_asset_volumes=candles[:, 5],
+            candle_usdt_volumes=np.around(a=candles[:, 5] * candles[:, 4], decimals=3),
+        )
         self.last_fetched_ms_time = int(candles[-1, 0])
 
-        return candles
+        return Footprint_Candles_Tuple
 
     def create_order(
         self,
         symbol: str,
         buy_sell: str,
         position_mode: int,
         order_type: str,
         asset_size: float,
         category: str = "linear",
         time_in_force: str = "GTC",
-        price: float = None,
-        triggerDirection: int = None,
-        triggerPrice: float = None,
+        price: Optional[float] = None,
+        triggerDirection: Optional[int] = None,
+        triggerPrice: Optional[float] = None,
         triggerBy: str = None,
         tpTriggerBy: str = None,
         slTriggerBy: str = None,
         custom_order_id: str = None,
-        takeProfit: float = None,
-        stopLoss: float = None,
+        takeProfit: Optional[float] = None,
+        stopLoss: Optional[float] = None,
         reduce_only: bool = None,
         closeOnTrigger: bool = None,
-        isLeverage: int = None,
+        isLeverage: Optional[int] = None,
     ):
         """
         https://bybit-exchange.github.io/docs/v5/order/create-order
         """
         end_point = "/v5/order/create"
         params = {}
         params["symbol"] = symbol.upper()
@@ -251,15 +279,15 @@
         response = self.__HTTP_post_request(end_point=end_point, params=params)
         try:
             order_id = response["result"]["orderId"]
             return order_id
         except Exception as e:
             raise Exception(f"Bybit create_order {response['retMsg']} -> {e}")
 
-    def create_long_hedge_mode_entry_market_order_stoploss(
+    def create_long_hedge_mode_entry_market_order_with_stoploss(
         self,
         asset_size: float,
         symbol: str,
         sl_price: float,
     ):
         return self.create_order(
             symbol=symbol,
@@ -302,31 +330,31 @@
             time_in_force="PostOnly",
         )
 
     def create_long_hedge_mode_sl_order(
         self,
         asset_size: float,
         symbol: str,
-        trigger_price: float,
+        sl_price: float,
     ):
         return self.create_order(
             symbol=symbol,
             position_mode=PositionModeType.BuySide,
             buy_sell="Sell",
             order_type="Market",
             asset_size=asset_size,
-            triggerPrice=trigger_price,
+            triggerPrice=sl_price,
             reduce_only=True,
             triggerDirection=TriggerDirectionType.Fall,
             time_in_force="GTC",
         )
 
     def get_position_info(
         self,
-        symbol: str,
+        symbol: str = None,
         baseCoin: str = None,
         category: str = "linear",
         limit: int = 50,
         settleCoin: str = None,
     ):
         """
         https://bybit-exchange.github.io/docs/v5/position
@@ -531,18 +559,17 @@
         params["orderStatus"] = orderStatus
         params["settleCoin"] = settleCoin
         params["startTime"] = since_datetime
         params["symbol"] = symbol
         response: dict = self.__HTTP_get_request(end_point=end_point, params=params)
         try:
             data_list = response["result"]["list"]
-            data_list[0]  # try this to see if anything is in here
             return data_list
         except Exception as e:
-            raise Exception(f"Bybit get_open_orders = Data or List is empty {response['retMsg']} -> {e}")
+            raise Exception(f"Bybit get_open_orders = {response['retMsg']} -> {e}")
 
     def check_if_order_open(
         self,
         order_id: str,
         symbol: str = None,
     ):
         data_list = self.get_open_orders(order_id=order_id, symbol=symbol)
@@ -662,60 +689,32 @@
             if response["retMsg"] == "Request accepted":
                 return True
             else:
                 raise Exception
         except Exception as e:
             raise Exception(f"Bybit set_leverage_mode = Data or List is empty {response['retMsg']} -> {e}")
 
-    # def set_leverage_mode(
-    #     self,
-    #     symbol: str,
-    #     leverage_mode: int,
-    #     category: str = "linear",
-    #     leverage: int = 5,
-    # ):
-    #     """
-    #     https://bybit-exchange.github.io/docs/v5/position/cross-isolate
-    #     Cross/isolated mode. 0: cross margin mode; 1: isolated margin mode
-    #     """
-    #     end_point = "/v5/position/switch-isolated"
-    #     leverage_str = str(leverage)
-    #     params = {}
-    #     params["symbol"] = symbol
-    #     params["category"] = category
-    #     params["tradeMode"] = leverage_mode
-    #     params["buyLeverage"] = leverage_str
-    #     params["sellLeverage"] = leverage_str
-    #     response: dict = self.__HTTP_post_request(end_point=end_point, params=params)
-    #     try:
-    #         if response["retMsg"] in ["OK", "Cross/isolated margin mode is not modified"]:
-    #             return True
-    #         else:
-    #             raise Exception
-    #     except Exception as e:
-    #         raise Exception(f"Bybit set_leverage_mode = Data or List is empty {response['retMsg']} -> {e}")
-
     def adjust_order(
         self,
         symbol: str,
-        asset_size: float = None,
+        asset_size: Optional[float] = None,
         category: str = "linear",
         custom_order_id: str = None,
         orderIv: str = None,
         order_id: str = None,
-        price: float = None,
-        slLimitPrice: float = None,
-        slTriggerBy: float = None,
-        stopLoss: float = None,
-        takeProfit: float = None,
-        tpLimitPrice: float = None,
+        price: Optional[float] = None,
+        slLimitPrice: Optional[float] = None,
+        slTriggerBy: Optional[float] = None,
+        stopLoss: Optional[float] = None,
+        takeProfit: Optional[float] = None,
+        tpLimitPrice: Optional[float] = None,
         tpslMode: str = None,
-        tpTriggerBy: float = None,
-        triggerBy: float = None,
-        triggerPrice: float = None,
+        tpTriggerBy: Optional[float] = None,
+        triggerBy: Optional[float] = None,
+        triggerPrice: Optional[float] = None,
     ):
         """
         https://bybit-exchange.github.io/docs/v5/order/amend-order
         """
         end_point = "/v5/order/amend"
         params = {}
         params["category"] = category
@@ -953,15 +952,15 @@
         self,
         symbol: str,
     ):
         true_false = self.set_position_mode(symbol=symbol, position_mode=0)
 
         return true_false
 
-    def set_and_get_exchange_settings(
+    def set_and_get_exchange_settings_tuple(
         self,
         leverage_mode: int,
         position_mode: int,
         symbol: str,
     ):
         self.position_mode = position_mode
         if position_mode == PositionModeType.HedgeMode:
@@ -1004,7 +1003,63 @@
         func_list = inspect.getmembers(Bybit, predicate=inspect.isfunction)
         new_list = []
         for func in func_list:
             func_name = func[0]
             if not "_" in func_name[0]:
                 new_list.append(func[0])
         return new_list
+
+    def close_hedge_positions_and_orders(
+        self,
+        symbol: str = None,
+        settleCoin: str = None,
+    ):
+        """
+        Parameters
+        ----------
+        symbol : str
+        """
+
+        position_info = self.get_position_info(symbol=symbol, settleCoin=settleCoin)
+
+        order_type = "Market"
+
+        asset_size_0 = float(position_info[0]["size"])
+        # Return buy or sale based on pos side (if in a short, side == sell)
+        if asset_size_0 > 0:
+            position_mode = int(position_info[0]["positionIdx"])
+            buy_sell = "Sell" if position_mode == 1 else "Buy"
+            self.create_order(
+                symbol=symbol,
+                order_type=order_type,
+                asset_size=asset_size_0,
+                buy_sell=buy_sell,
+                position_mode=position_mode,
+            )
+
+        asset_size_1 = float(position_info[1]["size"])
+        if asset_size_1 > 0:
+            position_mode = int(position_info[1]["positionIdx"])
+            buy_sell = "Buy" if position_mode == 2 else "Sell"
+            self.create_order(
+                symbol=symbol,
+                order_type=order_type,
+                asset_size=asset_size_1,
+                buy_sell=buy_sell,
+                position_mode=position_mode,
+            )
+
+        self.cancel_all_open_orders_per_symbol(symbol=symbol)
+
+        sleep(1)
+
+        open_order_list = self.get_open_orders(symbol=symbol)
+
+        position_info = self.get_position_info(symbol=symbol)
+
+        asset_size_0 = float(position_info[0]["size"])
+        asset_size_1 = float(position_info[1]["size"])
+
+        if open_order_list or asset_size_0 > 0 or asset_size_1 > 0:
+            return False
+        else:
+            return True
```

### Comparing `quantfreedom-0.1.4.6/quantfreedom/exchanges/bybit_exchange/bybit_live_mode.py` & `quantfreedom-0.2.0.0/quantfreedom/backtesters/bt_regular.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,571 +1,662 @@
-import os
+from typing import Optional
 import numpy as np
-import plotly.graph_objects as go
 import pandas as pd
-
-from time import sleep
-from datetime import datetime, timedelta
 from logging import getLogger
-
-from quantfreedom.email_sender import EmailSender
-from quantfreedom.exchanges.exchange import Exchange
+from multiprocessing import Pool
+from multiprocessing.pool import ApplyResult
+from quantfreedom.helpers.custom_logger import set_loggers
+from quantfreedom.helpers.helper_funcs import get_qf_score, order_records_to_df, make_bt_df
 from quantfreedom.order_handler.order import OrderHandler
-from quantfreedom.strategies.strategy import Strategy
-from quantfreedom.enums import (
-    CandleBodyType,
+from quantfreedom.core.plotting_base import plot_or_results
+from quantfreedom.core.strategy import Strategy
+from quantfreedom.core.enums import (
+    CurrentFootprintCandleTuple,
+    DecreasePosition,
+    FootprintCandlesTuple,
     OrderStatus,
-    PositionModeType,
     RejectedOrder,
+    or_dt,
 )
+from quantfreedom.helpers.utils import pretty_qf
 
-logger = getLogger("info")
-trade_logger = getLogger("trades")
+logger = getLogger()
 
 
-class BybitLiveMode:
-    def __init__(
-        self,
-        email_sender: EmailSender,
-        entry_order_type: str,
-        exchange: Exchange,
-        order: OrderHandler,
-        strategy: Strategy,
-        symbol: str,
-        trading_with: str,
-        tp_order_type: str,
-    ):
-        self.order = order
-        self.exchange = exchange
-        self.email_sender = email_sender
-        self.symbol = symbol
-        self.strategy = strategy
-        self.trading_with = trading_with
-
-        if self.exchange.position_mode == PositionModeType.HedgeMode:
-            if strategy.long_short == "long":
-                self.place_sl_order = exchange.create_long_hedge_mode_sl_order
-                self.get_position_info = exchange.get_long_hedge_mode_position_info
-                if entry_order_type == "market":
-                    self.entry_order = exchange.create_long_hedge_mode_entry_market_order
-
-                if tp_order_type == "limit":
-                    self.place_tp_order = exchange.create_long_hedge_mode_tp_limit_order
-
-        self.ex_position_size_asset = float(self.get_position_info(symbol=symbol).get("size"))
-        self.order.equity = exchange.get_equity_of_asset(trading_with=trading_with)
-
-    def run(
-        self,
-        candles_to_dl: int,
-        timeframe: str,
-    ):
-        latest_pnl = 0
-
-        logger.info(f"Starting live trading")
-        print(f"Starting live trading")
-        try:
-            self.last_pnl = self.exchange.get_latest_pnl_result(symbol=self.symbol)
-        except Exception as e:
-            logger.error(f"get_latest_pnl_result {e}")
-            pass
-        entry_order_id = 0
-        tp_order_id = 0
-        sl_order_id = 0
-
-        self.exchange.last_fetched_ms_time = int(
-            self.exchange.get_candles(
-                symbol=self.symbol,
-                timeframe=timeframe,
-            )[-1, CandleBodyType.Timestamp]
+def run_df_backtest(
+    candles: FootprintCandlesTuple,
+    strategy: Strategy,
+    threads: int,
+    step_by: int = 1,
+) -> pd.DataFrame:
+    global strategy_result_records
+
+    logger.disabled = True
+    # logger.disabled = False
+    # set_loggers(log_folder=strategy.log_folder)
+
+    starting_equity = strategy.static_os_tuple.starting_equity
+
+    order = OrderHandler(
+        long_short=strategy.long_short,
+        static_os_tuple=strategy.static_os_tuple,
+        exchange_settings_tuple=strategy.exchange_settings_tuple,
+    )
+
+    # Creating Settings Vars
+    total_bars = candles.candle_open_timestamps.size
+    step_by_settings = strategy.total_filtered_settings // step_by
+    chunk_process = step_by_settings // threads
+
+    print("Starting the backtest now ... and also here are some stats for your backtest.")
+
+    print("\n" + f"Total threads to use: {threads:,}")
+    print(f"Total indicator settings to test: {strategy.total_indicator_settings:,}")
+    print(f"Total order settings to test: {strategy.total_order_settings:,}")
+    print(f"Total settings combinations to test: {strategy.total_order_settings * strategy.total_indicator_settings:,}")
+    print(f"Total settings combination to test after filtering: {strategy.total_filtered_settings:,}")
+    print(f"Total settings combination with step by: {step_by_settings:,}")
+    print(f"Total settings combination to process per chunk: {chunk_process:,}")
+
+    total_candles = strategy.total_filtered_settings * total_bars
+    chunks = total_candles // threads
+    candle_chunks = chunks // step_by
+    print("\n" + f"Total candles: {total_bars:,}")
+    print(f"Total candles to test: {total_candles:,}")
+    print(f"Total candle chunks to be processed at the same time: {chunks:,}")
+    print(f"Total candle chunks with step by: {candle_chunks:,}")
+
+    num_array_columns = 9 + len(strategy.og_dos_tuple._fields) + len(strategy.og_ind_set_tuple._fields)
+    arr_shape = (strategy.total_filtered_settings, num_array_columns)
+    strategy_result_records = np.full(arr_shape, np.nan)
+
+    range_multiplier = strategy.total_filtered_settings / threads
+    p = Pool()
+    results = []
+    for thread in range(threads):
+        range_start = int(thread * range_multiplier)
+        range_end = int((thread + 1) * range_multiplier)
+        rec_arr_shape = (range_end - range_start, num_array_columns)
+        record_results = np.full(rec_arr_shape, np.nan)
+
+        r: ApplyResult = p.apply_async(
+            func=multiprocess_backtest,
+            args=[
+                candles,
+                order,
+                range_end,
+                range_start,
+                record_results,
+                starting_equity,
+                strategy,
+                total_bars,
+                step_by,
+            ],
+            callback=proc_results,
+            error_callback=handler,
         )
-        logger.info(f"Last Candle time {self.exchange.last_fetched_time_to_pd_datetime()}")
+        results.append(r)
 
-        sleep(self.get_sleep_time_to_next_bar())
+    print("\n" + "looping through results")
+    for r in results:
+        r.wait()
+
+    p.close()
+    p.join()
+    print("creating datafram")
+
+    backtest_df = make_bt_df(
+        strategy=strategy,
+        strategy_result_records=strategy_result_records,
+    )
+
+    return backtest_df
+
+
+def multiprocess_backtest(
+    candles: FootprintCandlesTuple,
+    order: OrderHandler,
+    range_end: int,
+    range_start: int,
+    record_results: np.ndarray,
+    starting_equity: float,
+    strategy: Strategy,
+    total_bars: int,
+    step_by: int,
+):
+    logger.disabled = True
+    rec_idx = 0
+    for set_idx in range(range_start, range_end, step_by):
+        logger.debug(set_idx)
 
-        while True:
-            try:
-                logger.info("Getting Candles")
-                print("Getting Candles")
-                self.candles = self.exchange.get_candles(
-                    symbol=self.symbol,
-                    timeframe=timeframe,
-                    candles_to_dl=candles_to_dl,
-                )
-                num_candles = self.candles.shape[0]
-                print("got candles")
-
-                # bar_index bar index is always the last bar ... so if we have 200 candles we are at index 199
-                bar_index = num_candles - 1
-                msg = "Couldn't verify that the following orders were placed "
+        strategy.set_cur_ind_tuple(
+            set_idx=set_idx,
+        )
+
+        strategy.set_cur_dos_tuple(
+            set_idx=set_idx,
+        )
+
+        strategy.set_entries_exits_array(
+            candles=candles,
+        )
+
+        pnl_array = np.full(shape=round(total_bars / 3), fill_value=np.nan)
+        filled_pnl_counter = 0
+        total_fees_paid = 0
 
-                logger.debug("Setting indicator")
+        order.update_class_dos(
+            dynamic_order_settings=strategy.cur_dos_tuple,
+        )
+        order.set_order_variables(
+            equity=starting_equity,
+        )
+
+        logger.debug("Set order variables, class dos and pnl array")
+
+        starting_bar = strategy.static_os_tuple.starting_bar - 1
+
+        for bar_index in range(starting_bar, total_bars):
+            logger.debug("\n\n")
+            logger.debug(
+                f"set_idx= {strategy.cur_dos_tuple.settings_index} loop_idx = {set_idx} bar_idx= {bar_index} datetime= {candles.candle_open_datetimes[bar_index]}"
+            )
+
+            if order.position_size_usd > 0:
                 try:
-                    latest_pnl = self.exchange.get_latest_pnl_result(symbol=self.symbol)
+                    current_candle = CurrentFootprintCandleTuple(
+                        open_price=candles.candle_open_prices[bar_index],
+                        high_price=candles.candle_high_prices[bar_index],
+                        low_price=candles.candle_low_prices[bar_index],
+                        close_price=candles.candle_close_prices[bar_index],
+                    )
+                    logger.debug("Checking stop loss hit")
+                    order.check_stop_loss_hit(
+                        current_candle=current_candle,
+                    )
+                    logger.debug("Checking liq hit")
+                    order.check_liq_hit(
+                        current_candle=current_candle,
+                    )
+                    logger.debug("Checking take profit hit")
+                    order.check_take_profit_hit(
+                        current_candle=current_candle,
+                        exit_price=strategy.exit_prices[bar_index],
+                    )
+
+                    logger.debug("Checking to move stop to break even")
+                    sl_to_be_price, sl_to_be_pct = order.check_move_sl_to_be(
+                        current_candle=current_candle,
+                    )
+                    if sl_to_be_price:
+                        order.sl_pct = sl_to_be_pct
+                        order.sl_price = sl_to_be_price
+
+                    logger.debug("Checking to move trailing stop loss")
+                    tsl_price, tsl_pct = order.check_move_tsl(
+                        current_candle=current_candle,
+                    )
+                    if tsl_price:
+                        order.sl_pct = tsl_pct
+                        order.sl_price = tsl_price
+
+                except DecreasePosition as e:
+                    (
+                        equity,
+                        fees_paid,
+                        realized_pnl,
+                    ) = order.calculate_decrease_position(
+                        cur_datetime=candles.candle_open_datetimes[bar_index],
+                        exit_fee_pct=e.exit_fee_pct,
+                        exit_price=e.exit_price,
+                        order_status=e.order_status,
+                        market_fee_pct=strategy.exchange_settings_tuple.market_fee_pct,
+                        equity=order.equity,
+                    )
+
+                    pnl_array[filled_pnl_counter] = realized_pnl
+                    filled_pnl_counter += 1
+                    total_fees_paid += fees_paid
+                    logger.debug("Filled pnl array and updated total fees paid")
+
+                    order.set_order_variables(equity=equity)
+                    logger.debug("reset order variables")
+
                 except Exception as e:
-                    logger.error(f"get_latest_pnl_result {e}")
-                logger.info("Evaluating Strat")
-                if self.strategy.live_evaluate(candles=self.candles):
-                    try:
-                        logger.debug("Setting ex postion size usd")
-                        self.__set_ex_position_size_usd()
-                        if self.ex_position_size_usd > 0:
-                            logger.debug("We are in a position updating order info")
-                            self.order.position_size_usd = self.ex_position_size_usd
-                            self.__set_order_average_entry()
-                        else:
-                            logger.debug("we are not in a position updating order info")
-                            self.order.position_size_usd = 0.0
-                            self.order.position_size_asset = 0.0
-                            self.order.average_entry = 0.0
-                            self.order.equity = self.exchange.get_equity_of_asset(trading_with=self.trading_with)
-                            self.order.available_balance = self.order.equity
-                            self.order.total_possible_loss = 0.0
-                            self.order.cash_used = 0.0
-                            self.order.cach_borrowed = 0.0
-
-                        logger.debug("calculate_stop_loss")
-                        sl_price = self.order.calculate_stop_loss(
-                            bar_index=bar_index,
-                            candles=self.candles,
-                        )
+                    logger.error(f"Exception checking sl liq tp and move -> {e}")
+                    raise Exception(f"Exception checking sl liq tp  and move -> {e}")
+            else:
+                logger.debug("Not in a pos so not checking SL Liq or TP")
+
+            logger.debug("strategy evaluate")
+            if strategy.entries[bar_index]:
+                strategy.entry_message(bar_index=bar_index)
+                try:
+                    logger.debug("calculate_stop_loss")
+                    sl_price = order.calculate_stop_loss(
+                        bar_index=bar_index,
+                        candles=candles,
+                    )
+
+                    logger.debug("calculate_increase_position")
+                    (
+                        average_entry,
+                        entry_price,
+                        entry_size_asset,
+                        entry_size_usd,
+                        position_size_asset,
+                        position_size_usd,
+                        total_possible_loss,
+                        total_trades,
+                        sl_pct,
+                    ) = order.calculate_increase_position(
+                        average_entry=order.average_entry,
+                        entry_price=candles.candle_close_prices[bar_index],
+                        equity=order.equity,
+                        position_size_asset=order.position_size_asset,
+                        position_size_usd=order.position_size_usd,
+                        sl_price=sl_price,
+                        total_trades=order.total_trades,
+                    )
+
+                    logger.debug("calculate_leverage")
+                    (
+                        available_balance,
+                        cash_borrowed,
+                        cash_used,
+                        leverage,
+                        liq_price,
+                    ) = order.calculate_leverage(
+                        available_balance=order.available_balance,
+                        average_entry=average_entry,
+                        cash_borrowed=order.cash_borrowed,
+                        cash_used=order.cash_used,
+                        position_size_asset=position_size_asset,
+                        position_size_usd=position_size_usd,
+                        sl_price=sl_price,
+                    )
+
+                    logger.debug("calculate_take_profit")
+                    (
+                        can_move_sl_to_be,
+                        tp_price,
+                        tp_pct,
+                    ) = order.calculate_take_profit(
+                        average_entry=average_entry,
+                        position_size_usd=position_size_usd,
+                        total_possible_loss=total_possible_loss,
+                    )
+                    logger.debug("filling order result")
+                    order.fill_order_result(
+                        available_balance=available_balance,
+                        average_entry=average_entry,
+                        can_move_sl_to_be=can_move_sl_to_be,
+                        cash_borrowed=cash_borrowed,
+                        cash_used=cash_used,
+                        entry_price=entry_price,
+                        entry_size_asset=entry_size_asset,
+                        entry_size_usd=entry_size_usd,
+                        equity=order.equity,
+                        exit_price=np.nan,
+                        fees_paid=np.nan,
+                        leverage=leverage,
+                        liq_price=liq_price,
+                        order_status=OrderStatus.EntryFilled,
+                        position_size_asset=position_size_asset,
+                        position_size_usd=position_size_usd,
+                        total_possible_loss=total_possible_loss,
+                        realized_pnl=np.nan,
+                        sl_pct=sl_pct,
+                        sl_price=sl_price,
+                        total_trades=total_trades,
+                        tp_pct=tp_pct,
+                        tp_price=tp_price,
+                    )
+                    logger.debug("We are in a position and filled the result")
+                except RejectedOrder:
+                    pass
+                except Exception as e:
+                    logger.error(f"Exception hit in eval strat -> {e}")
+                    raise Exception(f"Exception hit in eval strat -> {e}")
 
-                        logger.debug("calculate_increase_position")
-                        (
-                            average_entry,
-                            entry_price,
-                            entry_size_asset,
-                            entry_size_usd,
-                            position_size_asset,
-                            position_size_usd,
-                            total_possible_loss,
-                            total_trades,
-                            sl_pct,
-                        ) = self.order.calculate_increase_position(
-                            average_entry=self.order.average_entry,
-                            entry_price=self.candles[bar_index, CandleBodyType.Close],
-                            equity=self.order.equity,
-                            position_size_asset=self.order.position_size_asset,
-                            position_size_usd=self.order.position_size_usd,
-                            total_possible_loss=self.order.total_possible_loss,
-                            sl_price=sl_price,
-                            total_trades=self.order.total_trades,
-                        )
+        # Checking if gains
+        gains_pct = round(((order.equity - starting_equity) / starting_equity) * 100, 2)
+        wins_and_losses_array = pnl_array[~np.isnan(pnl_array)]
+        total_trades_closed = wins_and_losses_array.size
+        logger.debug(
+            f"""
+Results from backtest
+set_idx={strategy.cur_dos_tuple.settings_index}
+loop_idx = {set_idx}
+Starting eq={starting_equity}
+Ending eq={order.equity}
+Gains pct={gains_pct}
+total_trades={total_trades_closed}"""
+        )
+        if total_trades_closed > 0 and gains_pct > strategy.backtest_settings_tuple.gains_pct_filter:
+            if wins_and_losses_array.size > strategy.backtest_settings_tuple.total_trade_filter:
+                wins_and_losses_array_no_be = wins_and_losses_array[
+                    (wins_and_losses_array < -0.009) | (wins_and_losses_array > 0.009)
+                ]
+                qf_score = get_qf_score(
+                    gains_pct=gains_pct,
+                    wins_and_losses_array_no_be=wins_and_losses_array_no_be,
+                )
 
-                        logger.debug("calculate_leverage")
-                        (
-                            available_balance,
-                            cash_borrowed,
-                            cash_used,
-                            leverage,
-                            liq_price,
-                        ) = self.order.calculate_leverage(
-                            available_balance=self.order.available_balance,
-                            average_entry=average_entry,
-                            cash_borrowed=self.order.cash_borrowed,
-                            cash_used=self.order.cash_used,
-                            position_size_usd=position_size_usd,
-                            position_size_asset=position_size_asset,
-                            sl_price=sl_price,
-                        )
+                # Checking to the upside filter
+                if qf_score > strategy.backtest_settings_tuple.qf_filter:
+                    win_loss = np.where(wins_and_losses_array_no_be < 0, 0, 1)
+                    wins = np.count_nonzero(win_loss)
+                    losses = win_loss.size - wins
+                    win_rate = round(wins / win_loss.size * 100, 2)
 
-                        logger.debug("calculate_take_profit")
+                    total_pnl = wins_and_losses_array.sum()
+                    tuple_results = (
                         (
-                            can_move_sl_to_be,
-                            tp_price,
-                            tp_pct,
-                        ) = self.order.calculate_take_profit(
-                            average_entry=average_entry,
-                            position_size_usd=position_size_usd,
-                            total_possible_loss=total_possible_loss,
+                            wins_and_losses_array.size,
+                            wins,
+                            losses,
+                            gains_pct,
+                            win_rate,
+                            qf_score,
+                            round(total_fees_paid, 2),
+                            total_pnl,
+                            order.equity,
                         )
-                        logger.debug("filling order result")
-                        self.order.fill_order_result(
-                            available_balance=available_balance,
-                            average_entry=average_entry,
-                            can_move_sl_to_be=can_move_sl_to_be,
-                            cash_borrowed=cash_borrowed,
-                            cash_used=cash_used,
-                            entry_price=entry_price,
-                            entry_size_asset=entry_size_asset,
-                            entry_size_usd=entry_size_usd,
-                            equity=self.order.equity,
-                            exit_price=np.nan,
-                            fees_paid=np.nan,
-                            leverage=leverage,
-                            liq_price=liq_price,
-                            order_status=OrderStatus.EntryFilled,
-                            position_size_asset=position_size_asset,
-                            position_size_usd=position_size_usd,
-                            total_possible_loss=total_possible_loss,
-                            realized_pnl=np.nan,
-                            sl_pct=sl_pct,
-                            sl_price=sl_price,
-                            total_trades=total_trades,
-                            tp_pct=tp_pct,
-                            tp_price=tp_price,
-                        )
-                        logger.info("We are in a position and filled the result")
+                        + strategy.cur_dos_tuple
+                        + strategy.cur_ind_set_tuple
+                    )
+                    record_results[rec_idx] = tuple_results
+                    rec_idx += 1
+        logger.debug(
+            f"Starting New Loop\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n"
+        )
+    return range_start, range_end, record_results
 
-                        # place the order
-                        send_verify_error = False
-                        logger.info("Placing Entry Order")
-                        entry_order_id = self.entry_order(
-                            asset_size=self.order.entry_size_asset,
-                            symbol=self.symbol,
-                        )
 
-                        logger.info(f"Submitted entry order -> [order_id={entry_order_id}]")
-                        sleep(1)
+def proc_results(
+    results: tuple,
+):
+    start = results[0]
+    end = results[1]
+    arr = results[2]
+    strategy_result_records[start:end] = arr
+
+
+def handler(error):
+    print(f"Error: {error}", flush=True)
+
+
+def or_backtest(
+    candles: FootprintCandlesTuple,
+    disable_logger: bool,
+    disable_plot: bool,
+    strategy: Strategy,
+    set_idx: int,
+    logger_level: str = "INFO",
+):
+    if disable_logger:
+        set_loggers(
+            disable_logger=disable_logger,
+        )
+    else:
+        set_loggers(
+            disable_logger=disable_logger,
+            log_path=strategy.log_folder,
+            logger_level=logger_level,
+        )
 
-                        # check if order fileld
-                        logger.debug(f"Checking if entry order was filled")
-                        if self.exchange.check_if_order_filled(
-                            order_id=entry_order_id,
-                            symbol=self.symbol,
-                        ):
-                            logger.info("Entry was filled")
-                        else:
-                            msg += f"entry_order_id {entry_order_id} "
-                            send_verify_error = True
-                            logger.warning(f"Couldn't verify entry order was filled {entry_order_id}")
-
-                        # cancel other orders if in position
-                        logger.info(f"checking if in position to cancel tp and sl")
-                        self.__set_ex_position_size_asset()
-                        if self.ex_position_size_asset > 0:
-                            logger.info(f"We are in a pos and trying to cancel tp and sl")
-                            if self.exchange.cancel_all_open_orders_per_symbol(symbol=self.symbol):
-                                logger.info(f"Canceled the orders")
-                            else:
-                                logger.warning("Wasn't able to verify that the tp and sl were canceled")
-
-                        sleep(1)
-
-                        # set the levergae
-                        logger.info("Setting leverage")
-                        if self.exchange.set_leverage(
-                            symbol=self.symbol,
-                            leverage=self.order.leverage,
-                        ):
-                            logger.info(f"Leverage Changed")
-                        else:
-                            logger.warning("Couldn't verify that leverage was set")
-                            msg += f"leverage was set "
-                            send_verify_error = True
-
-                        logger.info(f"Submitting stop loss order")
-                        sl_order_id = self.place_sl_order(
-                            asset_size=self.ex_position_size_asset,
-                            symbol=self.symbol,
-                            trigger_price=self.order.sl_price,
-                        )
-                        logger.info(f"Submitted SL order -> [order_id={sl_order_id}]")
+    starting_equity = strategy.static_os_tuple.starting_equity
+
+    order = OrderHandler(
+        exchange_settings_tuple=strategy.exchange_settings_tuple,
+        long_short=strategy.long_short,
+        static_os_tuple=strategy.static_os_tuple,
+    )
+
+    set_idx = strategy.get_settings_index(set_idx=set_idx)
+
+    strategy.set_cur_ind_tuple(
+        set_idx=set_idx,
+    )
+
+    strategy.set_entries_exits_array(
+        candles=candles,
+    )
+
+    strategy.set_cur_dos_tuple(
+        set_idx=set_idx,
+    )
+
+    order.update_class_dos(
+        dynamic_order_settings=strategy.cur_dos_tuple,
+    )
+    order.set_order_variables(
+        equity=starting_equity,
+    )
+
+    total_bars = candles.candle_open_timestamps.size
+
+    or_filled = 0
+    order_records = np.empty(shape=int(total_bars / 3), dtype=or_dt)
+
+    for bar_index in range(strategy.static_os_tuple.starting_bar - 1, total_bars):
+        logger.debug("\n\n")
+        datetime = candles.candle_open_datetimes[bar_index]
+        logger.debug(f"set_idx= {set_idx} bar_idx= {bar_index} datetime= {datetime}")
+
+        if order.position_size_usd > 0:
+            try:
+                current_candle = CurrentFootprintCandleTuple(
+                    open_timestamp=candles.candle_open_timestamps[bar_index],
+                    open_price=candles.candle_open_prices[bar_index],
+                    high_price=candles.candle_high_prices[bar_index],
+                    low_price=candles.candle_low_prices[bar_index],
+                    close_price=candles.candle_close_prices[bar_index],
+                )
+                logger.debug("Checking stop loss hit")
+                order.check_stop_loss_hit(
+                    current_candle=current_candle,
+                )
+                logger.debug("Checking liq hit")
+                order.check_liq_hit(
+                    current_candle=current_candle,
+                )
+                logger.debug("Checking take profit hit")
+                order.check_take_profit_hit(
+                    current_candle=current_candle,
+                    exit_price=strategy.exit_prices[bar_index],
+                )
+
+                logger.debug("Checking to move stop to break even")
+                sl_to_be_price, sl_to_be_pct = order.check_move_sl_to_be(
+                    current_candle=current_candle,
+                )
+                if sl_to_be_price:
+                    order.sl_pct = sl_to_be_pct
+                    order.sl_price = sl_to_be_price
+                    logger.debug(f"Filling order for move sl to be")
+                    order.fill_or_exit_move(
+                        bar_index=bar_index,
+                        set_idx=set_idx,
+                        order_records=order_records[or_filled],
+                        order_status=OrderStatus.MovedSLToBE,
+                        timestamp=current_candle.open_timestamp,
+                        sl_price=sl_to_be_price,
+                        sl_pct=sl_to_be_pct,
+                    )
+                    or_filled += 1
+                    logger.debug(f"Filled sl to be order records")
+
+                logger.debug("Checking to move trailing stop loss")
+                tsl_price, tsl_pct = order.check_move_tsl(
+                    current_candle=current_candle,
+                )
+                if tsl_price:
+                    order.sl_pct = tsl_pct
+                    order.sl_price = tsl_price
+                    logger.debug(f"Filling order for tsl")
+
+                    order.fill_or_exit_move(
+                        bar_index=bar_index,
+                        set_idx=set_idx,
+                        order_records=order_records[or_filled],
+                        order_status=OrderStatus.MovedTSL,
+                        timestamp=current_candle.open_timestamp,
+                        sl_pct=tsl_pct,
+                        sl_price=tsl_price,
+                    )
+                    or_filled += 1
+                    logger.debug(f"Filled move tsl order records")
+
+            except DecreasePosition as e:
+                (
+                    equity,
+                    fees_paid,
+                    realized_pnl,
+                ) = order.calculate_decrease_position(
+                    cur_datetime=candles.candle_open_datetimes[bar_index],
+                    exit_fee_pct=e.exit_fee_pct,
+                    exit_price=e.exit_price,
+                    order_status=e.order_status,
+                    market_fee_pct=strategy.exchange_settings_tuple.market_fee_pct,
+                    equity=order.equity,
+                )
+                logger.debug(f"Filling or for decrease postiion {OrderStatus._fields[e.order_status]}")
+                order.fill_or_exit_move(
+                    bar_index=bar_index,
+                    set_idx=set_idx,
+                    order_records=order_records[or_filled],
+                    order_status=e.order_status,
+                    timestamp=current_candle.open_timestamp,
+                    equity=equity,
+                    exit_price=e.exit_price,
+                    fees_paid=fees_paid,
+                    realized_pnl=realized_pnl,
+                )
+                or_filled += 1
+                logger.debug(f"Filled decrease postiion order records for {OrderStatus._fields[e.order_status]}")
+
+                order.set_order_variables(equity=equity)
+                logger.debug("reset order variables")
 
-                        sleep(1)
-                        logger.info(f"Submitting take profit order")
-                        tp_order_id = self.place_tp_order(
-                            asset_size=self.ex_position_size_asset,
-                            symbol=self.symbol,
-                            tp_price=self.order.tp_price,
-                        )
-                        logger.info(f"Submitted TP order -> [order_id={tp_order_id}]")
-                        # sleep 1 second before checking to see if orders were placed
-                        sleep(1)
-                        logger.info(f"Checking if stop loss was placed")
-                        if self.exchange.check_if_order_open(
-                            order_id=sl_order_id,
-                            symbol=self.symbol,
-                        ):
-                            logger.info(f"Stop loss was placed")
-                        else:
-                            logger.warning(f"Couldn't verify sl order was placed {sl_order_id} ")
-                            msg += f"sl_order_id {sl_order_id} "
-                            send_verify_error = True
-
-                        logger.debug(f"Checking if tp was placed")
-                        if self.exchange.check_if_order_open(
-                            order_id=tp_order_id,
-                            symbol=self.symbol,
-                        ):
-                            logger.info(f"take profit placed")
-                        else:
-                            logger.info(f"Couldn't verify tp order was filled {tp_order_id}")
-                            msg += f"tp_order_id {tp_order_id}"
-                            send_verify_error = True
-
-                        if send_verify_error:
-                            logger.info("Something wan't verified so rechecking all")
-                            entry_placed = self.exchange.check_if_order_filled(
-                                symbol=self.symbol,
-                                order_id=entry_order_id,
-                            )
-                            leverage_changed = self.exchange.set_leverage(
-                                leverage=self.order.leverage,
-                                symbol=self.symbol,
-                            )
-                            sl_placed = self.exchange.check_if_order_open(
-                                order_id=sl_order_id,
-                                symbol=self.symbol,
-                            )
-                            tp_placed = self.exchange.check_if_order_open(
-                                order_id=tp_order_id,
-                                symbol=self.symbol,
-                            )
-                            verify_list = [entry_placed, leverage_changed, sl_placed, tp_placed]
-                            if not all(v == True for v in verify_list):
-                                logger.error(msg)
-                                raise Exception(msg)
-                            logger.info("All verified")
-
-                        else:
-                            self.__set_exchange_variables(
-                                entry_order_id=entry_order_id,
-                                sl_order_id=sl_order_id,
-                                tp_order_id=tp_order_id,
-                            )
-                            message = self.__create_entry_successful_message()
-                            print("Placed a new Trade")
-                            # entry_filename = self.__get_entry_plot_filename()
-                            # strategy_filename = self.strategy.get_strategy_plot_filename(candles=self.candles)
-                            # self.email_sender.email_new_order(
-                            #     message=message,
-                            #     entry_filename=entry_filename,
-                            #     strategy_filename=strategy_filename,
-                            # )
-                            logger.info("Entry placed on exchange")
-                            trade_logger.info(f"{message}")
-
-                    except RejectedOrder as e:
-                        pass
-                    except Exception as e:
-                        logger.error(f"Exception Entry -> {e}")
-                        raise Exception(f"Exception Entry -> {e}")
-                    self.__set_ex_position_size_asset()
-                    if self.ex_position_size_asset > 0:
-                        logger.info(f"We are in a position ... checking to move stop loss")
-                        try:
-                            current_candle = self.candles[bar_index, :]
-                            logger.debug("Checking to move stop to break even")
-                            sl_to_be_price, sl_to_be_pct = self.order.check_move_sl_to_be(current_candle=current_candle)
-                            if sl_to_be_price:
-                                if self.exchange.move_stop_order(
-                                    symbol=self.symbol,
-                                    order_id=sl_order_id,
-                                    asset_size=self.ex_position_size_asset,
-                                    new_price=sl_to_be_price,
-                                ):
-                                    logger.info(f"Moved stop loss from {self.order.sl_price} to {sl_to_be_price}")
-                                    self.order.sl_price = sl_to_be_price
-                                    self.order.sl_pct = sl_to_be_pct
-                                else:
-                                    logger.warning(f"Couldn't verify sl to be was moved {sl_order_id}")
-                                    raise Exception(f"Exception Move sl to be -> {e}")
-
-                            logger.debug("Checking to move trailing stop loss")
-                            tsl_price, tsl_pct = self.order.check_move_tsl(current_candle=current_candle)
-                            if tsl_price:
-                                if self.exchange.move_stop_order(
-                                    symbol=self.symbol,
-                                    order_id=sl_order_id,
-                                    asset_size=self.ex_position_size_asset,
-                                    new_price=tsl_price,
-                                ):
-                                    logger.info(f"Moved stop loss from {self.order.sl_price} to {tsl_price}")
-                                    self.order.sl_price = tsl_price
-                                    self.order.sl_price = tsl_pct
-                                else:
-                                    logger.warning(f"Couldn't verify tsl was moved {sl_order_id}")
-                                    raise Exception(f"Exception Move TSL -> {e}")
-
-                        except Exception as e:
-                            logger.error(f"Exception checking MoveStopLoss -> {e}")
-                            raise Exception(f"Exception checking MoveStopLoss -> {e}")
-                elif latest_pnl != self.last_pnl:
-                    print(f"Got a new pnl {latest_pnl}")
-                    logger.info(f"Got a new pnl {latest_pnl}")
-                    # self.email_sender.email_pnl(pnl=latest_pnl)
-                    self.last_pnl = latest_pnl
-                else:
-                    pass
             except Exception as e:
-                logger.error(f"Exception -> {e}")
-                # self.email_sender.email_error_msg(msg=f"Exception -> {e}")
-                raise Exception(f"Exception -> {e}")
-            sleep(self.get_sleep_time_to_next_bar())
-
-    def get_sleep_time_to_next_bar(self):
-        ms_to_next_candle = max(
-            0,
-            (self.exchange.last_fetched_ms_time + self.exchange.timeframe_in_ms * 2)
-            - self.exchange.get_current_time_ms(),
-        )
-        td = str(timedelta(seconds=ms_to_next_candle / 1000)).split(":")
-        logger.info(f"Will sleep for {td[0]} hrs {td[1]} mins and {td[2]} seconds till next bar\n")
-        print(f"Will sleep for {td[0]} hrs {td[1]} mins and {td[2]} seconds till next bar\n")
-
-        return int(ms_to_next_candle / 1000)
-
-    def __set_ex_position_size_asset(self):
-        logger.debug(f"Setting position size asset")
-        self.ex_position_size_asset = float(self.get_position_info(symbol=self.symbol)["size"])
-
-    def __set_ex_position_size_usd(self):
-        logger.debug(f"Setting position size usd")
-        pos_val = self.get_position_info(symbol=self.symbol)["positionValue"]
-        self.ex_position_size_usd = 0 if pos_val == "" else float(pos_val)
-
-    def __set_order_average_entry(self):
-        logger.debug(f"Setting average entry")
-        self.order.average_entry = float(self.get_position_info(symbol=self.symbol)["avgPrice"])
-
-    def __set_ex_total_possible_loss(self):
-        logger.debug(f"setting all exchange vars")
-        coin_size = self.ex_position_size_asset
-        pnl = coin_size * (self.ex_sl_price - self.ex_average_entry)
-        fee_open = coin_size * self.ex_average_entry * self.exchange.exchange_settings.market_fee_pct  # math checked
-        fee_close = coin_size * self.ex_sl_price * self.exchange.exchange_settings.market_fee_pct  # math checked
-        self.fees_paid = fee_open + fee_close  # math checked
-        self.ex_total_possible_loss = round(abs(pnl - self.fees_paid), 3)
-
-    def __set_ex_possible_profit(self):
-        logger.debug(f"setting all exchange vars")
-        coin_size = self.ex_position_size_asset
-        pnl = coin_size * (self.ex_tp_price - self.ex_average_entry)
-        fee_open = coin_size * self.ex_average_entry * self.exchange.exchange_settings.market_fee_pct  # math checked
-        fee_close = coin_size * self.ex_tp_price * self.exchange.exchange_settings.limit_fee_pct  # math checked
-        self.fees_paid = fee_open + fee_close  # math checked
-        self.ex_possible_profit = round(abs(pnl - self.fees_paid), 3)
-
-    def __set_exchange_variables(self, entry_order_id, sl_order_id, tp_order_id):
-        logger.debug(f"setting all exchange vars")
-        pos_info = self.get_position_info(symbol=self.symbol)
-        entry_info = self.exchange.get_filled_order_by_order_id(symbol=self.symbol, order_id=entry_order_id)
-        tp_info = self.exchange.get_open_order_by_order_id(symbol=self.symbol, order_id=tp_order_id)
-        sl_info = self.exchange.get_open_order_by_order_id(symbol=self.symbol, order_id=sl_order_id)
-
-        self.ex_position_size_asset = float(pos_info.get("size"))
-        self.ex_position_size_usd = float(pos_info.get("positionValue"))
-        self.ex_average_entry = float(pos_info.get("avgPrice"))
-        self.avg_entry_slippage = self.__get_pct_difference(self.order.average_entry, self.ex_average_entry)
-        self.ex_entry_price = float(entry_info.get("avgPrice"))
-        self.entry_slippage = self.__get_pct_difference(self.order.entry_price, self.ex_entry_price)
-        self.ex_entry_size_asset = float(entry_info.get("qty"))
-        self.ex_entry_size_usd = float(entry_info.get("cumExecValue"))
-        self.ex_leverage = float(pos_info.get("leverage"))
-        self.ex_liq_price = float(pos_info.get("liqPrice"))
-        self.ex_liq_pct = self.__get_pct_difference(starting_num=self.ex_average_entry, diff_num=self.ex_liq_price)
-        self.ex_tp_price = float(tp_info.get("price"))
-        self.ex_tp_pct = self.__get_pct_difference(starting_num=self.ex_average_entry, diff_num=self.ex_tp_price)
-        self.ex_sl_price = float(sl_info.get("triggerPrice"))
-        self.ex_sl_pct = self.__get_pct_difference(starting_num=self.ex_average_entry, diff_num=self.ex_sl_price)
-        coin_size = self.ex_position_size_asset
-        pnl = coin_size * (self.ex_sl_price - self.ex_average_entry)
-        fee_open = coin_size * self.ex_average_entry * self.exchange.exchange_settings.market_fee_pct  # math checked
-        fee_close = coin_size * self.ex_sl_price * self.exchange.exchange_settings.market_fee_pct  # math checked
-        self.fees_paid = fee_open + fee_close  # math checked
-        self.ex_total_possible_loss = round(-(pnl - self.fees_paid), 3)
-
-    def __get_pct_difference(self, starting_num, diff_num):
-        logger.debug(f"getting pct difference")
-        return round(abs((starting_num - diff_num) / starting_num) * 100, 3)
-
-    def __create_entry_successful_message(self):
-        logger.debug(f"Creating message")
-        self.__set_ex_total_possible_loss()
-        self.__set_ex_possible_profit()
-
-        message = f"An order was placed successfully\
-            \n[ex_candle_closing_price={self.candles[-1,CandleBodyType.Close]}]\
-            \n[entry_price={self.order.entry_price}]\
-            \n[ex_entry_price={self.ex_entry_price}]\
-            \n[Entry slippage={self.entry_slippage}]\
-            \n[average_entry={self.order.average_entry}]\
-            \n[ex_average_entry={self.ex_average_entry}]\
-            \n[Average Entry slippage={self.avg_entry_slippage}]\
-            \n[position_size_usd={self.order.position_size_usd}]\
-            \n[ex_position_size_usd={self.ex_position_size_usd}]\
-            \n[entry_size_usd={self.order.entry_size_usd}]\
-            \n[ex_entry_size_usd={self.ex_entry_size_usd}]\
-            \n[leverage={self.order.leverage}]\
-            \n[ex_leverage={self.ex_leverage}]\
-            \n[liq price={self.order.liq_price}]\
-            \n[ex_liq price={self.ex_liq_price}]\
-            \n[ex_liq_pct={self.ex_liq_pct}]\
-            \n[candle low={self.candles[-1,CandleBodyType.Low]}]\
-            \n[stop_loss_price={self.order.sl_price}]\
-            \n[ex_stop_loss_price={self.ex_sl_price}]\
-            \n[sl_pct={round(self.order.sl_pct * 100, 3)}]\
-            \n[ex_sl_pct={self.ex_sl_pct}]\
-            \n[take_profit_price={self.order.tp_price}]\
-            \n[ex_take_profit_price={self.ex_tp_price}]\
-            \n[tp_pct={round(self.order.tp_pct * 100, 3)}]\
-            \n[ex_tp_pct={self.ex_tp_pct}]\
-            \n[possible loss={self.order.total_possible_loss}]\
-            \n[ex_possible loss={self.ex_total_possible_loss}]\
-            \n[ex_possible profit={self.ex_possible_profit}]"
-        return message
-
-    # def __get_entry_plot_filename(self):
-    #     logger.debug("Getting entry plot file")
-    #     latest_candles = self.candles[-50:]
-    #     latest_candles_datetimes = pd.to_datetime(latest_candles[:, CandleBodyType.Timestamp], unit="ms")
-    #     graph_entry = [latest_candles_datetimes[-1]]
-    #     fig = go.Figure()
-    #     fig.add_candlestick(
-    #         x=latest_candles_datetimes,
-    #         open=latest_candles[:, CandleBodyType.Open],
-    #         high=latest_candles[:, CandleBodyType.High],
-    #         low=latest_candles[:, CandleBodyType.Low],
-    #         close=latest_candles[:, CandleBodyType.Close],
-    #         name="Exchange order",
-    #     )
-    #     # entry
-    #     fig.add_scatter(
-    #         x=graph_entry,
-    #         y=[self.order.entry_price],
-    #         mode="markers",
-    #         marker=dict(size=10, color="LightSeaGreen"),
-    #         name=f"Entry",
-    #     )
-    #     # average entry
-    #     fig.add_scatter(
-    #         x=graph_entry,
-    #         y=[self.ex_average_entry],
-    #         mode="markers",
-    #         marker=dict(size=10, color="purple", symbol="arrow-up"),
-    #         name=f"Average Entry",
-    #     )
-    #     # take profit
-    #     fig.add_scatter(
-    #         x=graph_entry,
-    #         y=[self.ex_tp_price],
-    #         mode="markers",
-    #         marker=dict(size=10, symbol="star", color="Green"),
-    #         name=f"Take Profit",
-    #     )
-    #     # stop loss
-    #     fig.add_scatter(
-    #         x=graph_entry,
-    #         y=[self.ex_sl_price],
-    #         mode="markers",
-    #         marker=dict(size=10, symbol="x", color="orange"),
-    #         name=f"Stop Loss",
-    #     )
-    #     # liq price
-    #     fig.add_scatter(
-    #         x=graph_entry,
-    #         y=[self.ex_liq_price],
-    #         mode="markers",
-    #         marker=dict(size=10, symbol="hexagram", color="red"),
-    #         name=f"Liq Price",
-    #     )
-    #     fig.update_layout(height=800, xaxis_rangeslider_visible=False)
-    #     fig.show()
-    #     entry_filename = os.path.join(
-    #         self.strategy.log_folder,
-    #         "logs",
-    #         "images",
-    #         f'entry_{datetime.utcnow().strftime("%m-%d-%Y_%H-%M-%S")}.png',
-    #     )
-    #     fig.write_image(entry_filename)
-    #     return entry_filename
+                logger.error(f"Exception checking sl liq tp and move -> {e}")
+                raise Exception(f"Exception checking sl liq tp and move -> {e}")
+        else:
+            logger.debug("Not in a pos so not checking SL Liq or TP")
+
+        logger.debug("strategy evaluate")
+        if strategy.entries[bar_index]:
+            strategy.entry_message(bar_index=bar_index)
+            try:
+                logger.debug("calculate_stop_loss")
+                sl_price = order.calculate_stop_loss(
+                    bar_index=bar_index,
+                    candles=candles,
+                )
+
+                logger.debug("calculate_increase_position")
+                (
+                    average_entry,
+                    entry_price,
+                    entry_size_asset,
+                    entry_size_usd,
+                    position_size_asset,
+                    position_size_usd,
+                    total_possible_loss,
+                    total_trades,
+                    sl_pct,
+                ) = order.calculate_increase_position(
+                    average_entry=order.average_entry,
+                    entry_price=candles.candle_close_prices[bar_index],
+                    equity=order.equity,
+                    position_size_asset=order.position_size_asset,
+                    position_size_usd=order.position_size_usd,
+                    sl_price=sl_price,
+                    total_trades=order.total_trades,
+                )
+
+                logger.debug("calculate_leverage")
+                (
+                    available_balance,
+                    cash_borrowed,
+                    cash_used,
+                    leverage,
+                    liq_price,
+                ) = order.calculate_leverage(
+                    available_balance=order.available_balance,
+                    average_entry=average_entry,
+                    cash_borrowed=order.cash_borrowed,
+                    cash_used=order.cash_used,
+                    position_size_usd=position_size_usd,
+                    position_size_asset=position_size_asset,
+                    sl_price=sl_price,
+                )
+
+                logger.debug("calculate_take_profit")
+                (
+                    can_move_sl_to_be,
+                    tp_price,
+                    tp_pct,
+                ) = order.calculate_take_profit(
+                    average_entry=average_entry,
+                    position_size_usd=position_size_usd,
+                    total_possible_loss=total_possible_loss,
+                )
+
+                logger.debug("calculate_take_profit")
+                order.fill_order_result(
+                    available_balance=available_balance,
+                    average_entry=average_entry,
+                    can_move_sl_to_be=can_move_sl_to_be,
+                    cash_borrowed=cash_borrowed,
+                    cash_used=cash_used,
+                    entry_price=entry_price,
+                    entry_size_asset=entry_size_asset,
+                    entry_size_usd=entry_size_usd,
+                    equity=order.equity,
+                    exit_price=np.nan,
+                    fees_paid=np.nan,
+                    leverage=leverage,
+                    liq_price=liq_price,
+                    order_status=OrderStatus.EntryFilled,
+                    position_size_asset=position_size_asset,
+                    position_size_usd=position_size_usd,
+                    total_possible_loss=total_possible_loss,
+                    realized_pnl=np.nan,
+                    sl_pct=sl_pct,
+                    sl_price=sl_price,
+                    total_trades=total_trades,
+                    tp_pct=tp_pct,
+                    tp_price=tp_price,
+                )
+                logger.debug("filling entry order records")
+                order.fill_or_entry(
+                    bar_index=bar_index + 1,
+                    set_idx=set_idx,
+                    order_records=order_records[or_filled],
+                    timestamp=candles.candle_open_timestamps[bar_index + 1],
+                )
+                or_filled += 1
+                logger.info("We are in a position and filled the result")
+            except RejectedOrder:
+                pass
+            except Exception as e:
+                if bar_index + 1 >= candles.candle_open_timestamps.size:
+                    raise Exception(f"Exception hit in eval strat -> {e}")
+                    pass
+                else:
+                    logger.error(f"Exception hit in eval strat -> {e}")
+                    raise Exception(f"Exception hit in eval strat -> {e}")
+    order_records_df = order_records_to_df(order_records[:or_filled])
+    pretty_qf(strategy.cur_dos_tuple)
+    pretty_qf(strategy.cur_ind_set_tuple)
+    if not disable_plot:
+        strategy.plot_signals(
+            candles=candles,
+        )
+        plot_or_results(
+            candles=candles,
+            order_records_df=order_records_df,
+        )
+    return order_records_df
```

### Comparing `quantfreedom-0.1.4.6/quantfreedom/exchanges/exchange.py` & `quantfreedom-0.2.0.0/quantfreedom/exchanges/exchange.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import pandas as pd
 
 from datetime import timedelta
 from time import time
 from datetime import datetime, timezone
 
-from quantfreedom.enums import ExchangeSettings
+from quantfreedom.core.enums import FootprintCandlesTuple
 
 UNIVERSAL_SIDES = ["buy", "sell"]
 UNIVERSAL_TIMEFRAMES = ["1m", "5m", "15m", "30m", "1h", "2h", "4h", "6h", "12h", "d", "w"]
 TIMEFRAMES_IN_MINUTES = [1, 5, 15, 30, 60, 120, 240, 360, 720, 1440, 10080]
 
 
 class Exchange:
@@ -18,15 +18,15 @@
     volume_yes_no_end = None
     position_mode = None
     timeframe_in_ms = None
     last_fetched_ms_time = None
 
     def __init__(
         self,
-        use_test_net: bool,
+        use_testnet: bool,
         api_key: str = None,
         secret_key: str = None,
     ):
         self.api_key = api_key
         self.secret_key = secret_key
 
     def sort_dict(self, data: dict):
@@ -95,20 +95,28 @@
         self,
         candles_to_dl_ms: int,
         since_datetime: datetime,
         timeframe_in_ms: int,
         until_datetime: datetime,
     ) -> tuple[int, int]:
         if until_datetime is None:
+            cur_time = self.get_current_time_ms()
+            until_timestamp = cur_time - (cur_time % timeframe_in_ms) - 5000  # note below
+            # we subtract the remainder of cur time / timeframe in ms to get the most recent timestamp for our timeframe
+            # then we subtract 5 seconds so that if we are doing 5 min we would get 02:05:00 and change it to 02:04:55
+            # this way we don't download the candle for 02:05:00 since it is not closed yet
             if since_datetime is None:
-                until_timestamp = self.get_current_time_ms() - timeframe_in_ms
-                since_timestamp = until_timestamp - candles_to_dl_ms
+                since_timestamp = until_timestamp - candles_to_dl_ms + 5000
+                # add back 5 seconds so we get the candle at 01:00:00 and not 00:59:55
             else:
                 since_timestamp = int(since_datetime.replace(tzinfo=timezone.utc).timestamp() * 1000)
-                until_timestamp = since_timestamp + candles_to_dl_ms - 5000  # 5000 is to sub 5 seconds
+                temp_until = since_timestamp + candles_to_dl_ms - 5000  # 5000 is to sub 5 seconds so we don't get the cur candle
+                if temp_until < until_timestamp:  # if false then we will try to get candles from the future
+                    until_timestamp = temp_until
+
         else:
             until_timestamp = int(until_datetime.replace(tzinfo=timezone.utc).timestamp() * 1000)
             if since_datetime is None:
                 since_timestamp = until_timestamp - candles_to_dl_ms
             else:
                 since_timestamp = int(since_datetime.replace(tzinfo=timezone.utc).timestamp() * 1000)
             until_timestamp -= 5000
@@ -122,18 +130,28 @@
         step_size: str,
     ):
         if "." not in step_size:
             return int(step_size)
         else:
             return step_size.index("1") - step_size.index(".")
 
+    def get_sleep_time_to_next_bar(self):
+        ms_to_next_candle = max(
+            0,
+            (self.last_fetched_ms_time + self.timeframe_in_ms * 2) - self.get_current_time_ms(),
+        )
+        td = str(timedelta(seconds=ms_to_next_candle / 1000)).split(":")
+        print(f"Will sleep for {td[0]} hrs {td[1]} mins and {td[2]} seconds till next bar\n")
+
+        return int(ms_to_next_candle / 1000)
+
     def create_order(self, **kwargs):
         pass
 
-    def get_candles(self, **kwargs):
+    def get_candles(self, **kwargs) -> FootprintCandlesTuple:
         pass
 
     def cancel_open_order(self, **kwargs):
         pass
 
     def get_filled_order_by_order_id(self, **kwargs):
         pass
@@ -143,17 +161,14 @@
 
     def get_open_order_by_order_id(self, **kwargs):
         pass
 
     def cancel_all_open_orders_per_symbol(self, **kwargs):
         pass
 
-    def get_wallet_info_of_asset(self, **kwargs):
-        pass
-
     def check_if_order_filled(self, **kwargs):
         pass
 
     def set_leverage(self, **kwargs):
         pass
 
     def check_if_order_canceled(self, **kwargs):
@@ -185,15 +200,18 @@
 
     def set_init_last_fetched_time(self, **kwargs):
         pass
 
     def get_exchange_timeframe(self, **kwargs):
         pass
 
-    def set_and_get_exchange_settings(self, **kwargs):
+    def set_and_get_exchange_settings_tuple(self, **kwargs):
         pass
 
     def get_no_fees_balance_of_asset_market_in_only(self, **kwargs):
         pass
 
-    def create_long_hedge_mode_entry_market_order_stoploss(self, **kwargs):
+    def create_long_hedge_mode_entry_market_order_with_stoploss(self, **kwargs):
+        pass
+
+    def close_hedge_positions_and_orders(self, **kwargs):
         pass
```

### Comparing `quantfreedom-0.1.4.6/quantfreedom/exchanges/mufex_exchange/mufex.py` & `quantfreedom-0.2.0.0/quantfreedom/exchanges/mufex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,45 @@
+from typing import Optional
 import hmac
 import hashlib
 import inspect
 import numpy as np
 from time import sleep, time
 from requests import get, post
 from datetime import datetime, timezone
 
-from quantfreedom.enums import (
+from quantfreedom.core.enums import (
     ExchangeSettings,
+    FootprintCandlesTuple,
     LeverageModeType,
     PositionModeType,
     TriggerDirectionType,
 )
 from quantfreedom.exchanges.exchange import UNIVERSAL_TIMEFRAMES, Exchange
 
 MUFEX_TIMEFRAMES = [1, 5, 15, 30, 60, 120, 240, 360, 720, "D", "W"]
 
 
 class Mufex(Exchange):
     def __init__(
         # Exchange Vars
         self,
-        use_test_net: bool,
+        use_testnet: bool,
         api_key: str = None,
         secret_key: str = None,
     ):
         """
         main docs page https://www.mufex.finance/apidocs/derivatives/contract/index.html
 
         Make sure you have your position mode set to hedge or else a lot of functions will not work.
         https://www.mufex.finance/apidocs/derivatives/contract/index.html?console#t-dv_switchpositionmode
         """
         self.api_key = api_key
         self.secret_key = secret_key
-        if use_test_net:
+        if use_testnet:
             self.url_start = "https://api.testnet.mufex.finance"
         else:
             self.url_start = "https://api.mufex.finance"
 
     ################################################################
     ################################################################
     ###################                          ###################
@@ -58,15 +60,15 @@
         signature = self.__gen_signature(timestamp=timestamp, params_as_string=params_as_dict_string)
         headers = {
             "MF-ACCESS-API-KEY": self.api_key,
             "MF-ACCESS-SIGN": signature,
             "MF-ACCESS-SIGN-TYPE": "2",
             "MF-ACCESS-TIMESTAMP": timestamp,
             "MF-ACCESS-RECV-WINDOW": "5000",
-            "X-Referer": "A6JVVHCXZ",
+            "X-Referer": "AKF3CWKDT",
             "Content-Type": "application/json",
         }
 
         try:
             response = post(
                 url=self.url_start + end_point,
                 headers=headers,
@@ -127,15 +129,15 @@
         self,
         symbol: str,
         timeframe: str,
         since_datetime: datetime = None,
         until_datetime: datetime = None,
         candles_to_dl: int = 1500,
         category: str = "linear",
-    ) -> np.array:
+    ) -> FootprintCandlesTuple:
         """
         [mufex candle docs](https://www.mufex.finance/apidocs/derivatives/contract/index.html?console#t-dv_querykline)
 
         Parameters
         ----------
         symbol : str
             [Mufex Symbol List](https://www.mufex.finance/apidocs/derivatives/contract/index.html?console#symbol-symbol)
@@ -172,35 +174,49 @@
             "category": category,
             "symbol": symbol,
             "interval": ex_timeframe,
             "start": since_timestamp,
             "end": until_timestamp,
             "limit": 1500,
         }
-        # start_time = self.get_current_time_sec()
+        the_url = self.url_start + end_point
         while params["start"] + self.timeframe_in_ms < until_timestamp:
             try:
-                response: dict = get(url=self.url_start + end_point, params=params).json()
+                response: dict = get(url=the_url, params=params).json()
                 new_candles = response["data"]["list"]
                 last_candle_timestamp = int(new_candles[-1][0])
                 if last_candle_timestamp == params["start"]:
                     print("sleeping .2 seconds")
                     sleep(0.2)
                 else:
                     candles_list.extend(new_candles)
                     # add 2 sec so we don't download the same candle two times
                     params["start"] = last_candle_timestamp + 2000
 
             except Exception as e:
                 raise Exception(f"Mufex get_candles {response.get('message')} - > {e}")
 
         candles = np.array(candles_list, dtype=np.float_)[:, :-1]
+
+        open_timestamps = candles[:, 0].astype(np.int64)
+
+        Footprint_Candles_Tuple = FootprintCandlesTuple(
+            candle_open_datetimes=open_timestamps.astype("datetime64[ms]"),
+            candle_open_timestamps=open_timestamps,
+            candle_durations_seconds=np.full(candles.shape[0], int(self.timeframe_in_ms / 1000)),
+            candle_open_prices=candles[:, 1],
+            candle_high_prices=candles[:, 2],
+            candle_low_prices=candles[:, 3],
+            candle_close_prices=candles[:, 4],
+            candle_asset_volumes=candles[:, 5],
+            candle_usdt_volumes=np.around(a=candles[:, 5] * candles[:, 4], decimals=3),
+        )
         self.last_fetched_ms_time = int(candles[-1, 0])
 
-        return candles
+        return Footprint_Candles_Tuple
 
     def get_closed_pnl(
         self,
         symbol: str,
         limit: int = 200,
         since_datetime: datetime = None,
         until_datetime: datetime = None,
@@ -336,23 +352,23 @@
         self,
         symbol: str,
         buy_sell: str,
         position_mode: PositionModeType,  # type: ignore
         order_type: str,
         asset_size: float,
         time_in_force: str = "GoodTillCancel",
-        price: float = None,
+        price: Optional[float] = None,
         triggerDirection: TriggerDirectionType = None,  # type: ignore
         triggerPrice: str = None,
         triggerBy: str = None,
         tpTriggerBy: str = None,
         slTriggerBy: str = None,
         custom_order_id: str = None,
-        takeProfit: float = None,
-        stopLoss: float = None,
+        takeProfit: Optional[float] = None,
+        stopLoss: Optional[float] = None,
         reduce_only: bool = None,
         closeOnTrigger: bool = None,
     ):
         """
         https://www.mufex.finance/apidocs/derivatives/contract/index.html#t-dv_placeorder
 
         time_in_force:
@@ -486,19 +502,18 @@
         params["symbol"] = symbol
         params["limit"] = limit
         params["orderId"] = order_id
         params["orderLinkId"] = custom_order_id
         params["orderFilter"] = orderFilter
         response: dict = self.__HTTP_get_request(end_point=end_point, params=params)
         try:
-            response["data"]["list"][0]
             data_list = response["data"]["list"]
             return data_list
         except Exception as e:
-            raise Exception(f"Mufex get_open_orders = Data or List is empty {response['message']} -> {e}")
+            raise Exception(f"Mufex get_open_orders = {response['message']} -> {e}")
 
     def get_open_order_by_order_id(
         self,
         symbol: str,
         order_id: str,
     ):
         open_order = self.get_open_orders(symbol=symbol, order_id=order_id)[0]
@@ -567,15 +582,15 @@
         params["settleCoin"] = settleCoin
         response: dict = self.__HTTP_get_request(end_point=end_point, params=params)
         try:
             data_list = response["data"]["list"]
 
             return data_list
         except Exception as e:
-            raise Exception(f"Mufex get_account_position_info = Data or List is empty {response['message']} -> {e}")
+            raise Exception(f"Mufex get_account_position_info = {response['message']} -> {e}")
 
     def cancel_open_order(
         self,
         symbol: str,
         order_id: str = None,
         custom_order_id: str = None,
     ):
@@ -896,15 +911,15 @@
             max_asset_size,
             min_asset_size,
             asset_tick_step,
             price_tick_step,
             leverage_tick_step,
         )
 
-    def set_and_get_exchange_settings(
+    def set_and_get_exchange_settings_tuple(
         self,
         leverage_mode: LeverageModeType,  # type: ignore
         position_mode: PositionModeType,  # type: ignore
         symbol: str,
     ):
         self.position_mode = position_mode
         if position_mode == PositionModeType.HedgeMode:
@@ -994,27 +1009,27 @@
         symbol: str,
     ):
         if float(self.get_position_info(symbol=symbol)[0]["entryPrice"]) > 0:
             return True
         else:
             return False
 
-    def create_long_hedge_mode_entry_market_order_stoploss(
+    def create_long_hedge_mode_entry_market_order_with_stoploss(
         self,
         asset_size: float,
         symbol: str,
         sl_price: float,
     ):
         return self.create_order(
             symbol=symbol,
             position_mode=PositionModeType.BuySide,
             buy_sell="Buy",
             order_type="Market",
             asset_size=asset_size,
-            time_in_force="GTC",
+            time_in_force="GoodTillCancel",
             stopLoss=sl_price,
         )
 
     def create_long_hedge_mode_entry_market_order(
         self,
         asset_size: float,
         symbol: str,
@@ -1045,23 +1060,23 @@
             time_in_force="PostOnly",
         )
 
     def create_long_hedge_mode_sl_order(
         self,
         asset_size: float,
         symbol: str,
-        trigger_price: float,
+        sl_price: float,
     ):
         return self.create_order(
             symbol=symbol,
             position_mode=PositionModeType.BuySide,
             buy_sell="Sell",
             order_type="Market",
             asset_size=asset_size,
-            triggerPrice=trigger_price,
+            triggerPrice=sl_price,
             reduce_only=True,
             triggerDirection=TriggerDirectionType.Fall,
             time_in_force="GoodTillCancel",
         )
 
     def get_long_hedge_mode_position_info(
         self,
@@ -1074,7 +1089,63 @@
         func_list = inspect.getmembers(Mufex, predicate=inspect.isfunction)
         new_list = []
         for func in func_list:
             func_name = func[0]
             if not "_" in func_name[0]:
                 new_list.append(func[0])
         return new_list
+
+    def close_hedge_positions_and_orders(
+        self,
+        symbol: str = None,
+        settleCoin: str = None,
+    ):
+        """
+        Parameters
+        ----------
+        symbol : str
+        """
+
+        position_info = self.get_position_info(symbol=symbol, settleCoin=settleCoin)
+
+        order_type = "Market"
+
+        asset_size_0 = float(position_info[0]["size"])
+        # Return buy or sale based on pos side (if in a short, side == sell)
+        if asset_size_0 > 0:
+            position_mode = int(position_info[0]["positionIdx"])
+            buy_sell = "Sell" if position_mode == 1 else "Buy"
+            self.create_order(
+                symbol=symbol,
+                order_type=order_type,
+                asset_size=asset_size_0,
+                buy_sell=buy_sell,
+                position_mode=position_mode,
+            )
+
+        asset_size_1 = float(position_info[1]["size"])
+        if asset_size_1 > 0:
+            position_mode = int(position_info[1]["positionIdx"])
+            buy_sell = "Buy" if position_mode == 2 else "Sell"
+            self.create_order(
+                symbol=symbol,
+                order_type=order_type,
+                asset_size=asset_size_1,
+                buy_sell=buy_sell,
+                position_mode=position_mode,
+            )
+
+        self.cancel_all_open_orders_per_symbol(symbol=symbol)
+
+        sleep(1)
+
+        open_order_list = self.get_open_orders(symbol=symbol)
+
+        position_info = self.get_position_info(symbol=symbol)
+
+        asset_size_0 = float(position_info[0]["size"])
+        asset_size_1 = float(position_info[1]["size"])
+
+        if open_order_list or asset_size_0 > 0 or asset_size_1 > 0:
+            return False
+        else:
+            return True
```

### Comparing `quantfreedom-0.1.4.6/quantfreedom/helper_funcs.py` & `quantfreedom-0.2.0.0/quantfreedom/backtesters/bt_live.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,280 +1,300 @@
-from typing import NamedTuple
 import numpy as np
-import pandas as pd
 from logging import getLogger
-from datetime import datetime
-from quantfreedom.enums import AccountState, DynamicOrderSettings, DynamicOrderSettingsArrays, OrderResult
-from quantfreedom.exchanges.apex_exchange.apex import Apex
-from quantfreedom.exchanges.binance_exchange.binance_us import BinanceUS
-from quantfreedom.exchanges.binance_exchange.binance_usdm import BinanceUSDM
-from quantfreedom.exchanges.bybit_exchange.bybit import Bybit
-from quantfreedom.exchanges.mufex_exchange.mufex import Mufex
-
-logger = getLogger("info")
-
-
-def dl_ex_candles(
-    symbol: str,
-    exchange: str,
-    timeframe: str,
-    since_datetime: datetime = None,
-    until_datetime: datetime = None,
-    candles_to_dl: int = None,
+from quantfreedom.helpers.custom_logger import set_loggers
+from quantfreedom.helpers.helper_funcs import order_records_to_df
+from quantfreedom.order_handler.order import OrderHandler
+from quantfreedom.core.plotting_base import plot_or_results
+from quantfreedom.core.strategy import Strategy
+from quantfreedom.core.enums import (
+    CurrentFootprintCandleTuple,
+    DecreasePosition,
+    FootprintCandlesTuple,
+    OrderStatus,
+    RejectedOrder,
+    or_dt,
+)
+from quantfreedom.helpers.utils import pretty_qf
+
+logger = getLogger()
+
+
+def live_backtest(
+    candles: FootprintCandlesTuple,
+    disable_logger: bool,
+    disable_plot: bool,
+    strategy: Strategy,
+    set_idx: int,
+    logger_level: str = "INFO",
 ):
-    """
-    Download candles from the exchange of your choice
-
-    Parameters
-    ----------
-    exchange: str
-        binance us = 'binance_us' | default candles to dl is 1500
-
-        binance futures = 'binance_usdm' | default candles to dl is 1500
-
-        apex = 'apex' | default candles to dl is 200
-
-        mufex = 'mufex' | default candles to dl is 1500
-
-        bybit = 'bybit' | default candles to dl is 1000
-    symbol : str
-        Check the api of the exchange or get all the symbols of the exchange to see which ones you need to put here
-    timeframe : str
-            "1m", "5m", "15m", "30m", "1h", "2h", "4h", "6h", "12h", "d", "w"
-    since_datetime : datetime
-        The start date, in datetime format, of candles you want to download. EX: datetime(year, month, day, hour, minute)
-    until_datetime : datetime
-        The until date, in datetime format, of candles you want to download minus one candle so if you are on the 5 min if you say your until date is 1200 your last candle will be 1155. EX: datetime(year, month, day, hour, minute)
-    candles_to_dl : int
-        The amount of candles you want to download
-
-    Returns
-    -------
-    np.array
-        a 2 dim array with the following columns "timestamp", "open", "high", "low", "close", "volume"
-    """
-    if exchange.lower() == "binance_usdm":
-        return BinanceUSDM(use_test_net=False).get_candles(
-            symbol=symbol,
-            timeframe=timeframe,
-            since_datetime=since_datetime,
-            until_datetime=until_datetime,
-            candles_to_dl=1500 if candles_to_dl is None else candles_to_dl,
-        )
-    elif exchange.lower() == "binance_us":
-        return BinanceUS().get_candles(
-            symbol=symbol,
-            timeframe=timeframe,
-            since_datetime=since_datetime,
-            until_datetime=until_datetime,
-            candles_to_dl=1500 if candles_to_dl is None else candles_to_dl,
-        )
-    elif exchange.lower() == "apex":
-        return Apex(use_test_net=False).get_candles(
-            symbol=symbol,
-            timeframe=timeframe,
-            since_datetime=since_datetime,
-            until_datetime=until_datetime,
-            candles_to_dl=200 if candles_to_dl is None else candles_to_dl,
-        )
-    elif exchange.lower() == "mufex":
-        return Mufex(use_test_net=False).get_candles(
-            symbol=symbol,
-            timeframe=timeframe,
-            since_datetime=since_datetime,
-            until_datetime=until_datetime,
-            candles_to_dl=1500 if candles_to_dl is None else candles_to_dl,
-        )
-    elif exchange.lower() == "bybit":
-        return Bybit(use_test_net=False).get_candles(
-            symbol=symbol,
-            timeframe=timeframe,
-            since_datetime=since_datetime,
-            until_datetime=until_datetime,
-            candles_to_dl=1000 if candles_to_dl is None else candles_to_dl,
+    if disable_logger:
+        set_loggers(
+            disable_logger=disable_logger,
         )
     else:
-        raise Exception("You need to pick an exchange from this list apex, binance_usdm, mufex, binance_us, bybit")
-
-
-def candles_to_df(
-    candles: np.array,
-) -> pd.DataFrame:
-    """
-    Converts your numpy array candles to a pandas dataframe
-
-    Parameters
-    ----------
-    candles : np.array
-        a 2 dim array with the following columns "timestamp", "open", "high", "low", "close", "volume"
-
-    Returns
-    -------
-    pd.DataFrame
-        columns "timestamp", "open", "high", "low", "close", "volume" with an index of pandas datetimes
-    """
-    candles_df = pd.DataFrame(candles, columns=["timestamp", "open", "high", "low", "close", "volume"])
-    candles_df["timestamp"] = candles_df["timestamp"].astype(dtype=np.int64)
-    candles_df.set_index(pd.to_datetime(candles_df["timestamp"], unit="ms"), inplace=True)
-    candles_df.index.rename("datetime", inplace=True)
-    return candles_df
-
-
-def get_qf_score(
-    gains_pct: float,
-    wins_and_losses_array_no_be: np.array,
-):
-    x = np.arange(1, len(wins_and_losses_array_no_be) + 1)
-    y = wins_and_losses_array_no_be.cumsum()
-
-    xm = x.mean()
-    ym = y.mean()
-
-    y_ym = y - ym
-    if (y_ym == 0).all():
-        y_ym = np.array([1.0])
-    y_ym_s = np.power(y_ym, 2)
-
-    x_xm = x - xm
-    if (x_xm == 0).all():
-        x_xm = np.array([1.0])
-    x_xm_s = np.power(x_xm, 2)
-
-    b1 = (x_xm * y_ym).sum() / x_xm_s.sum()
-    b0 = ym - b1 * xm
-
-    y_pred = b0 + b1 * x
-
-    yp_ym = y_pred - ym
-
-    yp_ym_s = np.power(yp_ym, 2)
+        set_loggers(
+            disable_logger=disable_logger,
+            log_path=strategy.log_folder,
+            logger_level=logger_level,
+        )
 
-    qf_score = yp_ym_s.sum() / y_ym_s.sum()
+    starting_equity = strategy.static_os_tuple.starting_equity
 
-    if gains_pct <= 0:
-        qf_score = -(qf_score)
-    return round(qf_score, 3)
+    order = OrderHandler(
+        exchange_settings_tuple=strategy.exchange_settings_tuple,
+        long_short=strategy.long_short,
+        static_os_tuple=strategy.static_os_tuple,
+    )
 
+    set_idx = strategy.get_settings_index(
+        set_idx=set_idx,
+    )
 
-def get_dos(
-    dos_cart_arrays: DynamicOrderSettingsArrays,
-    dos_index: int,
-):
-    return DynamicOrderSettings(
-        max_trades=dos_cart_arrays.max_trades[dos_index],
-        account_pct_risk_per_trade=dos_cart_arrays.account_pct_risk_per_trade[dos_index],
-        risk_reward=dos_cart_arrays.risk_reward[dos_index],
-        sl_based_on_add_pct=dos_cart_arrays.sl_based_on_add_pct[dos_index],
-        sl_based_on_lookback=dos_cart_arrays.sl_based_on_lookback[dos_index],
-        sl_bcb_type=dos_cart_arrays.sl_bcb_type[dos_index],
-        sl_to_be_cb_type=dos_cart_arrays.sl_to_be_cb_type[dos_index],
-        sl_to_be_when_pct=dos_cart_arrays.sl_to_be_when_pct[dos_index],
-        trail_sl_bcb_type=dos_cart_arrays.trail_sl_bcb_type[dos_index],
-        trail_sl_by_pct=dos_cart_arrays.trail_sl_by_pct[dos_index],
-        trail_sl_when_pct=dos_cart_arrays.trail_sl_when_pct[dos_index],
+    strategy.set_cur_ind_tuple(
+        set_idx=set_idx,
+    )
+    strategy.set_entries_exits_array(
+        candles=candles,
     )
+    strategy.set_cur_dos_tuple(set_idx=set_idx)
 
+    order.update_class_dos(dynamic_order_settings=strategy.cur_dos_tuple)
+    order.set_order_variables(equity=starting_equity)
 
-def cart_product(
-    named_tuple: NamedTuple,
-) -> np.array:
-    n = 1
-    for x in named_tuple:
-        n *= x.size
-    out = np.empty((n, len(named_tuple)))
-
-    for i in range(len(named_tuple)):
-        m = int(n / named_tuple[i].size)
-        out[:n, i] = np.repeat(named_tuple[i], m)
-        n //= named_tuple[i].size
-
-    n = named_tuple[-1].size
-    for k in range(len(named_tuple) - 2, -1, -1):
-        n *= named_tuple[k].size
-        m = int(n / named_tuple[k].size)
-        for j in range(1, named_tuple[k].size):
-            out[j * m : (j + 1) * m, k + 1 :] = out[0:m, k + 1 :]
-    return out.T
-
-
-def dos_cart_product(
-    dos_arrays: DynamicOrderSettingsArrays,
-) -> DynamicOrderSettingsArrays:
-    cart_arrays = cart_product(named_tuple=dos_arrays)
-    return DynamicOrderSettingsArrays(
-        max_trades=cart_arrays[0].astype(np.int_),
-        account_pct_risk_per_trade=cart_arrays[1] / 100,
-        risk_reward=cart_arrays[2],
-        sl_based_on_add_pct=cart_arrays[3] / 100,
-        sl_based_on_lookback=cart_arrays[4].astype(np.int_),
-        sl_bcb_type=cart_arrays[5].astype(np.int_),
-        sl_to_be_cb_type=cart_arrays[6].astype(np.int_),
-        sl_to_be_when_pct=cart_arrays[7] / 100,
-        trail_sl_bcb_type=cart_arrays[8].astype(np.int_),
-        trail_sl_by_pct=cart_arrays[9] / 100,
-        trail_sl_when_pct=cart_arrays[10] / 100,
-    )
+    total_bars = candles.candle_open_timestamps.size
 
+    or_filled = 0
+    order_records = np.empty(shape=int(total_bars / 3), dtype=or_dt)
+
+    loop_start = strategy.static_os_tuple.starting_bar - 1
+    for bar_index in range(loop_start, total_bars):
+        logger.debug("\n\n")
+        datetime = candles.candle_open_datetimes[bar_index]
+        logger.debug(f"set_idx= {set_idx} bar_idx= {bar_index} datetime= {datetime}")
+
+        if order.position_size_usd > 0:
+            try:
+                current_candle = CurrentFootprintCandleTuple(
+                    open_timestamp=candles.candle_open_timestamps[bar_index],
+                    open_price=candles.candle_open_prices[bar_index],
+                    high_price=candles.candle_high_prices[bar_index],
+                    low_price=candles.candle_low_prices[bar_index],
+                    close_price=candles.candle_close_prices[bar_index],
+                )
+                logger.debug("Checking stop loss hit")
+                order.check_stop_loss_hit(
+                    current_candle=current_candle,
+                )
+                logger.debug("Checking liq hit")
+                order.check_liq_hit(
+                    current_candle=current_candle,
+                )
+                logger.debug("Checking take profit hit")
+                order.check_take_profit_hit(
+                    current_candle=current_candle,
+                    exit_price=strategy.exit_prices[bar_index],
+                )
+
+                logger.debug("Checking to move stop to break even")
+                sl_to_be_price, sl_to_be_pct = order.check_move_sl_to_be(
+                    current_candle=current_candle,
+                )
+                if sl_to_be_price:
+                    order.sl_pct = sl_to_be_pct
+                    order.sl_price = sl_to_be_price
+                    logger.debug(f"Filling order for move sl to be")
+                    order.fill_or_exit_move(
+                        bar_index=bar_index,
+                        set_idx=set_idx,
+                        order_records=order_records[or_filled],
+                        order_status=OrderStatus.MovedSLToBE,
+                        timestamp=current_candle.open_timestamp,
+                        sl_price=sl_to_be_price,
+                        sl_pct=sl_to_be_pct,
+                    )
+                    or_filled += 1
+                    logger.debug(f"Filled sl to be order records")
+
+                logger.debug("Checking to move trailing stop loss")
+                tsl_price, tsl_pct = order.check_move_tsl(
+                    current_candle=current_candle,
+                )
+                if tsl_price:
+                    order.sl_pct = tsl_pct
+                    order.sl_price = tsl_price
+                    logger.debug(f"Filling order for tsl")
+
+                    order.fill_or_exit_move(
+                        bar_index=bar_index,
+                        set_idx=set_idx,
+                        order_records=order_records[or_filled],
+                        order_status=OrderStatus.MovedTSL,
+                        timestamp=current_candle.open_timestamp,
+                        sl_pct=tsl_pct,
+                        sl_price=tsl_price,
+                    )
+                    or_filled += 1
+                    logger.debug(f"Filled move tsl order records")
+
+            except DecreasePosition as e:
+                (
+                    equity,
+                    fees_paid,
+                    realized_pnl,
+                ) = order.calculate_decrease_position(
+                    cur_datetime=current_candle.open_timestamp,
+                    exit_fee_pct=e.exit_fee_pct,
+                    exit_price=e.exit_price,
+                    order_status=e.order_status,
+                    market_fee_pct=strategy.exchange_settings_tuple.market_fee_pct,
+                    equity=order.equity,
+                )
+                logger.debug(f"Filling or for decrease postiion {OrderStatus._fields[e.order_status]}")
+                order.fill_or_exit_move(
+                    bar_index=bar_index,
+                    set_idx=set_idx,
+                    order_records=order_records[or_filled],
+                    order_status=e.order_status,
+                    timestamp=current_candle.open_timestamp,
+                    equity=equity,
+                    exit_price=e.exit_price,
+                    fees_paid=fees_paid,
+                    realized_pnl=realized_pnl,
+                )
+                or_filled += 1
+                logger.debug(f"Filled decrease postiion order records for {OrderStatus._fields[e.order_status]}")
+
+                order.set_order_variables(equity=equity)
+                logger.debug("reset order variables")
+
+            except Exception as e:
+                logger.error(f"Exception checking sl liq tp and move -> {e}")
+                raise Exception(f"Exception checking sl liq tp and move -> {e}")
+        else:
+            logger.debug("Not in a pos so not checking SL Liq or TP")
+
+        logger.debug("strategy evaluate")
+
+        beg = bar_index - loop_start
+        end = bar_index + 1
+
+        result = strategy.live_bt(
+            bar_index=bar_index,
+            beg=beg,
+            candles=candles,
+            end=end,
+        )
 
-def round_size_by_tick_step(
-    user_num: float,
-    exchange_num: float,
-) -> float:
-    return round(user_num, exchange_num)
-
-
-def fill_order_records(
-    account_state: AccountState,
-    or_index: int,
-    order_records: np.array,
-    order_result: OrderResult,
-) -> int:
-    order_records["ind_set_idx"] = account_state.ind_set_index
-    order_records["or_set_idx"] = account_state.dos_index
-    order_records["bar_idx"] = account_state.bar_index
-    order_records["timestamp"] = account_state.timestamp
-
-    order_records["equity"] = account_state.equity
-    order_records["available_balance"] = account_state.available_balance
-    order_records["cash_borrowed"] = account_state.cash_borrowed
-    order_records["cash_used"] = account_state.cash_used
-
-    order_records["average_entry"] = order_result.average_entry
-    order_records["fees_paid"] = account_state.fees_paid
-    order_records["leverage"] = order_result.leverage
-    order_records["liq_price"] = order_result.liq_price
-    order_records["order_status"] = order_result.order_status
-    order_records["total_possible_loss"] = account_state.total_possible_loss
-    order_records["total_trades"] = account_state.total_trades
-    order_records["entry_size_asset"] = order_result.entry_size_asset
-    order_records["entry_size_usd"] = order_result.entry_size_usd
-    order_records["entry_price"] = order_result.entry_price
-    order_records["exit_price"] = order_result.exit_price
-    order_records["position_size_asset"] = order_result.position_size_asset
-    order_records["position_size_usd"] = order_result.position_size_usd
-    order_records["realized_pnl"] = account_state.realized_pnl
-    order_records["sl_pct"] = round(order_result.sl_pct * 100, 3)
-    order_records["sl_price"] = order_result.sl_price
-    order_records["tp_pct"] = round(order_result.tp_pct * 100, 3)
-    order_records["tp_price"] = order_result.tp_price
-    return or_index + 1
-
-
-def log_dynamic_order_settings(
-    dos_index: int,
-    dynamic_order_settings: DynamicOrderSettingsArrays,
-):
-    logger.info(
-        f"""
-Dynamic Order settings index= {dos_index}
-max_trades={dynamic_order_settings.max_trades}
-account_pct_risk_per_trade={round(dynamic_order_settings.account_pct_risk_per_trade * 100, 3)}
-risk_reward={dynamic_order_settings.risk_reward}
-sl_based_on_add_pct={round(dynamic_order_settings.sl_based_on_add_pct * 100, 3)}
-sl_based_on_lookback={dynamic_order_settings.sl_based_on_lookback}
-sl_bcb_type={dynamic_order_settings.sl_bcb_type}
-sl_to_be_cb_type={dynamic_order_settings.sl_to_be_cb_type}
-sl_to_be_when_pct={round(dynamic_order_settings.sl_to_be_when_pct * 100, 3)}
-trail_sl_bcb_type={dynamic_order_settings.trail_sl_bcb_type}
-trail_sl_by_pct={round(dynamic_order_settings.trail_sl_by_pct * 100, 3)}
-trail_sl_when_pct={round(dynamic_order_settings.trail_sl_when_pct * 100, 3)}"""
-    )
+        if result:
+            strategy.entry_message(bar_index=bar_index)
+            try:
+                logger.debug("calculate_stop_loss")
+                sl_price = order.calculate_stop_loss(
+                    bar_index=bar_index,
+                    candles=candles,
+                )
+
+                logger.debug("calculate_increase_position")
+                (
+                    average_entry,
+                    entry_price,
+                    entry_size_asset,
+                    entry_size_usd,
+                    position_size_asset,
+                    position_size_usd,
+                    total_possible_loss,
+                    total_trades,
+                    sl_pct,
+                ) = order.calculate_increase_position(
+                    average_entry=order.average_entry,
+                    entry_price=candles.candle_close_prices[bar_index],
+                    equity=order.equity,
+                    position_size_asset=order.position_size_asset,
+                    position_size_usd=order.position_size_usd,
+                    sl_price=sl_price,
+                    total_trades=order.total_trades,
+                )
+
+                logger.debug("calculate_leverage")
+                (
+                    available_balance,
+                    cash_borrowed,
+                    cash_used,
+                    leverage,
+                    liq_price,
+                ) = order.calculate_leverage(
+                    available_balance=order.available_balance,
+                    average_entry=average_entry,
+                    cash_borrowed=order.cash_borrowed,
+                    cash_used=order.cash_used,
+                    position_size_usd=position_size_usd,
+                    position_size_asset=position_size_asset,
+                    sl_price=sl_price,
+                )
+
+                logger.debug("calculate_take_profit")
+                (
+                    can_move_sl_to_be,
+                    tp_price,
+                    tp_pct,
+                ) = order.calculate_take_profit(
+                    average_entry=average_entry,
+                    position_size_usd=position_size_usd,
+                    total_possible_loss=total_possible_loss,
+                )
+
+                logger.debug("calculate_take_profit")
+                order.fill_order_result(
+                    available_balance=available_balance,
+                    average_entry=average_entry,
+                    can_move_sl_to_be=can_move_sl_to_be,
+                    cash_borrowed=cash_borrowed,
+                    cash_used=cash_used,
+                    entry_price=entry_price,
+                    entry_size_asset=entry_size_asset,
+                    entry_size_usd=entry_size_usd,
+                    equity=order.equity,
+                    exit_price=np.nan,
+                    fees_paid=np.nan,
+                    leverage=leverage,
+                    liq_price=liq_price,
+                    order_status=OrderStatus.EntryFilled,
+                    position_size_asset=position_size_asset,
+                    position_size_usd=position_size_usd,
+                    total_possible_loss=total_possible_loss,
+                    realized_pnl=np.nan,
+                    sl_pct=sl_pct,
+                    sl_price=sl_price,
+                    total_trades=total_trades,
+                    tp_pct=tp_pct,
+                    tp_price=tp_price,
+                )
+                logger.debug("filling entry order records")
+                order.fill_or_entry(
+                    bar_index=bar_index + 1,
+                    set_idx=set_idx,
+                    order_records=order_records[or_filled],
+                    timestamp=candles.candle_open_timestamps[bar_index + 1],
+                )
+                or_filled += 1
+                logger.info("We are in a position and filled the result")
+            except RejectedOrder:
+                pass
+            except Exception as e:
+                if bar_index + 1 >= candles.candle_open_timestamps.size:
+                    raise Exception(f"Exception hit in eval strat -> {e}")
+                    pass
+                else:
+                    logger.error(f"Exception hit in eval strat -> {e}")
+                    raise Exception(f"Exception hit in eval strat -> {e}")
+    order_records_df = order_records_to_df(order_records[:or_filled])
+    pretty_qf(strategy.cur_dos_tuple)
+    pretty_qf(strategy.cur_ind_set_tuple)
+    if not disable_plot:
+        strategy.plot_signals(
+            candles=candles,
+        )
+        plot_or_results(
+            candles=candles,
+            order_records_df=order_records_df,
+        )
+    return order_records_df
```

### Comparing `quantfreedom-0.1.4.6/quantfreedom/indicators/tv_indicators.py` & `quantfreedom-0.2.0.0/quantfreedom/indicators/tv_indicators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Callable
 import numpy as np
 
-from quantfreedom.enums import CandleBodyType
+from quantfreedom.core.enums import CandleBodyType, FootprintCandlesTuple
 
 
 def wma_tv(
-    source: np.array,
+    source: np.ndarray,
     length: int,
-) -> np.array:
+) -> np.ndarray:
     """
     [Weighted Moving Average From Tradingview](https://www.tradingview.com/pine-script-reference/v5/#fun_ta.wma)
 
     [Explainer Video](https://youtu.be/eHlHoWC4W8k)
 
     Parameters
     ----------
-    source : np.array
+    source : np.ndarray
         Values to process
     length : int
         Number of bars
 
     Returns
     -------
     np.array
@@ -35,23 +35,23 @@
     for index in range(starting_index, source.size):
         the_sum = (source[index - len_minus_one : index + 1] * weight).sum()
         wma[index] = the_sum / norm
     return wma
 
 
 def sma_tv(
-    source: np.array,
+    source: np.ndarray,
     length: int,
-) -> np.array:
+) -> np.ndarray:
     """
     [Simple Moving average from tradingview](https://www.tradingview.com/pine-script-reference/v5/#fun_ta.sma)
 
     Parameters
     ----------
-    source : np.array
+    source : np.ndarray
         Values to process
     length : int
         Number of bars
 
     Returns
     -------
     np.array
@@ -65,23 +65,23 @@
     for i in range(starting_index, source.size):
         sma[i] = source[i - len_minus_one : i + 1].mean()
 
     return sma
 
 
 def ema_tv(
-    source: np.array,
+    source: np.ndarray,
     length: int,
-) -> np.array:
+) -> np.ndarray:
     """
     [Exponential Moving average from tradingview](https://www.tradingview.com/pine-script-reference/v5/#fun_ta.ema)
 
     Parameters
     ----------
-    source : np.array
+    source : np.ndarray
         Values to process
     length : int
         Number of bars
 
     Returns
     -------
     np.array
@@ -97,23 +97,23 @@
     for index in range(starting_index, source.size):
         ema[index] = alpha * source[index] + (1 - alpha) * ema[index - 1]
 
     return ema
 
 
 def rma_tv(
-    source: np.array,
+    source: np.ndarray,
     length: int,
-) -> np.array:
+) -> np.ndarray:
     """
     [Relative strength index Moving average from tradingview](https://www.tradingview.com/pine-script-reference/v5/#fun_ta.rma)
 
     Parameters
     ----------
-    source : np.array
+    source : np.ndarray
         Values to process
     length : int
         Number of bars
 
     Returns
     -------
     np.array
@@ -129,26 +129,26 @@
     for i in range(starting_index, source.size):
         rma[i] = alpha * source[i] + (1 - alpha) * rma[i - 1]
 
     return rma
 
 
 def rma_tv_2(
-    source_1: np.array,
-    source_2: np.array,
+    source_1: np.ndarray,
+    source_2: np.ndarray,
     length: int,
 ):
     """
     [Relative strength index Moving average from tradingview](https://www.tradingview.com/pine-script-reference/v5/#fun_ta.rma)
 
     Parameters
     ----------
-    source_1 : np.array
+    source_1 : np.ndarray
         Values to process
-    source_2 : np.array
+    source_2 : np.ndarray
         Values to process
     length : int
         Number of bars
 
     Returns
     -------
     np.array
@@ -168,25 +168,25 @@
         rma_1[i] = alpha * source_1[i] + (1 - alpha) * rma_1[i - 1]
         rma_2[i] = alpha * source_2[i] + (1 - alpha) * rma_2[i - 1]
 
     return rma_1, rma_2
 
 
 def stdev_tv(
-    source: np.array,
+    source: np.ndarray,
     length: int,
-) -> np.array:
+) -> np.ndarray:
     """
     [Standard deviation from tradingview](https://www.tradingview.com/pine-script-reference/v5/#fun_ta.stdev)
 
     [Explainer Video](https://youtu.be/Hejf_bzLfL4)
 
     Parameters
     ----------
-    source : np.array
+    source : np.ndarray
         Values to process
     length : int
         Number of bars
 
     Returns
     -------
     np.array
@@ -212,27 +212,27 @@
         sum_square_dev[i] = (res_2 * res_2).sum()
 
     stdev = np.sqrt(sum_square_dev / length)
     return stdev
 
 
 def macd_tv(
-    source: np.array,
+    source: np.ndarray,
     fast_length: int,
     slow_length: int,
     signal_smoothing: int,
     oscillator_type: Callable = ema_tv,
     signal_ma_type: Callable = ema_tv,
 ) -> tuple[np.array, np.array, np.array]:
     """
     [Moving average convergence divergence from tradingview](https://www.tradingview.com/pine-script-reference/v5/#fun_ta.macd)
 
     Parameters
     ----------
-    source : np.array
+    source : np.ndarray
         Values to process
     fast_length : int
         Number of bars
     slow_length : int
         Number of bars
     signal_smoothing : int
         Number of bars
@@ -253,23 +253,23 @@
     histogram = macd - signal
     return histogram, macd, signal
 
 
 def bb_tv(
     length: int,
     multi: float,
-    source: np.array,
+    source: np.ndarray,
     basis_ma_type: Callable = sma_tv,
 ) -> tuple[np.array, np.array, np.array]:
     """
     [Bollinger bands from tradingview](https://www.tradingview.com/pine-script-reference/v5/#fun_ta.bb)
 
     Parameters
     ----------
-    source : np.array
+    source : np.ndarray
         Values to process
     length : int
         Number of bars
     multi : float
         Standard deviation factor
     basis_ma_type : Callable
         Function to process basic ma
@@ -283,22 +283,22 @@
     dev = multi * stdev_tv(source=source, length=length)
     upper = basis + dev
     lower = basis - dev
     return basis, upper, lower
 
 
 def true_range_tv(
-    candles: np.array,
-) -> np.array:
+    candles: FootprintCandlesTuple,
+) -> np.ndarray:
     """
     [True Range from tradingview](https://www.tradingview.com/pine-script-reference/v5/#fun_ta.tr)
 
     Parameters
     ----------
-    candles : np.array
+    candles : np.ndarray
         2-dim np.array with columns in the following order [timestamp, open, high, low, close, volume]
 
     Returns
     -------
     np.array
         true_range
     """
@@ -313,24 +313,24 @@
         ),
         np.absolute(low - prev_close),
     )
     return true_range
 
 
 def atr_tv(
-    candles: np.array,
+    candles: FootprintCandlesTuple,
     length: int,
     smoothing_type: Callable = rma_tv,
-) -> np.array:
+) -> np.ndarray:
     """
     [Average true range smoothing from tradingview](https://www.tradingview.com/pine-script-reference/v5/#fun_ta.atr)
 
     Parameters
     ----------
-    candles : np.array
+    candles : np.ndarray
         2-dim np.array with columns in the following order [timestamp, open, high, low, close, volume]
     length : int
         Number of bars
     smoothing_type : Callable
         function to process the smoothing of the atr
 
     Returns
@@ -341,22 +341,22 @@
     true_range = true_range_tv(candles=candles)
     atr = smoothing_type(source=true_range, length=length)
     return atr
 
 
 def rsi_tv(
     length: int,
-    source: np.array,
-) -> np.array:
+    source: np.ndarray,
+) -> np.ndarray:
     """
     [Relative strength index](https://www.tradingview.com/pine-script-reference/v5/#fun_ta.rsi)
 
     Parameters
     ----------
-    source : np.array
+    source : np.ndarray
         Values to process
     length : int
         Number of bars
 
     Returns
     -------
     np.array
@@ -376,28 +376,29 @@
         source_2=losses,
         length=length,
     )
 
     rs = rma_gains / rma_losses
 
     rsi = 100 - (100 / (1 + rs))
+
     return rsi
 
 
 def supertrend_tv(
-    candles: np.array,
+    candles: FootprintCandlesTuple,
     atr_length: int,
     factor: int,
 ) -> tuple[np.array, np.array]:
     """
     [Super Trend](https://www.tradingview.com/pine-script-reference/v5/#fun_ta.supertrend)
 
     Parameters
     ----------
-    candles : np.array
+    candles : np.ndarray
         2-dim np.array with columns in the following order [timestamp, open, high, low, close, volume]
     atr_length : int
         Number of bars
     factor : int
         The multiplier by which the ATR will get multiplied
 
     Returns
@@ -448,30 +449,30 @@
             if current_close < lower_band:
                 direction[i] = 1
                 super_trend[i] = upper_band
     return super_trend, direction
 
 
 def vwap_tv(
-    candles: np.array,
-) -> np.array:
+    candles: FootprintCandlesTuple,
+) -> np.ndarray:
     """
     [Volume Weighted Average Price](https://blog.quantinsti.com/vwap-strategy/)
 
     Parameters
     ----------
-    candles : np.array
+    candles : np.ndarray
         2-dim np.array with columns in the following order [timestamp, open, high, low, close, volume]
 
     Returns
     -------
     np.array
         vwap
     """
-    timestamps = candles[:, CandleBodyType.Timestamp]
+    timestamps = candles[:, CandleBodyType.OpenTimestamp]
     high = candles[:, CandleBodyType.High]
     low = candles[:, CandleBodyType.Low]
     close = candles[:, CandleBodyType.Close]
     volume = candles[:, CandleBodyType.Volume]
 
     typical_price = (high + low + close) / 3
     tp_x_vol = typical_price * volume
@@ -497,23 +498,23 @@
         raise Exception("You need to have enough data to where you have at least one start of the day")
 
     vwap = cum_tp / cum_vol
     return vwap
 
 
 def donchain_channels_tv(
-    candles: np.array,
+    candles: FootprintCandlesTuple,
     length: int,
 ):
     """
     Donchain channels
 
     Parameters
     ----------
-    candles : np.array
+    candles : np.ndarray
         2-dim np.array with columns in the following order [timestamp, open, high, low, close, volume]
     length : int
         Number of bars of donchain lookback
 
     Returns
     -------
     tuple[np.array, np.array, np.array]
@@ -532,26 +533,26 @@
 
     basis = np.mean(np.array([upper, lower]), axis=0)
 
     return upper, basis, lower
 
 
 def squeeze_momentum_lazybear_tv(
-    candles: np.array,
+    candles: FootprintCandlesTuple,
     length_bb: int,
     length_kc: int,
     multi_bb: int,
     multi_kc: int,
 ) -> tuple[np.array, np.array, np.array]:
     """
     [LazyBear Pinescript](https://www.tradingview.com/script/nqQ1DT5a-Squeeze-Momentum-Indicator-LazyBear/)
 
     Parameters
     ----------
-    candles : np.array
+    candles : np.ndarray
         2-dim np.array with columns in the following order [timestamp, open, high, low, close, volume]
     length_bb : int
         Number of bars of Bollinger Bands
     length_kc : int
         Number of bars of KC
     multi_bb : int
         The multiplier by which the Bollinger Bands will get multiplied
@@ -600,25 +601,25 @@
         s_min_ma_hl[i] = close[i] - ma_hl_avg
         m, b = np.linalg.lstsq(A, s_min_ma_hl[i - length_kc_m_1 : i + 1], rcond=None)[0]
         sqz_hist[i] = b + m * (length_kc_m_1)
     return sqz_hist, sqz_on, no_sqz
 
 
 def linear_regression_candles_ugurvu_tv(
-    candles: np.array,
+    candles: FootprintCandlesTuple,
     lin_reg_length: int,
     smoothing_length: int,
     smoothing_type: Callable = sma_tv,
 ) -> tuple[np.array, np.array]:
     """
     [Linear regression indicator](https://www.tradingview.com/script/hMaQO1FX-Linear-Regression-Candles/)
 
     Parameters
     ----------
-    candles : np.array
+    candles : np.ndarray
         2-dim np.array with columns in the following order [timestamp, open, high, low, close, volume]
     lin_reg_length : int
         Number of bars for lin reg
     smoothing_length : int
         Number of bars for singal line
     smoothing_type : Callable
         function to process the smoothing of the singal line
@@ -654,23 +655,23 @@
         lin_reg_candles[i, CandleBodyType.Close] = b + m * (lin_reg_length_m_1)
 
     signal = smoothing_type(
         source=lin_reg_candles[:, CandleBodyType.Close],
         length=smoothing_length,
     )
 
-    lin_reg_candles[:, CandleBodyType.Timestamp] = candles[:, CandleBodyType.Timestamp]
+    lin_reg_candles[:, CandleBodyType.OpenTimestamp] = candles[:, CandleBodyType.OpenTimestamp]
     lin_reg_candles[:, CandleBodyType.Volume] = candles[:, CandleBodyType.Volume]
 
     return lin_reg_candles, signal
 
 
 def revolution_volatility_bands_tv(
     length: int,
-    source: np.array,
+    source: np.ndarray,
 ):
     basis = ema_tv(source=source, length=length)
 
     a = source - basis
     b = np.where(a < 0, a * -1, a)
     d = ema_tv(source=b, length=length)
 
@@ -698,24 +699,24 @@
         lower_rising[x] = lower_smooth[x]
         upper_falling[x] = upper_smooth[x]
 
     return upper_smooth, upper_falling, lower_smooth, lower_rising
 
 
 # def range_detextor_lux_algo_tv(
-#     candles: np.array,
+#     candles: FootprintCandlesTuple,
 #     min_range_length: int,
 #     atr_multi: int,
 #     atr_length: int,
 # ) -> tuple[np.array, np.array]:
 #     """
 #     https://www.tradingview.com/script/QOuZIuvH-Range-Detector-LuxAlgo/
 #     """
 #     close = candles[:, CandleBodyType.Close]
-#     timestamp = candles[:, CandleBodyType.Timestamp]
+#     timestamp = candles[:, CandleBodyType.OpenTimestamp]
 #     box_y = np.full(close.size * 2, np.nan)
 #     box_x = np.full(close.size * 2, np.nan)
 #     atr = atr_tv(candles=candles, length=atr_length) * atr_multi
 #     sma = sma_tv(source=close, length=min_range_length)
 
 #     count = -1
 #     box_index = 0
```

### Comparing `quantfreedom-0.1.4.6/quantfreedom/nb_funcs/nb_order_handler/nb_leverage.py` & `quantfreedom-0.2.0.0/quantfreedom/order_handler/leverage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,334 +1,277 @@
-from typing import Callable, NamedTuple
 import numpy as np
-from numba import njit
+from logging import getLogger
+from quantfreedom.core.enums import (
+    CandleBodyType,
+    CurrentFootprintCandleTuple,
+    DecreasePosition,
+    LeverageStrategyType,
+    OrderStatus,
+    RejectedOrder,
+)
+from quantfreedom.helpers.helper_funcs import round_size_by_tick_step
+
+logger = getLogger()
+
+
+class Leverage:
+    def __init__(
+        self,
+        leverage_strategy_type: LeverageStrategyType,  # type: ignore
+        leverage_tick_step: float,
+        long_short: str,
+        market_fee_pct: float,
+        max_leverage: float,
+        min_leverage: float,
+        mmr_pct: float,
+        price_tick_step: float,
+        static_leverage: float,
+    ):
+        self.min_leverage = min_leverage
+        self.price_tick_step = price_tick_step
+        self.leverage_tick_step = leverage_tick_step
+        self.max_leverage = max_leverage
+        self.mmr_pct = mmr_pct
+        self.market_fee_pct = market_fee_pct
+        self.static_leverage = static_leverage
+
+        if long_short.lower() == "long":
+            self.calc_dynamic_lev = self.long_calc_dynamic_lev
+            self.get_liq_price = self.long_get_liq_price
+            self.get_bankruptcy_price = self.long_get_bankruptcy_price
+            self.liq_hit_bool = self.long_liq_hit_bool
+        elif long_short.lower() == "short":
+            self.calc_dynamic_lev = self.short_calc_dynamic_lev
+            self.get_liq_price = self.short_get_liq_price
+            self.get_bankruptcy_price = self.short_get_bankruptcy_price
+            self.liq_hit_bool = self.short_liq_hit_bool
+        else:
+            raise Exception("long or short are the only options for long_short")
+
+        self.checker_liq_hit = self.check_liq_hit
+        if leverage_strategy_type == LeverageStrategyType.Dynamic:
+            self.lev_calculator = self.dynamic_lev
+
+    def long_get_bankruptcy_price(
+        self,
+        average_entry: float,
+        leverage: float,
+    ):
+        # https://www.bybithelp.com/en-US/s/article/Order-Cost-USDT-Contract
+        return average_entry * (leverage - 1) / leverage
 
-from quantfreedom.enums import CandleBodyType, LoggerFuncType, StringerFuncType
-from quantfreedom.nb_funcs.nb_helper_funcs import nb_round_size_by_tick_step
+    def short_get_bankruptcy_price(
+        self,
+        average_entry: float,
+        leverage: float,
+    ):
+        # https://www.bybithelp.com/en-US/s/article/Order-Cost-USDT-Contract
+        return average_entry * (leverage + 1) / leverage
 
+    def long_get_liq_price(
+        self,
+        average_entry: float,
+        leverage: float,
+    ):
+        # liq formula
+        # https://www.bybithelp.com/HelpCenterKnowledge/bybitHC_Article?id=000001067&language=en_US
+        return average_entry * (1 - (1 / leverage) + self.mmr_pct)
 
-class LevAccExOther(NamedTuple):
-    available_balance: float
-    cash_borrowed: float
-    cash_used: float
-    leverage_tick_step: float
-    market_fee_pct: float
-    max_leverage: float
-    min_leverage: float
-    mmr_pct: float
-    price_tick_step: float
-
-
-class LevOrderInfo(NamedTuple):
-    average_entry: float
-    position_size_asset: float
-    position_size_usd: float
-    sl_price: float
-    static_leverage: float
-
-
-@njit(cache=True)
-def nb_long_get_bankruptcy_price(
-    average_entry: float,
-    leverage: float,
-):
-    # https://www.bybithelp.com/en-US/s/article/Order-Cost-USDT-Contract
-    return average_entry * (leverage - 1) / leverage
-
-
-@njit(cache=True)
-def nb_long_get_liq_price(
-    average_entry: float,
-    leverage: float,
-    mmr_pct: float,
-):
-    # liq formula
-    # https://www.bybithelp.com/HelpCenterKnowledge/bybitHC_Article?id=000001067&language=en_US
-    return average_entry * (1 - (1 / leverage) + mmr_pct)
-
-
-@njit(cache=True)
-def nb_long_liq_hit_bool(
-    current_candle: np.array,
-    liq_price: float,
-    logger,
-    stringer,
-):
-    candle_low = current_candle[CandleBodyType.Low]
-    logger("nb_leverage.py - nb_check_liq_hit() - candle_low= " + stringer[StringerFuncType.float_to_str](candle_low))
-    return liq_price > candle_low
-
-
-@njit(cache=True)
-def nb_long_calc_dynamic_lev(
-    average_entry: float,
-    mmr_pct: float,
-    sl_price: float,
-):
-    # https://www.bybithelp.com/HelpCenterKnowledge/bybitHC_Article?id=000001067&language=en_US
-    # https://www.symbolab.com/solver/simplify-calculator/solve%20for%20l%2C%20e%5Ccdot%5Cleft(1-%5Cfrac%7B1%7D%7Bl%7D%2Bm%5Cright)%3Ds-s%5Ccdot%20p?or=input
-    # the .001 is to add .001 buffer
-    return average_entry / (-sl_price + sl_price * 0.001 + average_entry + average_entry * mmr_pct)
-
-
-@njit(cache=True)
-def nb_short_calc_dynamic_lev(
-    average_entry: float,
-    mmr_pct: float,
-    sl_price: float,
-):
-    # https://www.bybithelp.com/HelpCenterKnowledge/bybitHC_Article?id=000001067&language=en_US
-    # https://www.symbolab.com/solver/simplify-calculator/solve%20for%20l%2C%20e%5Ccdot%5Cleft(1%2B%5Cfrac%7B1%7D%7Bl%7D-m%5Cright)%3Ds%2Bs%5Ccdot%20p?or=input
-    # the .001 is to add .001 buffer
-    return average_entry / (sl_price + sl_price * 0.001 - average_entry + average_entry * mmr_pct)
-
-
-@njit(cache=True)
-def nb_short_get_bankruptcy_price(
-    average_entry: float,
-    leverage: float,
-):
-    # https://www.bybithelp.com/en-US/s/article/Order-Cost-USDT-Contract
-    return average_entry * (leverage + 1) / leverage
-
-
-@njit(cache=True)
-def nb_short_get_liq_price(
-    average_entry: float,
-    leverage: float,
-    mmr_pct: float,
-):
-    # liq formula
-    # https://www.bybithelp.com/HelpCenterKnowledge/bybitHC_Article?id=000001067&language=en_US
-    return average_entry * (1 + (1 / leverage) - mmr_pct)
-
-
-@njit(cache=True)
-def nb_short_liq_hit_bool(
-    current_candle: np.array,
-    liq_price: float,
-    logger,
-    stringer,
-):
-    candle_high = current_candle[CandleBodyType.High]
-    logger("nb_leverage.py - nb_short_liq_hit_bool() - candle_high= " + stringer[StringerFuncType.float_to_str](candle_high))
-    return liq_price < candle_high
-
-
-@njit(cache=True)
-def nb_calc_liq_price(
-    average_entry: float,
-    leverage: float,
-    logger,
-    market_fee_pct: float,
-    mmr_pct: float,
-    nb_get_bankruptcy_price,
-    nb_get_liq_price,
-    og_available_balance: float,
-    og_cash_borrowed: float,
-    og_cash_used: float,
-    position_size_asset: float,
-    position_size_usd: float,
-    price_tick_step: float,
-    stringer,
-):
-    # Getting Order Cost
-    # https://www.bybithelp.com/HelpCenterKnowledge/bybitHC_Article?id=000001064&language=en_US
-    initial_margin = (position_size_asset * average_entry) / leverage
-    fee_to_open = position_size_asset * average_entry * market_fee_pct  # math checked
-    bankruptcy_price = nb_get_bankruptcy_price(
-        average_entry=average_entry,
-        leverage=leverage,
-    )
-    fee_to_close = position_size_asset * bankruptcy_price * market_fee_pct
-
-    cash_used = initial_margin + fee_to_open + fee_to_close  # math checked
-    logger(
-        "nb_leverage.py - nb_calc_liq_price() -"
-        + "\ninitial_margin= "
-        + stringer[StringerFuncType.float_to_str](round(initial_margin, 3))
-        + "\nfee_to_open= "
-        + stringer[StringerFuncType.float_to_str](round(fee_to_open, 3))
-        + "\nbankruptcy_price= "
-        + stringer[StringerFuncType.float_to_str](round(bankruptcy_price, 3))
-        + "\ncash_used= "
-        + stringer[StringerFuncType.float_to_str](round(cash_used, 3))
-    )
-
-    if cash_used > og_available_balance:
-        logger("nb_leverage.py - nb_calc_liq_price() - Cash used bigger than available balance")
-        raise Exception
-    else:
+    def short_get_liq_price(
+        self,
+        average_entry: float,
+        leverage: float,
+    ):
         # liq formula
         # https://www.bybithelp.com/HelpCenterKnowledge/bybitHC_Article?id=000001067&language=en_US
-        available_balance = round(og_available_balance - cash_used, 3)
-        cash_used = round(og_cash_used + cash_used, 3)
-        cash_borrowed = round(og_cash_borrowed + position_size_usd - cash_used, 3)
+        return average_entry * (1 + (1 / leverage) - self.mmr_pct)
+
+    def calc_liq_price(
+        self,
+        average_entry: float,
+        leverage: float,
+        og_available_balance: float,
+        og_cash_borrowed: float,
+        og_cash_used: float,
+        position_size_asset: float,
+        position_size_usd: float,
+    ):
+        # Getting Order Cost
+        # https://www.bybithelp.com/HelpCenterKnowledge/bybitHC_Article?id=000001064&language=en_US
+
+        initial_margin = (position_size_asset * average_entry) / leverage
+        fee_to_open = position_size_asset * average_entry * self.market_fee_pct  # math checked
+        bankruptcy_price = self.get_bankruptcy_price(average_entry=average_entry, leverage=leverage)
+        fee_to_close = position_size_asset * bankruptcy_price * self.market_fee_pct
+
+        cash_used = initial_margin + fee_to_open + fee_to_close  # math checked
+
+        logger.debug(
+            f"""
+initial_margin= {round(initial_margin, 2)}
+fee_to_open= {round(fee_to_open, 2)}
+bankruptcy_price= {round(bankruptcy_price, 2)}
+fee to close= {round(fee_to_close, 2)}
+cash_used= {round(cash_used, 2)}
+og_available_balance= {og_available_balance}"""
+        )
+
+        if cash_used > og_available_balance:
+            msg = "Cash used bigger than available balance AKA position size too big"
+            logger.warning(msg)
+            RejectedOrder.msg = msg
+            raise RejectedOrder
+        else:
+            available_balance = round(og_available_balance - cash_used, 2)
+            cash_used = round(og_cash_used + cash_used, 2)
+            cash_borrowed = round(og_cash_borrowed + position_size_usd - cash_used, 2)
+
+            liq_price = self.get_liq_price(average_entry=average_entry, leverage=leverage)  # math checked
+            liq_price = round_size_by_tick_step(
+                user_num=liq_price,
+                exchange_num=self.price_tick_step,
+            )
+
+        return (
+            available_balance,
+            cash_borrowed,
+            cash_used,
+            liq_price,
+        )
 
-        liq_price = nb_get_liq_price(
+    def static_lev(
+        self,
+        available_balance: float,
+        average_entry: float,
+        cash_borrowed: float,
+        cash_used: float,
+        position_size_asset: float,
+        position_size_usd: float,
+        sl_price: float,
+    ):
+        (
+            available_balance,
+            can_move_sl_to_be,
+            cash_borrowed,
+            cash_used,
+            liq_price,
+        ) = self.calc_liq_price(
+            leverage=self.static_leverage,
+            position_size_asset=position_size_asset,
+            position_size_usd=position_size_usd,
             average_entry=average_entry,
-            leverage=leverage,
-            mmr_pct=mmr_pct,
-        )  # math checked
-        liq_price = nb_round_size_by_tick_step(
-            exchange_num=price_tick_step,
-            user_num=liq_price,
+            og_cash_used=cash_used,
+            og_available_balance=available_balance,
+            og_cash_borrowed=cash_borrowed,
         )
-        logger(
-            "nb_leverage.py - nb_calc_liq_price() -"
-            + "\navailable_balance= "
-            + stringer[StringerFuncType.float_to_str](available_balance)
-            + "\nnew cash_used= "
-            + stringer[StringerFuncType.float_to_str](cash_used)
-            + "\ncash_borrowed= "
-            + stringer[StringerFuncType.float_to_str](cash_borrowed)
-            + "\nliq_price= "
-            + stringer[StringerFuncType.float_to_str](liq_price)
+        logger.debug(f"Lev set to static lev= {self.static_leverage}")
+        return (
+            available_balance,
+            can_move_sl_to_be,
+            cash_borrowed,
+            cash_used,
+            self.static_leverage,
+            liq_price,
         )
 
-    return (
-        available_balance,
-        cash_borrowed,
-        cash_used,
-        liq_price,
-    )
-
-
-@njit(cache=True)
-def nb_static_lev(
-    lev_acc_ex_other: LevAccExOther,
-    lev_order_info: LevOrderInfo,
-    logger,
-    nb_calc_dynamic_lev,
-    nb_get_bankruptcy_price,
-    nb_get_liq_price,
-    stringer,
-):
-    (
-        available_balance,
-        cash_borrowed,
-        cash_used,
-        liq_price,
-    ) = nb_calc_liq_price(
-        average_entry=lev_order_info.average_entry,
-        leverage=lev_order_info.static_leverage,
-        logger=logger,
-        market_fee_pct=lev_acc_ex_other.market_fee_pct,
-        mmr_pct=lev_acc_ex_other.mmr_pct,
-        nb_get_bankruptcy_price=nb_get_bankruptcy_price,
-        nb_get_liq_price=nb_get_liq_price,
-        og_available_balance=lev_acc_ex_other.available_balance,
-        og_cash_borrowed=lev_acc_ex_other.cash_borrowed,
-        og_cash_used=lev_acc_ex_other.cash_used,
-        position_size_asset=lev_order_info.position_size_asset,
-        position_size_usd=lev_order_info.position_size_usd,
-        price_tick_step=lev_acc_ex_other.price_tick_step,
-        stringer=stringer,
-    )
-    leverage = lev_order_info.static_leverage
-    logger(
-        "nb_leverage.py - nb_calculate_leverage() - Lev set to static lev= "
-        + stringer[StringerFuncType.float_to_str](leverage)
-    )
-    return (
-        available_balance,
-        cash_borrowed,
-        cash_used,
-        leverage,
-        liq_price,
-    )
-
-
-@njit(cache=True)
-def nb_dynamic_lev(
-    lev_acc_ex_other: LevAccExOther,
-    lev_order_info: LevOrderInfo,
-    logger,
-    nb_calc_dynamic_lev,
-    nb_get_bankruptcy_price,
-    nb_get_liq_price,
-    stringer,
-):
-    leverage = nb_calc_dynamic_lev(
-        average_entry=lev_order_info.average_entry,
-        mmr_pct=lev_acc_ex_other.mmr_pct,
-        sl_price=lev_order_info.sl_price,
-    )
-    leverage = nb_round_size_by_tick_step(
-        exchange_num=lev_acc_ex_other.leverage_tick_step,
-        user_num=leverage,
-    )
-    if leverage > lev_acc_ex_other.max_leverage:
-        logger(
-            "nb_leverage.py - nb_calculate_leverage() - Lev too high"
-            + " Old Lev= "
-            + stringer[StringerFuncType.float_to_str](leverage)
-            + " Max Lev= "
-            + stringer[StringerFuncType.float_to_str](lev_acc_ex_other.max_leverage)
+    def long_calc_dynamic_lev(
+        self,
+        average_entry: float,
+        sl_price: float,
+    ):
+        # https://www.bybithelp.com/HelpCenterKnowledge/bybitHC_Article?id=000001067&language=en_US
+        # https://www.symbolab.com/solver/simplify-calculator/solve%20for%20l%2C%20e%5Ccdot%5Cleft(1-%5Cfrac%7B1%7D%7Bl%7D%2Bm%5Cright)%3Ds-s%5Ccdot%20p?or=input
+        # the .001 is to add .001 buffer
+        return average_entry / (-sl_price + sl_price * 0.001 + average_entry + average_entry * self.mmr_pct)
+
+    def short_calc_dynamic_lev(
+        self,
+        average_entry: float,
+        sl_price: float,
+    ):
+        # https://www.bybithelp.com/HelpCenterKnowledge/bybitHC_Article?id=000001067&language=en_US
+        # https://www.symbolab.com/solver/simplify-calculator/solve%20for%20l%2C%20e%5Ccdot%5Cleft(1%2B%5Cfrac%7B1%7D%7Bl%7D-m%5Cright)%3Ds%2Bs%5Ccdot%20p?or=input
+        # the .001 is to add .001 buffer
+        return average_entry / (sl_price + sl_price * 0.001 - average_entry + average_entry * self.mmr_pct)
+
+    def dynamic_lev(
+        self,
+        available_balance: float,
+        average_entry: float,
+        cash_borrowed: float,
+        cash_used: float,
+        position_size_asset: float,
+        position_size_usd: float,
+        sl_price: float,
+    ):
+        leverage = self.calc_dynamic_lev(average_entry=average_entry, sl_price=sl_price)
+        leverage = round_size_by_tick_step(
+            user_num=leverage,
+            exchange_num=self.leverage_tick_step,
         )
-        leverage = lev_acc_ex_other.max_leverage
-    elif leverage < lev_acc_ex_other.min_leverage:
-        logger(
-            "nb_leverage.py - nb_calculate_leverage() - Lev too low"
-            + " Old Lev= "
-            + stringer[StringerFuncType.float_to_str](leverage)
-            + " Min Lev= "
-            + stringer[StringerFuncType.float_to_str](lev_acc_ex_other.min_leverage)
+        if leverage > self.max_leverage:
+            logger.warning(f"Lev too high Lev= {leverage} Max Lev= {self.max_leverage}")
+            leverage = self.max_leverage
+        elif leverage < self.min_leverage:
+            logger.warning(f"Lev too low Lev= {leverage} Min Lev= {self.min_leverage}")
+            leverage = 1
+        else:
+            logger.debug(f"Leverage= {leverage}")
+
+        (
+            available_balance,
+            cash_borrowed,
+            cash_used,
+            liq_price,
+        ) = self.calc_liq_price(
+            leverage=leverage,
+            average_entry=average_entry,
+            og_cash_used=cash_used,
+            og_available_balance=available_balance,
+            og_cash_borrowed=cash_borrowed,
+            position_size_asset=position_size_asset,
+            position_size_usd=position_size_usd,
         )
-        leverage = 1.0
-    else:
-        logger(
-            "nb_leverage.py - nb_calculate_leverage() -"
-            + " Leverage= "
-            + stringer[StringerFuncType.float_to_str](leverage)
+        return (
+            available_balance,
+            cash_borrowed,
+            cash_used,
+            leverage,
+            liq_price,
         )
 
-    (
-        available_balance,
-        cash_borrowed,
-        cash_used,
-        liq_price,
-    ) = nb_calc_liq_price(
-        average_entry=lev_order_info.average_entry,
-        leverage=leverage,
-        logger=logger,
-        market_fee_pct=lev_acc_ex_other.market_fee_pct,
-        mmr_pct=lev_acc_ex_other.mmr_pct,
-        nb_get_bankruptcy_price=nb_get_bankruptcy_price,
-        nb_get_liq_price=nb_get_liq_price,
-        og_available_balance=lev_acc_ex_other.available_balance,
-        og_cash_borrowed=lev_acc_ex_other.cash_borrowed,
-        og_cash_used=lev_acc_ex_other.cash_used,
-        position_size_asset=lev_order_info.position_size_asset,
-        position_size_usd=lev_order_info.position_size_usd,
-        price_tick_step=lev_acc_ex_other.price_tick_step,
-        stringer=stringer,
-    )
-    return (
-        available_balance,
-        cash_borrowed,
-        cash_used,
-        leverage,
-        liq_price,
-    )
-
-
-@njit(cache=True)
-def nb_check_liq_hit(
-    current_candle: np.array,
-    liq_price: float,
-    logger,
-    nb_liq_hit_bool,
-    stringer,
-):
-    candle_low = current_candle[CandleBodyType.Low]
-    if nb_liq_hit_bool(
-        current_candle=current_candle,
-        logger=logger,
-        liq_price=liq_price,
-        stringer=stringer,
-    ):
-        logger("nb_leverage.py - nb_check_liq_hit() - Liq Hit")
-        return True
-    else:
-        logger("nb_leverage.py - nb_check_liq_hit() - No hit on liq price")
-        return False
+    def long_liq_hit_bool(
+        self,
+        current_candle: CurrentFootprintCandleTuple,
+        liq_price: float,
+    ):
+        candle_low = current_candle[CandleBodyType.Low]
+        logger.debug(f"candle_low= {candle_low}")
+        return liq_price > candle_low
+
+    def short_liq_hit_bool(
+        self,
+        current_candle: CurrentFootprintCandleTuple,
+        liq_price: float,
+    ):
+        candle_high = current_candle[CandleBodyType.High]
+        logger.debug(f"candle_high= {candle_high}")
+        return liq_price < candle_high
+
+    def check_liq_hit(
+        self,
+        current_candle: CurrentFootprintCandleTuple,
+        liq_price: float,
+    ):
+        if self.liq_hit_bool(
+            current_candle=current_candle,
+            liq_price=liq_price,
+        ):
+            logger.debug("Liq Hit")
+            raise DecreasePosition(
+                exit_fee_pct=self.market_fee_pct,
+                exit_price=liq_price,
+                order_status=OrderStatus.LiquidationFilled,
+            )
+        else:
+            logger.debug("No hit on liq price")
+            pass
```

### Comparing `quantfreedom-0.1.4.6/quantfreedom/order_handler/increase_position.py` & `quantfreedom-0.2.0.0/quantfreedom/order_handler/increase_position.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from logging import getLogger
-from quantfreedom.enums import (
+from quantfreedom.core.enums import (
     IncreasePositionType,
     RejectedOrder,
     StopLossStrategyType,
 )
-from quantfreedom.helper_funcs import round_size_by_tick_step
+from quantfreedom.helpers.helper_funcs import round_size_by_tick_step
 
-logger = getLogger("info")
+logger = getLogger()
 
 
 class IncreasePosition:
     account_pct_risk_per_trade: float
     max_equity_risk_pct: float
     max_trades: int
 
@@ -82,22 +82,24 @@
         Parameters
         ----------
         entry_size_asset : float
             entry size of the asset
 
         """
         if entry_size_asset < self.min_asset_size:
-            logger.warning(
-                f"entry size too small entry_size_asset= {entry_size_asset} < self.min_asset_size= {self.min_asset_size}"
-            )
+            msg = f"entry size too small entry_size_asset= {entry_size_asset} < self.min_asset_size= {self.min_asset_size}"
+            logger.warning(msg)
+            RejectedOrder.msg = msg
             raise RejectedOrder
         elif entry_size_asset > self.max_asset_size:
-            logger.warning(
+            msg = (
                 f"entry size too big entry_size_asset= {entry_size_asset} > self.max_asset_size= {self.max_asset_size}"
             )
+            logger.warning(msg)
+            RejectedOrder.msg = msg
             raise RejectedOrder
 
         logger.debug(f"Entry size is fine entry_size_asset= {entry_size_asset}")
 
     def c_pl_ra_ps(
         self,
         equity: float,
@@ -108,28 +110,28 @@
         -------
         Creates possible loss then checks if it is bigger than risk account percent size then returns the new possible loss and total trades
 
         Parameters
         ----------
         equity : float
             equity
-        total_possible_loss : float
-            total_possible_loss
         total_trades : int
             total_trades
 
         Returns
         -------
         int, int
             total_possible_loss, total_trades
         """
         total_trades += 1
 
         if total_trades > self.max_trades:
-            logger.warning(f"Max trades reached - total trades= {total_trades} max trades= {self.max_trades}")
+            msg = f"Max trades reached - total trades= {total_trades} max trades= {self.max_trades}"
+            logger.warning(msg)
+            RejectedOrder.msg = msg
             raise RejectedOrder
 
         possible_loss = -int(equity * self.account_pct_risk_per_trade)
 
         total_possible_loss = int(total_trades * possible_loss)
 
         logger.debug(
@@ -153,16 +155,14 @@
         -------
         Creates possible loss then adds 1 to total trades then checks if total trades is bigger than max trades
 
         Parameters
         ----------
         average_entry : float
             average_entry
-        total_possible_loss : float
-            total_possible_loss
         position_size_asset : float
             position_size_asset
         sl_price : float
             sl_price
         total_trades : int
             total_trades
 
@@ -170,22 +170,23 @@
         -------
         tuple[int, int]
             total_possible_loss, total_trades
         """
         total_trades += 1
 
         if total_trades > self.max_trades:
-            logger.warning(
-                f"""
+
+            msg = f"""
 Max trades reached
 Total trades= {total_trades}
 max trades= {self.max_trades}
 possible_loss= {possible_loss}
 total_possible_loss= {total_possible_loss}"""
-            )
+            logger.warning(msg)
+            RejectedOrder.msg = msg
             raise RejectedOrder
 
         pnl = -abs(average_entry - sl_price) * position_size_asset  # math checked
         fee_open = position_size_asset * average_entry * self.market_fee_pct  # math checked
         fee_close = position_size_asset * sl_price * self.market_fee_pct  # math checked
         fees_paid = fee_open + fee_close  # math checked
         possible_loss = -int(pnl - fees_paid)
@@ -308,30 +309,30 @@
             total_trades,
             sl_pct
         """
         position_size_asset += self.min_asset_size
         entry_size_asset = self.min_asset_size
         logger.debug(f"entry_size_asset= {entry_size_asset} position_size_asset{position_size_asset}")
 
-        entry_size_usd = round(self.min_asset_size * entry_price, 3)
+        entry_size_usd = round(self.min_asset_size * entry_price, 2)
         logger.debug(f"entry_size_usd = {entry_size_usd}")
 
         average_entry = (entry_size_usd + position_size_usd) / (
             (entry_size_usd / entry_price) + (position_size_usd / average_entry)
         )
         average_entry = round_size_by_tick_step(
             user_num=average_entry,
             exchange_num=self.price_tick_step,
         )
         logger.debug(f"average_entry {average_entry}")
 
-        sl_pct = round(abs(average_entry - sl_price) / average_entry, 3)
-        logger.debug(f"sl_pct= {round(sl_pct*100, 3)}")
+        sl_pct = round(abs(average_entry - sl_price) / average_entry, 2)
+        logger.debug(f"sl_pct= {round(sl_pct*100, 2)}")
 
-        position_size_usd = round(entry_size_usd + position_size_usd, 3)
+        position_size_usd = round(entry_size_usd + position_size_usd, 2)
         logger.debug(f"position_size_usd= {position_size_usd}")
 
         total_possible_loss, total_trades = self.c_total_trades(
             average_entry=average_entry,
             total_possible_loss=total_possible_loss,
             total_trades=total_trades,
             position_size_asset=position_size_asset,
@@ -381,21 +382,21 @@
             total_possible_loss,
             total_trades,
             sl_pct
         """
         entry_size_asset = position_size_asset = self.min_asset_size
         logger.debug(f"entry_size_asset={entry_size_asset} position_size_asset= {position_size_asset}")
 
-        entry_size_usd = position_size_usd = round(entry_size_asset * entry_price, 3)
+        entry_size_usd = position_size_usd = round(entry_size_asset * entry_price, 2)
         logger.debug(f"entry_size_usd= {entry_size_usd} position_size_usd= {position_size_usd}")
 
         average_entry = entry_price
         logger.debug(f"average_entry {average_entry}")
-        sl_pct = round(abs(average_entry - sl_price) / average_entry, 3)
-        logger.debug(f"sl_pct= {round(sl_pct*100, 3)}")
+        sl_pct = round(abs(average_entry - sl_price) / average_entry, 2)
+        logger.debug(f"sl_pct= {round(sl_pct*100, 2)}")
 
         total_possible_loss, total_trades = self.c_total_trades(
             average_entry=average_entry,
             position_size_asset=position_size_asset,
             total_possible_loss=0,
             sl_price=sl_price,
             total_trades=0,
@@ -498,15 +499,15 @@
         Returns
         -------
         float
             entry_size_usd
         """
         price_mult_loss = entry_price * -total_possible_loss
         div_by = -sl_price + entry_price + entry_price * self.market_fee_pct + self.market_fee_pct * sl_price
-        entry_size_usd = round(price_mult_loss / div_by, 3)
+        entry_size_usd = round(price_mult_loss / div_by, 2)
         return entry_size_usd
 
     def short_entry_size_p(
         self,
         average_entry: float,
         entry_price: float,
         position_size_usd: float,
@@ -585,15 +586,15 @@
         Returns
         -------
         float
             entry_size_usd
         """
         price_mult_loss = entry_price * -total_possible_loss
         div_by = -entry_price + sl_price + entry_price * self.market_fee_pct + self.market_fee_pct * sl_price
-        entry_size_usd = round(price_mult_loss / div_by, 3)
+        entry_size_usd = round(price_mult_loss / div_by, 2)
         return entry_size_usd
 
     def rpa_slbcb(
         self,
         equity: float,
         average_entry: float,
         entry_price: float,
@@ -727,28 +728,28 @@
 
         position_size_asset = round_size_by_tick_step(
             user_num=position_size_asset + entry_size_asset,
             exchange_num=self.asset_tick_step,
         )
         logger.debug(f"position_size_asset= {position_size_asset}")
 
-        position_size_usd = round(entry_size_usd + position_size_usd, 3)
+        position_size_usd = round(entry_size_usd + position_size_usd, 2)
         logger.debug(f"position_size_usd= {position_size_usd}")
 
         average_entry = (entry_size_usd + position_size_usd) / (
             (entry_size_usd / entry_price) + (position_size_usd / average_entry)
         )
         average_entry = round_size_by_tick_step(
             user_num=average_entry,
             exchange_num=self.price_tick_step,
         )
         logger.debug(f"average_entry= {average_entry}")
 
-        sl_pct = round(abs(average_entry - sl_price) / average_entry, 3)
-        logger.debug(f"sl_pct= {round(sl_pct * 100, 3)}")
+        sl_pct = round(abs(average_entry - sl_price) / average_entry, 2)
+        logger.debug(f"sl_pct= {round(sl_pct * 100, 2)}")
         return (
             average_entry,
             entry_price,
             entry_size_asset,
             entry_size_usd,
             position_size_asset,
             position_size_usd,
@@ -805,16 +806,16 @@
             user_num=entry_size_usd / entry_price,
             exchange_num=self.asset_tick_step,
         )
         self.c_too_b_s(entry_size_asset=entry_size_asset)
 
         average_entry = entry_price
 
-        sl_pct = round(abs(average_entry - sl_price) / average_entry, 3)
-        logger.debug(f"sl_pct= {round(sl_pct * 100, 3)}")
+        sl_pct = round(abs(average_entry - sl_price) / average_entry, 2)
+        logger.debug(f"sl_pct= {round(sl_pct * 100, 2)}")
         return (
             average_entry,
             entry_price,
             entry_size_asset,
             entry_size_usd,
             position_size_asset,
             position_size_usd,
```

### Comparing `quantfreedom-0.1.4.6/quantfreedom/order_handler/order.py` & `quantfreedom-0.2.0.0/quantfreedom/order_handler/order.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,90 @@
-from logging import getLogger
 import numpy as np
-from quantfreedom.enums import (
-    OrderStatus,
-    DynamicOrderSettings,
-    ExchangeSettings,
-    StaticOrderSettings,
-)
+
+from logging import getLogger
+
 from quantfreedom.order_handler.increase_position import IncreasePosition
 from quantfreedom.order_handler.leverage import Leverage
 from quantfreedom.order_handler.stop_loss import StopLoss
 from quantfreedom.order_handler.take_profit import TakeProfit
 
+from quantfreedom.core.enums import (
+    CurrentFootprintCandleTuple,
+    FootprintCandlesTuple,
+    OrderStatus,
+    DynamicOrderSettings,
+    ExchangeSettings,
+    StaticOrderSettings,
+)
 
-logger = getLogger("info")
+logger = getLogger()
 
 
 class OrderHandler:
     cach_borrowed = 0
 
     def __init__(
         self,
-        exchange_settings: ExchangeSettings,
+        exchange_settings_tuple: ExchangeSettings,
         long_short: str,
-        static_os: StaticOrderSettings,
+        static_os_tuple: StaticOrderSettings,
     ) -> None:
         # Decrease Position
         if long_short.lower() == "long":
             self.pnl_calc = self.long_pnl_calc
         elif long_short.lower() == "short":
             self.pnl_calc = self.short_pnl_calc
         else:
             raise Exception("long or short are the only options for long_short")
 
         self.obj_stop_loss = StopLoss(
             long_short=long_short,
-            market_fee_pct=exchange_settings.market_fee_pct,
-            pg_min_max_sl_bcb=static_os.pg_min_max_sl_bcb,
-            price_tick_step=exchange_settings.price_tick_step,
-            sl_strategy_type=static_os.sl_strategy_type,
-            sl_to_be_bool=static_os.sl_to_be_bool,
-            trail_sl_bool=static_os.trail_sl_bool,
-            z_or_e_type=static_os.z_or_e_type,
+            market_fee_pct=exchange_settings_tuple.market_fee_pct,
+            pg_min_max_sl_bcb=static_os_tuple.pg_min_max_sl_bcb,
+            price_tick_step=exchange_settings_tuple.price_tick_step,
+            sl_strategy_type=static_os_tuple.sl_strategy_type,
+            sl_to_be_bool=static_os_tuple.sl_to_be_bool,
+            trail_sl_bool=static_os_tuple.trail_sl_bool,
+            z_or_e_type=static_os_tuple.z_or_e_type,
         )
         self.obj_inc_pos = IncreasePosition(
-            asset_tick_step=exchange_settings.asset_tick_step,
-            increase_position_type=static_os.increase_position_type,
+            asset_tick_step=exchange_settings_tuple.asset_tick_step,
+            increase_position_type=static_os_tuple.increase_position_type,
             long_short=long_short,
-            market_fee_pct=exchange_settings.market_fee_pct,
-            max_asset_size=exchange_settings.max_asset_size,
-            min_asset_size=exchange_settings.min_asset_size,
-            price_tick_step=exchange_settings.price_tick_step,
-            sl_strategy_type=static_os.sl_strategy_type,
+            market_fee_pct=exchange_settings_tuple.market_fee_pct,
+            max_asset_size=exchange_settings_tuple.max_asset_size,
+            min_asset_size=exchange_settings_tuple.min_asset_size,
+            price_tick_step=exchange_settings_tuple.price_tick_step,
+            sl_strategy_type=static_os_tuple.sl_strategy_type,
         )
         self.obj_leverage = Leverage(
-            leverage_strategy_type=static_os.leverage_strategy_type,
-            leverage_tick_step=exchange_settings.leverage_tick_step,
+            leverage_strategy_type=static_os_tuple.leverage_strategy_type,
+            leverage_tick_step=exchange_settings_tuple.leverage_tick_step,
             long_short=long_short,
-            market_fee_pct=exchange_settings.market_fee_pct,
-            max_leverage=exchange_settings.max_leverage,
-            min_leverage=exchange_settings.min_leverage,
-            mmr_pct=exchange_settings.mmr_pct,
-            price_tick_step=exchange_settings.price_tick_step,
-            static_leverage=static_os.static_leverage,
+            market_fee_pct=exchange_settings_tuple.market_fee_pct,
+            max_leverage=exchange_settings_tuple.max_leverage,
+            min_leverage=exchange_settings_tuple.min_leverage,
+            mmr_pct=exchange_settings_tuple.mmr_pct,
+            price_tick_step=exchange_settings_tuple.price_tick_step,
+            static_leverage=static_os_tuple.static_leverage,
         )
 
-        if static_os.tp_fee_type.lower() == "market":
-            tp_fee_pct = exchange_settings.market_fee_pct
-        elif static_os.tp_fee_type.lower() == "limit":
-            tp_fee_pct = exchange_settings.limit_fee_pct
+        if static_os_tuple.tp_fee_type.lower() == "market":
+            tp_fee_pct = exchange_settings_tuple.market_fee_pct
+        elif static_os_tuple.tp_fee_type.lower() == "limit":
+            tp_fee_pct = exchange_settings_tuple.limit_fee_pct
         else:
             raise Exception("market or limit are the only options for tp_fee_type")
 
         self.obj_take_profit = TakeProfit(
             long_short=long_short,
-            market_fee_pct=exchange_settings.market_fee_pct,
-            price_tick_step=exchange_settings.price_tick_step,
+            market_fee_pct=exchange_settings_tuple.market_fee_pct,
+            price_tick_step=exchange_settings_tuple.price_tick_step,
             tp_fee_pct=tp_fee_pct,
-            tp_strategy_type=static_os.tp_strategy_type,
+            tp_strategy_type=static_os_tuple.tp_strategy_type,
         )
 
     def pass_func(self, **kwargs):
         pass
 
     def set_order_variables(self, equity: float):
         self.available_balance = equity
@@ -106,28 +110,26 @@
         self.total_trades = 0
         self.tp_pct = 0.0
         self.tp_price = 0.0
 
     def fill_or_exit_move(
         self,
         bar_index: int,
-        dos_index: int,
-        ind_set_index: int,
-        order_records: np.array,
+        order_records: np.ndarray,
         order_status: OrderStatus,  # type: ignore
         timestamp: int,
+        set_idx: int,
         equity: float = np.nan,
         exit_price: float = np.nan,
         fees_paid: float = np.nan,
         realized_pnl: float = np.nan,
         sl_pct: float = np.nan,
         sl_price: float = np.nan,
     ):
-        order_records["ind_set_idx"] = ind_set_index
-        order_records["or_set_idx"] = dos_index
+        order_records["set_idx"] = set_idx
         order_records["bar_idx"] = bar_index
         order_records["timestamp"] = timestamp
 
         order_records["equity"] = equity
         order_records["available_balance"] = equity
         order_records["cash_borrowed"] = np.nan
         order_records["cash_used"] = np.nan
@@ -150,21 +152,19 @@
         order_records["sl_price"] = sl_price
         order_records["tp_pct"] = np.nan
         order_records["tp_price"] = np.nan
 
     def fill_or_entry(
         self,
         bar_index: int,
-        dos_index: int,
-        ind_set_index: int,
-        order_records: np.array,
+        set_idx: int,
+        order_records: np.ndarray,
         timestamp: int,
     ):
-        order_records["ind_set_idx"] = ind_set_index
-        order_records["or_set_idx"] = dos_index
+        order_records["set_idx"] = set_idx
         order_records["bar_idx"] = bar_index
         order_records["timestamp"] = timestamp
 
         order_records["equity"] = self.equity
         order_records["available_balance"] = self.available_balance
         order_records["cash_borrowed"] = self.cash_borrowed
         order_records["cash_used"] = self.cash_used
@@ -179,52 +179,64 @@
         order_records["entry_size_asset"] = self.entry_size_asset
         order_records["entry_size_usd"] = self.entry_size_usd
         order_records["entry_price"] = self.entry_price
         order_records["exit_price"] = self.exit_price
         order_records["position_size_asset"] = self.position_size_asset
         order_records["position_size_usd"] = self.position_size_usd
         order_records["realized_pnl"] = self.realized_pnl
-        order_records["sl_pct"] = round(self.sl_pct * 100, 3)
+        order_records["sl_pct"] = round(self.sl_pct * 100, 2)
         order_records["sl_price"] = self.sl_price
-        order_records["tp_pct"] = round(self.tp_pct * 100, 3)
+        order_records["tp_pct"] = round(self.tp_pct * 100, 2)
         order_records["tp_price"] = self.tp_price
 
-    def check_move_tsl(self, current_candle: np.array):
+    def check_move_tsl(
+        self,
+        current_candle: CurrentFootprintCandleTuple,
+    ):
         return self.obj_stop_loss.checker_tsl(
             average_entry=self.average_entry,
             current_candle=current_candle,
             sl_price=self.sl_price,
         )
 
-    def check_move_sl_to_be(self, current_candle: np.array):
+    def check_move_sl_to_be(
+        self,
+        current_candle: CurrentFootprintCandleTuple,
+    ):
         return self.obj_stop_loss.checker_sl_to_be(
             average_entry=self.average_entry,
             can_move_sl_to_be=self.can_move_sl_to_be,
             current_candle=current_candle,
             sl_price=self.sl_price,
         )
 
-    def check_liq_hit(self, current_candle: np.array):
+    def check_liq_hit(
+        self,
+        current_candle: CurrentFootprintCandleTuple,
+    ):
         self.obj_leverage.checker_liq_hit(
             current_candle=current_candle,
             liq_price=self.liq_price,
         )
 
     def check_take_profit_hit(
         self,
-        current_candle: np.array,
+        current_candle: CurrentFootprintCandleTuple,
         exit_price: float,
     ):
         self.obj_take_profit.checker_tp_hit(
             exit_price=exit_price,
             current_candle=current_candle,
             tp_price=self.tp_price,
         )
 
-    def check_stop_loss_hit(self, current_candle: np.array):
+    def check_stop_loss_hit(
+        self,
+        current_candle: CurrentFootprintCandleTuple,
+    ):
         self.obj_stop_loss.checker_sl_hit(
             current_candle=current_candle,
             sl_price=self.sl_price,
         )
 
     def update_class_dos(
         self,
@@ -246,15 +258,15 @@
         self.obj_stop_loss.trail_sl_bcb_type = dynamic_order_settings.trail_sl_bcb_type
         self.obj_stop_loss.trail_sl_by_pct = dynamic_order_settings.trail_sl_by_pct
         self.obj_stop_loss.trail_sl_when_pct = dynamic_order_settings.trail_sl_when_pct
 
     def calculate_stop_loss(
         self,
         bar_index: int,
-        candles: np.array,
+        candles: FootprintCandlesTuple,
     ):
         sl_price = self.obj_stop_loss.sl_calculator(
             bar_index=bar_index,
             candles=candles,
         )
         logger.info(f"sl price= {sl_price}")
         return sl_price
@@ -292,15 +304,16 @@
             f"""
 average_entry= {average_entry}
 entry_price= {entry_price}
 entry_size_asset= {entry_size_asset}
 entry_size_usd= {entry_size_usd}
 position_size_asset= {position_size_asset}
 position_size_usd= {position_size_usd}
-sl_pct= {round(sl_pct*100, 3)}"""
+sl_pct= {round(sl_pct*100, 2)}
+"""
         )
         return (
             average_entry,
             entry_price,
             entry_size_asset,
             entry_size_usd,
             position_size_asset,
@@ -337,15 +350,16 @@
         )
         logger.info(
             f"""
 available_balance= {available_balance}
 cash_borrowed= {cash_borrowed}
 cash_used= {cash_used}
 leverage= {leverage}
-liq_price= {liq_price}"""
+liq_price= {liq_price}
+"""
         )
         return (
             available_balance,
             cash_borrowed,
             cash_used,
             leverage,
             liq_price,
@@ -365,60 +379,64 @@
             average_entry=average_entry,
             position_size_usd=position_size_usd,
             total_possible_loss=total_possible_loss,
         )
         logger.info(
             f"""
 tp_price= {tp_price}
-tp_pct= {round(tp_pct * 100, 3)}"""
+tp_pct= {round(tp_pct * 100, 2)}
+"""
         )
         return (
             can_move_sl_to_be,
             tp_price,
             tp_pct,
         )
 
     def long_pnl_calc(self, exit_price: float):
-        return round((exit_price - self.average_entry) * self.position_size_asset, 3)  # math checked
+        return round((exit_price - self.average_entry) * self.position_size_asset, 2)  # math checked
 
     def short_pnl_calc(self, exit_price: float):
-        return round((self.average_entry - exit_price) * self.position_size_asset, 3)  # math checked
+        return round((self.average_entry - exit_price) * self.position_size_asset, 2)  # math checked
 
     def calculate_decrease_position(
         self,
+        cur_datetime: str,
         exit_fee_pct: float,
         exit_price: float,
         equity: float,
         market_fee_pct: float,
         order_status: OrderStatus,  # type: ignore
     ):
         pnl = self.pnl_calc(exit_price=exit_price)  # math checked
         logger.debug(f"pnl= {pnl}")
 
-        fee_open = round(self.position_size_asset * self.average_entry * market_fee_pct, 3)  # math checked
+        fee_open = round(self.position_size_asset * self.average_entry * market_fee_pct, 2)  # math checked
         logger.debug(f"fee_open= {fee_open}")
 
-        fee_close = round(self.position_size_asset * exit_price * exit_fee_pct, 3)  # math checked
+        fee_close = round(self.position_size_asset * exit_price * exit_fee_pct, 2)  # math checked
         logger.debug(f"fee_close= {fee_close}")
 
-        fees_paid = round(fee_open + fee_close, 3)  # math checked
+        fees_paid = round(fee_open + fee_close, 2)  # math checked
         logger.debug(f"fees_paid= {fees_paid}")
 
-        realized_pnl = round(pnl - fees_paid, 3)  # math checked
+        realized_pnl = round(pnl - fees_paid, 2)  # math checked
         logger.debug(f"realized_pnl= {realized_pnl}")
 
-        equity = round(realized_pnl + equity, 3)
+        equity = round(realized_pnl + equity, 2)
         logger.debug(f"equity= {equity}")
 
         logger.info(
             f"""
+datetime= {cur_datetime}
 equity= {equity}
 fees_paid= {fees_paid}
 order_status= {OrderStatus._fields[order_status]}
-realized_pnl= {realized_pnl}"""
+realized_pnl= {realized_pnl}
+"""
         )
         return (
             equity,
             fees_paid,
             realized_pnl,
         )
```

### Comparing `quantfreedom-0.1.4.6/quantfreedom/order_handler/stop_loss.py` & `quantfreedom-0.2.0.0/quantfreedom/order_handler/stop_loss.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 import numpy as np
 from logging import getLogger
 
-from quantfreedom.helper_funcs import round_size_by_tick_step
-from quantfreedom.enums import (
+from quantfreedom.helpers.helper_funcs import round_size_by_tick_step
+from quantfreedom.core.enums import (
     CandleBodyType,
+    CurrentFootprintCandleTuple,
     DecreasePosition,
+    FootprintCandlesTuple,
     OrderStatus,
     StopLossStrategyType,
 )
 
-logger = getLogger("info")
+logger = getLogger()
 
 
 class StopLoss:
     sl_based_on_add_pct: float
-    sl_based_on_lookback: float
+    sl_based_on_lookback: int
     sl_bcb_type: int
     sl_to_be_cb_type: int
     sl_to_be_when_pct: float
-    trail_sl_bcb_type: float
+    trail_sl_bcb_type: int
     trail_sl_by_pct: float
     trail_sl_when_pct: float
 
     def __init__(
         self,
         long_short: str,
         market_fee_pct: float,
         pg_min_max_sl_bcb: str,
         price_tick_step: float,
-        sl_strategy_type: StopLossStrategyType,
+        sl_strategy_type: StopLossStrategyType,  # type: ignore
         sl_to_be_bool: bool,
         trail_sl_bool: bool,
         z_or_e_type: str,
     ) -> None:
         self.market_fee_pct = market_fee_pct
         self.price_tick_step = price_tick_step
 
@@ -81,75 +83,100 @@
         if trail_sl_bool:
             self.checker_tsl = self.check_move_tsl
         else:
             self.checker_tsl = self.pass_func
 
     # Long Functions
 
-    def long_sl_price_calc(self, candle_body: float, add_pct: float):
+    def long_sl_price_calc(
+        self,
+        candle_body: float,
+        add_pct: float,
+    ):
         sl_price = candle_body - (candle_body * add_pct)
         return sl_price
 
     def long_sl_hit_bool(
         self,
-        current_candle: np.array,
+        current_candle: CurrentFootprintCandleTuple,
         sl_price: float,
     ):
         logger.debug("Starting")
-        candle_low = current_candle[CandleBodyType.Low]
+        candle_low = current_candle.low_price
         logger.debug(f"candle_low= {candle_low}")
         return sl_price > candle_low
 
     def long_sl_to_zero_price(self, average_entry: float):
         sl_price = (average_entry + self.market_fee_pct * average_entry) / (1 - self.market_fee_pct)
         return sl_price
 
     def num_greater_than_num(self, num_1: float, num_2: float):
         return num_1 > num_2
 
     # Short Functions
 
     def short_sl_hit_bool(
         self,
-        current_candle: np.array,
+        current_candle: CurrentFootprintCandleTuple,
         sl_price: float,
     ):
         logger.debug("Starting")
-        candle_high = current_candle[CandleBodyType.High]
+        candle_high = current_candle.high_price
         logger.debug(f"candle_high= {candle_high}")
         return sl_price < candle_high
 
-    def short_sl_price_calc(self, candle_body: float, add_pct: float):
+    def short_sl_price_calc(
+        self,
+        candle_body: float,
+        add_pct: float,
+    ):
         sl_price = candle_body + (candle_body * add_pct)
         return sl_price
 
-    def short_sl_to_zero_price(self, average_entry: float):
-        sl_price = (average_entry - self.market_fee_pct * average_entry) / (1 + self.market_fee_pct)
+    def short_sl_to_zero_price(
+        self,
+        average_entry: float,
+    ):
+        numerator = average_entry - self.market_fee_pct * average_entry
+        denominator = 1 + self.market_fee_pct
+        sl_price = numerator / denominator
         return sl_price
 
-    def num_less_than_num(self, num_1: float, num_2: float):
+    def num_less_than_num(
+        self,
+        num_1: float,
+        num_2: float,
+    ):
         return num_1 < num_2
 
     # Main Functions
-    def sl_to_zero(self, average_entry: float):
-        sl_price = self.sl_to_zero_price(average_entry=average_entry)
+    def sl_to_zero(
+        self,
+        average_entry: float,
+    ):
+        sl_price = self.sl_to_zero_price(
+            average_entry=average_entry,
+        )
         sl_price = round_size_by_tick_step(
             user_num=sl_price,
             exchange_num=self.price_tick_step,
         )
         return sl_price
 
-    def sl_to_entry(self, average_entry: float):
+    def sl_to_entry(
+        self,
+        average_entry: float,
+    ):
         sl_price = average_entry
         return sl_price
 
     def sl_based_on_candle_body(
         self,
         bar_index: int,
-        candles: np.array,
+        candles: FootprintCandlesTuple,
     ) -> float:
         """
         Long Stop Loss Based on Candle Body Calculator
         """
         # lb will be bar index if sl isn't based on lookback because look back will be 0
         lookback = max(bar_index - self.sl_based_on_lookback, 0)
         logger.debug(f"lookback to index= {lookback}")
@@ -172,15 +199,15 @@
         )
         logger.debug(f"sl_price= {sl_price}")
 
         return sl_price
 
     def check_sl_hit(
         self,
-        current_candle: np.array,
+        current_candle: CurrentFootprintCandleTuple,
         sl_price: float,
     ):
         if self.get_sl_hit(
             current_candle=current_candle,
             sl_price=sl_price,
         ):
             logger.debug(f"Stop loss hit sl_price= {sl_price}")
@@ -193,87 +220,94 @@
             logger.debug("No hit on stop loss")
             pass
 
     def check_move_sl_to_be(
         self,
         average_entry: float,
         can_move_sl_to_be: bool,
-        current_candle: np.array,
+        current_candle: CurrentFootprintCandleTuple,
         sl_price: float,
     ):
         """
         Checking to see if we move the stop loss to break even
         """
         if can_move_sl_to_be:
             logger.debug("Might move sl to break even")
             # Stop Loss to break even
             candle_body = current_candle[self.sl_to_be_cb_type]
             pct_from_ae = abs(candle_body - average_entry) / average_entry
-            logger.debug(f"pct_from_ae= {round(pct_from_ae * 100, 3)}")
+            logger.debug(f"pct_from_ae= {round(pct_from_ae * 100, 2)}")
             move_sl_bool = self.move_sl_bool(num_1=pct_from_ae, num_2=self.sl_to_be_when_pct)
             if move_sl_bool:
                 old_sl = sl_price
                 sl_price = self.zero_or_entry_calc(average_entry=average_entry)
-                sl_pct = round(abs(average_entry - sl_price) / average_entry, 3)
-                logger.debug(f"Moving old_sl= {old_sl} to new sl= {sl_price} sl_pct= {round(sl_pct*100, 3)}")
+                sl_pct = round(abs(average_entry - sl_price) / average_entry, 2)
+                logger.debug(f"Moving old_sl= {old_sl} to new sl= {sl_price} sl_pct= {round(sl_pct*100, 2)}")
                 return sl_price, sl_pct
             else:
                 logger.debug("not moving sl to be")
                 return None, None
         else:
             logger.debug("can't move sl to be")
             return None, None
 
     def check_move_tsl(
         self,
         average_entry: float,
-        current_candle: np.array,
+        current_candle: CurrentFootprintCandleTuple,
         sl_price: float,
     ):
         """
         Checking to see if we move the trailing stop loss
         """
         candle_body = current_candle[self.trail_sl_bcb_type]
         pct_from_ae = abs(candle_body - average_entry) / average_entry
-        logger.debug(f"pct_from_ae= {round(pct_from_ae * 100, 3)}")
+        logger.debug(f"pct_from_ae= {round(pct_from_ae * 100, 2)}")
         possible_move_tsl = self.move_sl_bool(num_1=pct_from_ae, num_2=self.trail_sl_when_pct)
         if possible_move_tsl:
             logger.debug("Maybe move tsl")
             temp_sl_price = self.sl_price_calc(candle_body=candle_body, add_pct=self.trail_sl_by_pct)
             temp_sl_price = round_size_by_tick_step(
                 user_num=temp_sl_price,
                 exchange_num=self.price_tick_step,
             )
             logger.debug(f"temp sl= {temp_sl_price}")
             if self.move_sl_bool(num_1=temp_sl_price, num_2=sl_price):
-                sl_pct = round(abs(average_entry - temp_sl_price) / average_entry, 3)
-                logger.debug(f"Moving tsl new sl= {temp_sl_price} > old sl= {sl_price} sl_pct= {round(sl_pct*100, 3)}")
+                sl_pct = round(abs(average_entry - temp_sl_price) / average_entry, 2)
+                logger.debug(f"Moving tsl new sl= {temp_sl_price} > old sl= {sl_price} sl_pct= {round(sl_pct*100, 2)}")
                 return temp_sl_price, sl_pct
             else:
                 logger.debug("Wont move tsl")
                 return None, None
         else:
             logger.debug("Not moving tsl")
             return None, None
 
     def min_price_getter(
         self,
         bar_index: int,
-        candles: np.array,
+        candles: FootprintCandlesTuple,
         lookback: int,
         candle_body_type: int,
     ) -> float:
-        price = candles[lookback : bar_index + 1, candle_body_type].min()
-        return price
+        the_prices = candles[candle_body_type]
+        lb_the_prices = the_prices[lookback : bar_index + 1]
+        final_the_prices = lb_the_prices.min()
+        return final_the_prices
 
     def max_price_getter(
         self,
         bar_index: int,
-        candles: np.array,
+        candles: FootprintCandlesTuple,
         lookback: int,
         candle_body_type: int,
     ) -> float:
-        price = candles[lookback : bar_index + 1, candle_body_type].max()
-        return price
+        the_prices = candles[candle_body_type]
+        lb_the_prices = the_prices[lookback : bar_index + 1]
+        final_the_prices = lb_the_prices.max()
+        return final_the_prices
 
     def pass_func(self, **kwargs):
         return None, None
+
+    def sl_to_zero_price(self, **kwargs):
+        pass
```

### Comparing `quantfreedom-0.1.4.6/quantfreedom/order_handler/take_profit.py` & `quantfreedom-0.2.0.0/quantfreedom/order_handler/take_profit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 import numpy as np
+
 from logging import getLogger
-from quantfreedom.helper_funcs import round_size_by_tick_step
-from quantfreedom.enums import CandleBodyType, DecreasePosition, OrderStatus, TakeProfitStrategyType
 
-logger = getLogger("info")
+from quantfreedom.helpers.helper_funcs import round_size_by_tick_step
+from quantfreedom.core.enums import (
+    CandleBodyType,
+    CurrentFootprintCandleTuple,
+    DecreasePosition,
+    OrderStatus,
+    TakeProfitStrategyType,
+)
+
+logger = getLogger()
 
 
 class TakeProfit:
     risk_reward: float
 
     def __init__(
         self,
         long_short: str,
         market_fee_pct: float,
         price_tick_step: float,
         tp_fee_pct: float,
-        tp_strategy_type: TakeProfitStrategyType,
+        tp_strategy_type: TakeProfitStrategyType,  # type: ignore
     ):
         self.market_fee_pct = market_fee_pct
         self.price_tick_step = price_tick_step
         self.tp_fee_pct = tp_fee_pct
 
         if long_short.lower() == "long":
             self.get_tp_price = self.long_tp_price
@@ -51,15 +59,15 @@
             - (average_entry * position_size_usd)
             + (average_entry * self.market_fee_pct * position_size_usd)
         ) / (position_size_usd * (1 + self.tp_fee_pct))
         return tp_price
 
     def short_c_tp_candle(
         self,
-        current_candle: np.array,
+        current_candle: CurrentFootprintCandleTuple,
         tp_price: float,
     ):
         candle_low = current_candle[CandleBodyType.Low]
         logger.debug(f"candle_high= {candle_low}")
         return tp_price > candle_low
 
     def long_tp_price(
@@ -73,15 +81,15 @@
             + (average_entry * position_size_usd)
             + (average_entry * self.market_fee_pct * position_size_usd)
         ) / (position_size_usd * (1 - self.tp_fee_pct))
         return tp_price
 
     def long_c_tp_candle(
         self,
-        current_candle: np.array,
+        current_candle: CurrentFootprintCandleTuple,
         tp_price: float,
     ):
         candle_high = current_candle[CandleBodyType.High]
         logger.debug(f"candle_high= {candle_high}")
         result = tp_price < candle_high
         return result
 
@@ -101,16 +109,16 @@
 
         tp_price = round_size_by_tick_step(
             user_num=tp_price,
             exchange_num=self.price_tick_step,
         )
         logger.debug(f"tp_price= {tp_price}")
 
-        tp_pct = round(abs((tp_price - average_entry)) / average_entry, 3)
-        logger.debug(f"tp_pct= {round(tp_pct * 100, 3)}")
+        tp_pct = round(abs((tp_price - average_entry)) / average_entry, 2)
+        logger.debug(f"tp_pct= {round(tp_pct * 100, 2)}")
         can_move_sl_to_be = True
         logger.debug("can_move_sl_to_be= True")
         return (
             can_move_sl_to_be,
             tp_price,
             tp_pct,
         )
@@ -129,15 +137,15 @@
             can_move_sl_to_be,
             tp_price,
             tp_pct,
         )
 
     def c_tp_hit_regular(
         self,
-        current_candle: np.array,
+        current_candle: CurrentFootprintCandleTuple,
         exit_price: float,
         tp_price: float,
     ):
         if self.get_check_tp_candle_price(
             current_candle=current_candle,
             tp_price=tp_price,
         ):
@@ -149,23 +157,23 @@
             )
         else:
             logger.debug("No Tp Hit")
             pass
 
     def c_tp_hit_nothing(
         self,
-        current_candle: np.array,
+        current_candle: CurrentFootprintCandleTuple,
         exit_price: float,
         tp_price: float,
     ):
         pass
 
     def c_tp_hit_provided(
         self,
-        current_candle: np.array,
+        current_candle: CurrentFootprintCandleTuple,
         exit_price: float,
         tp_price: float,
     ):
         if not np.isnan(exit_price):
             logger.debug(f"TP Hit tp_price= {exit_price}")
             raise DecreasePosition(
                 exit_fee_pct=self.tp_fee_pct,
```

### Comparing `quantfreedom-0.1.4.6/quantfreedom/plotting/plotting_base.py` & `quantfreedom-0.2.0.0/quantfreedom/core/plotting_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import numpy as np
 import pandas as pd
-from quantfreedom.enums import CandleBodyType
+from quantfreedom.core.enums import CandleBodyType, FootprintCandlesTuple
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
 
 def plot_candles_1_ind_same_pane(
-    candles: np.array,
-    indicator: np.array,
+    candles: FootprintCandlesTuple,
+    indicator: np.ndarray,
     ind_name: str,
     ind_color: str = "yellow",
 ):
-    datetimes = candles[:, CandleBodyType.Timestamp].astype("datetime64[ms]")
+    datetimes = candles[:, CandleBodyType.OpenTimestamp].astype("datetime64[ms]")
     fig = go.Figure()
     fig.add_candlestick(
         x=datetimes,
         open=candles[:, 1],
         high=candles[:, 2],
         low=candles[:, 3],
         close=candles[:, 4],
@@ -28,20 +28,20 @@
         line_color=ind_color,
     )
     fig.update_layout(height=800, xaxis_rangeslider_visible=False)
     return fig
 
 
 def plot_candles_1_ind_dif_pane(
-    candles: np.array,
-    indicator: np.array,
+    candles: FootprintCandlesTuple,
+    indicator: np.ndarray,
     ind_name: str,
     ind_color: str = "yellow",
 ):
-    datetimes = candles[:, CandleBodyType.Timestamp].astype("datetime64[ms]")
+    datetimes = candles[:, CandleBodyType.OpenTimestamp].astype("datetime64[ms]")
     fig = make_subplots(
         cols=1,
         rows=2,
         shared_xaxes=True,
         subplot_titles=["Candles", ind_name],
         row_heights=[0.6, 0.4],
         vertical_spacing=0.1,
@@ -70,16 +70,16 @@
     )
 
     fig.update_layout(height=800, xaxis_rangeslider_visible=False)
     fig.show()
 
 
 def plot_vwap(
-    candles: np.array,
-    indicator: np.array,
+    candles: FootprintCandlesTuple,
+    indicator: np.ndarray,
     ind_color: str = "yellow",
 ):
     fig = plot_candles_1_ind_same_pane(
         candles=candles,
         indicator=indicator,
         ind_name="VWAP",
         ind_color=ind_color,
@@ -94,16 +94,16 @@
             ),
         ),
     )
     fig.show()
 
 
 def plot_rma(
-    candles: np.array,
-    indicator: np.array,
+    candles: FootprintCandlesTuple,
+    indicator: np.ndarray,
     ind_color: str = "yellow",
 ):
     fig = plot_candles_1_ind_same_pane(
         candles=candles,
         indicator=indicator,
         ind_name="RMA",
         ind_color=ind_color,
@@ -119,16 +119,16 @@
             ),
         ),
     )
     fig.show()
 
 
 def plot_wma(
-    candles: np.array,
-    indicator: np.array,
+    candles: FootprintCandlesTuple,
+    indicator: np.ndarray,
     ind_color: str = "yellow",
 ):
     fig = plot_candles_1_ind_same_pane(
         candles=candles,
         indicator=indicator,
         ind_name="WMA",
         ind_color=ind_color,
@@ -144,16 +144,16 @@
             ),
         ),
     )
     fig.show()
 
 
 def plot_sma(
-    candles: np.array,
-    indicator: np.array,
+    candles: FootprintCandlesTuple,
+    indicator: np.ndarray,
     ind_color: str = "yellow",
 ):
     fig = plot_candles_1_ind_same_pane(
         candles=candles,
         indicator=indicator,
         ind_name="SMA",
         ind_color=ind_color,
@@ -169,16 +169,16 @@
             ),
         ),
     )
     fig.show()
 
 
 def plot_ema(
-    candles: np.array,
-    indicator: np.array,
+    candles: FootprintCandlesTuple,
+    indicator: np.ndarray,
     ind_color: str = "yellow",
 ):
     fig = plot_candles_1_ind_same_pane(
         candles=candles,
         indicator=indicator,
         ind_name="EMA",
         ind_color=ind_color,
@@ -194,59 +194,59 @@
             ),
         ),
     )
     fig.show()
 
 
 def plot_rsi(
-    candles: np.array,
-    indicator: np.array,
+    candles: FootprintCandlesTuple,
+    indicator: np.ndarray,
     ind_color: str = "yellow",
 ):
     return plot_candles_1_ind_dif_pane(
         candles=candles,
         indicator=indicator,
         ind_name="RSI",
         ind_color=ind_color,
     )
 
 
 def plot_atr(
-    candles: np.array,
-    indicator: np.array,
+    candles: FootprintCandlesTuple,
+    indicator: np.ndarray,
     ind_color: str = "red",
 ):
     return plot_candles_1_ind_dif_pane(
         candles=candles,
         indicator=indicator,
         ind_name="ATR",
         ind_color=ind_color,
     )
 
 
 def plot_stdev(
-    candles: np.array,
-    indicator: np.array,
+    candles: FootprintCandlesTuple,
+    indicator: np.ndarray,
     ind_color: str = "yellow",
 ):
     return plot_candles_1_ind_dif_pane(
         candles=candles,
         indicator=indicator,
         ind_name="STDEV",
         ind_color=ind_color,
     )
 
 
 def plot_bollinger_bands(
-    candles: np.array,
-    indicator: np.array,
+    candles: FootprintCandlesTuple,
+    indicator: np.ndarray,
     ul_rgb: str = "48, 123, 255",
     basis_color_rgb: str = "255, 176, 0",
 ):
-    datetimes = candles[:, CandleBodyType.Timestamp].astype("datetime64[ms]")
+    datetimes = candles[:, CandleBodyType.OpenTimestamp].astype("datetime64[ms]")
     fig = go.Figure(
         data=[
             go.Scatter(
                 x=datetimes,
                 y=indicator[:, 2],
                 name="lower",
                 line_color=f"rgb({ul_rgb})",
@@ -287,20 +287,20 @@
             ),
         ),
     )
     fig.show()
 
 
 def plot_macd(
-    candles: np.array,
-    signal: np.array,
-    histogram: np.array,
-    macd: np.array,
+    candles: FootprintCandlesTuple,
+    signal: np.ndarray,
+    histogram: np.ndarray,
+    macd: np.ndarray,
 ):
-    datetimes = candles[:, CandleBodyType.Timestamp].astype("datetime64[ms]")
+    datetimes = candles[:, CandleBodyType.OpenTimestamp].astype("datetime64[ms]")
     fig = make_subplots(
         cols=1,
         rows=2,
         shared_xaxes=True,
         subplot_titles=["Candles", "MACD"],
         row_heights=[0.6, 0.4],
         vertical_spacing=0.1,
@@ -352,18 +352,18 @@
     )
     # Update options and show plot
     fig.update_layout(height=800, xaxis_rangeslider_visible=False)
     fig.show()
 
 
 def plot_squeeze_mom_lazybear(
-    candles: np.array,
-    indicator: np.array,
+    candles: FootprintCandlesTuple,
+    indicator: np.ndarray,
 ):
-    datetimes = candles[:, CandleBodyType.Timestamp].astype("datetime64[ms]")
+    datetimes = candles[:, CandleBodyType.OpenTimestamp].astype("datetime64[ms]")
     fig = make_subplots(
         cols=1,
         rows=2,
         shared_xaxes=True,
         subplot_titles=["Candles", "Squeeze LazyBear"],
         row_heights=[0.6, 0.4],
         vertical_spacing=0.1,
@@ -400,15 +400,15 @@
     )
     # Update options and show plot
     fig.update_layout(height=800, xaxis_rangeslider_visible=False)
     fig.show()
 
 
 def plot_or_results(
-    candles: np.array,
+    candles: FootprintCandlesTuple,
     order_records_df: pd.DataFrame,
 ):
     fig = make_subplots(
         cols=1,
         rows=2,
         shared_xaxes=True,
         subplot_titles=["Candles", "Cumulative Realized PnL"],
@@ -416,19 +416,19 @@
         vertical_spacing=0.1,
     )
 
     try:
         # Candles
         fig.add_trace(
             go.Candlestick(
-                x=candles[:, CandleBodyType.Timestamp].astype("datetime64[ms]"),
-                open=candles[:, 1],
-                high=candles[:, 2],
-                low=candles[:, 3],
-                close=candles[:, 4],
+                x=candles.candle_open_datetimes,
+                open=candles.candle_open_prices,
+                high=candles.candle_high_prices,
+                low=candles.candle_low_prices,
+                close=candles.candle_close_prices,
                 name="Candles",
             ),
             col=1,
             row=1,
         )
     except:
         pass
@@ -455,14 +455,37 @@
             ),
             col=1,
             row=1,
         )
     except:
         pass
     try:
+        # avg Entries
+        fig.add_trace(
+            go.Scatter(
+                x=entries_dt,
+                y=entries_df["average_entry"],
+                mode="markers",
+                name="Avgerage Entries",
+                marker=dict(
+                    size=10,
+                    symbol="circle",
+                    color="#DE66FF",
+                    line=dict(
+                        width=1,
+                        color="DarkSlateGrey",
+                    ),
+                ),
+            ),
+            col=1,
+            row=1,
+        )
+    except:
+        pass
+    try:
         fig.add_trace(
             # Stop Losses
             go.Scatter(
                 x=entries_dt,
                 y=entries_df["sl_price"],
                 mode="markers",
                 name="Stop Losses",
@@ -579,17 +602,21 @@
             row=1,
         )
     except:
         pass
     try:
         pnl_dt_df = order_records_df[~order_records_df["realized_pnl"].isna()]["datetime"]
         dt_list = pnl_dt_df.to_list()
-        dt_list.insert(0, candles[0, 0].astype("datetime64[ms]"))
+        dt_list.insert(
+            0,
+            candles.candle_open_datetimes[0],
+        )
 
-        pnl_df = order_records_df[~order_records_df["realized_pnl"].isna()]["realized_pnl"]
+        pnl_df_no_nan = order_records_df[~order_records_df["realized_pnl"].isna()]
+        pnl_df = pnl_df_no_nan["realized_pnl"]
         pnl_list = pnl_df.to_list()
         pnl_list.insert(0, 0)
         cumulative_pnl = np.array(pnl_list).cumsum()
         # Cumulative Realized PnL
         fig.add_trace(
             go.Scatter(
                 x=dt_list,
@@ -604,18 +631,18 @@
         pass
     fig.update_layout(height=1000, xaxis_rangeslider_visible=False)
     fig.update_yaxes(tickformat="$,")
     fig.show()
 
 
 def plot_supertrend(
-    candles: np.array,
-    indicator: np.array,
+    candles: FootprintCandlesTuple,
+    indicator: np.ndarray,
 ):
-    datetimes = candles[:, CandleBodyType.Timestamp].astype("datetime64[ms]")
+    datetimes = candles[:, CandleBodyType.OpenTimestamp].astype("datetime64[ms]")
     lower = np.where(indicator[:, 1] < 0, indicator[:, 0], np.nan)
     upper = np.where(indicator[:, 1] > 0, indicator[:, 0], np.nan)
     fig = go.Figure(
         data=[
             go.Candlestick(
                 x=datetimes,
                 open=candles[:, 1],
@@ -648,18 +675,18 @@
             ),
         ),
     )
     fig.show()
 
 
 def plot_linear_regression_candles_ugurvu_tv(
-    lin_reg_candles: np.array,
-    signal: np.array,
+    lin_reg_candles: FootprintCandlesTuple,
+    signal: np.ndarray,
 ):
-    datetimes = lin_reg_candles[:, CandleBodyType.Timestamp].astype("datetime64[ms]")
+    datetimes = lin_reg_candles[:, CandleBodyType.OpenTimestamp].astype("datetime64[ms]")
     fig = go.Figure(
         data=[
             go.Candlestick(
                 x=datetimes,
                 open=lin_reg_candles[:, CandleBodyType.Open],
                 high=lin_reg_candles[:, CandleBodyType.High],
                 low=lin_reg_candles[:, CandleBodyType.Low],
@@ -675,22 +702,22 @@
         ]
     )
     fig.update_layout(height=800, xaxis_rangeslider_visible=False)
     fig.show()
 
 
 def plot_revolution_volatility_bands_tv(
-    candles: np.array,
-    upper_smooth: np.array,
-    upper_falling: np.array,
-    lower_smooth: np.array,
-    lower_rising: np.array,
+    candles: FootprintCandlesTuple,
+    upper_smooth: np.ndarray,
+    upper_falling: np.ndarray,
+    lower_smooth: np.ndarray,
+    lower_rising: np.ndarray,
     ind_color: str = "yellow",
 ):
-    datetimes = candles[:, CandleBodyType.Timestamp].astype("datetime64[ms]")
+    datetimes = candles[:, CandleBodyType.OpenTimestamp].astype("datetime64[ms]")
     fig = go.Figure()
     fig.add_candlestick(
         x=datetimes,
         open=candles[:, 1],
         high=candles[:, 2],
         low=candles[:, 3],
         close=candles[:, 4],
@@ -721,18 +748,18 @@
         line=dict(color="blue", width=6),
     )
     fig.update_layout(height=800, xaxis_rangeslider_visible=False)
     fig.show()
 
 
 def plot_volume(
-    candles: np.array,
-    moving_average: np.array = None,
+    candles: FootprintCandlesTuple,
+    moving_average: np.ndarray = None,
 ):
-    datetimes = candles[:, CandleBodyType.Timestamp].astype("datetime64[ms]")
+    datetimes = candles[:, CandleBodyType.OpenTimestamp].astype("datetime64[ms]")
     close_prices = candles[:, CandleBodyType.Close]
     open_prices = candles[:, CandleBodyType.Open]
     volume = candles[:, CandleBodyType.Volume]
 
     fig = go.Figure()
     fig.add_bar(
         x=datetimes,
@@ -747,19 +774,19 @@
         )
     fig.update_layout(height=400, xaxis_rangeslider_visible=False)
     fig.show()
 
 
 """
 def plot_range_detextor_LuxAlgo(
-    candles: np.array,
-    box_x: np.array,
-    box_y: np.array,
+    candles: FootprintCandlesTuple,
+    box_x: np.ndarray,
+    box_y: np.ndarray,
 ):
-    datetimes = candles[:, CandleBodyType.Timestamp].astype("datetime64[ms]")
+    datetimes = candles[:, CandleBodyType.OpenTimestamp].astype("datetime64[ms]")
     fig = go.Figure(
         data=[
             go.Candlestick(
                 x=datetimes,
                 open=candles[:, 1],
                 high=candles[:, 2],
                 low=candles[:, 3],
```

### Comparing `quantfreedom-0.1.4.6/quantfreedom/utils.py` & `quantfreedom-0.2.0.0/quantfreedom/helpers/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import NamedTuple
+from typing import NamedTuple, Optional
 import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
 
 from pathlib import Path
 from IPython.paths import get_ipython_cache_dir
 
@@ -32,14 +32,16 @@
     """
     for p in Path(get_ipython_cache_dir() + "\\numba_cache").rglob("*.nb*"):
         p.unlink()
     for p in Path(__file__).parent.parent.rglob("numba_cache"):
         delete_dir(p)
     for p in Path(__file__).parent.parent.rglob("__pycache__"):
         delete_dir(p)
+    for p in Path(__file__).parent.parent.rglob("cdk.out"):
+        delete_dir(p)
     for p in Path(__file__).parent.parent.rglob("*.py[co]"):
         p.unlink()
 
 
 def pretty_qf(
     named_tuple: NamedTuple,
 ):
@@ -58,18 +60,40 @@
         for x in range(len(named_tuple)):
             items.append(indent + named_tuple._fields[x] + " = " + str(named_tuple[x]) + ",\n")
         return print(type(named_tuple).__name__ + "(" + "\n" + "".join(items) + ")")
     except:
         return named_tuple
 
 
+def pretty_qf_string(
+    named_tuple: NamedTuple,
+):
+    """
+    Prints named tuples in a pretty way
+
+    Parameters
+    ----------
+    named_tuple : namedtuple
+        must only be a named tuple
+    """
+    try:
+        named_tuple._fields[0]
+        items = []
+        indent = str("    ")
+        for x in range(len(named_tuple)):
+            items.append(indent + named_tuple._fields[x] + " = " + str(named_tuple[x]) + ",\n")
+        return type(named_tuple).__name__ + "(" + "\n" + "".join(items) + ")"
+    except:
+        return named_tuple
+
+
 def generate_candles(
     number_of_candles: int = 100,
     plot_candles: bool = False,
-    seed: int = None,
+    seed: Optional[int] = None,
 ):
     """
     Generate a dataframe filled with random candles
 
     Parameters
     ----------
     number_of_candles : int, 100
@@ -84,15 +108,15 @@
     pdFrame
         Dataframe of open high low close
     """
     np.random.seed(seed)
 
     periods = number_of_candles * 48
 
-    prices = np.around(30000 + np.random.normal(scale=1, size=periods).cumsum(), 3)
+    prices = np.around(30000 + np.random.normal(scale=1, size=periods).cumsum(), 2)
 
     data = pd.DataFrame(
         prices,
         index=pd.Index(
             pd.date_range("01/01/2000", periods=periods, freq="30min"),
             name="open_time",
         ),
```

