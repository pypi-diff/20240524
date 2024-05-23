# Comparing `tmp/biobear-0.20.2.tar.gz` & `tmp/biobear-0.20.3.tar.gz`

## Comparing `biobear-0.20.2.tar` & `biobear-0.20.3.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0      413 1970-01-01 00:00:00.000000 biobear-0.20.2/Cargo.toml
--rw-r--r--   0     1001      127       18 2024-05-21 16:32:44.000000 biobear-0.20.2/.github/FUNDING.yml
--rw-r--r--   0     1001      127     3295 2024-05-21 16:32:44.000000 biobear-0.20.2/.github/biobear.svg
--rw-r--r--   0     1001      127      100 2024-05-21 16:32:44.000000 biobear-0.20.2/.github/dependabot.yml
--rw-r--r--   0     1001      127     4104 2024-05-21 16:32:44.000000 biobear-0.20.2/.github/workflows/release.yml
--rw-r--r--   0     1001      127     1517 2024-05-21 16:32:44.000000 biobear-0.20.2/.github/workflows/smoke-test.yml
--rw-r--r--   0     1001      127      143 2024-05-21 16:32:44.000000 biobear-0.20.2/.github/workflows/smoketest.py
--rw-r--r--   0     1001      127     1160 2024-05-21 16:32:44.000000 biobear-0.20.2/.github/workflows/test.yml
--rw-r--r--   0     1001      127     4135 2024-05-21 16:32:44.000000 biobear-0.20.2/.gitignore
--rw-r--r--   0     1001      127     4593 2024-05-21 16:32:44.000000 biobear-0.20.2/CHANGELOG.md
--rw-r--r--   0     1001      127     1055 2024-05-21 16:32:44.000000 biobear-0.20.2/LICENSE
--rw-r--r--   0     1001      127      273 2024-05-21 16:32:44.000000 biobear-0.20.2/Makefile
--rw-r--r--   0     1001      127     7956 2024-05-21 16:32:44.000000 biobear-0.20.2/README.md
--rw-r--r--   0     1001      127      393 2024-05-21 16:32:44.000000 biobear-0.20.2/benchmarks/biobear-scan.py
--rw-r--r--   0     1001      127      467 2024-05-21 16:32:44.000000 biobear-0.20.2/benchmarks/biopython-scan.py
--rw-r--r--   0     1001      127      979 2024-05-21 16:32:44.000000 biobear-0.20.2/benchmarks/results.json
--rw-r--r--   0     1001      127     1569 2024-05-21 16:32:44.000000 biobear-0.20.2/bin/test.sh
--rw-r--r--   0     1001      127      285 2024-05-21 16:32:44.000000 biobear-0.20.2/cz.json
--rw-r--r--   0     1001      127      252 2024-05-21 16:32:44.000000 biobear-0.20.2/docs.bash
--rw-r--r--   0     1001      127     2587 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/__init__.py
--rw-r--r--   0     1001      127     2304 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/bam_reader.py
--rw-r--r--   0     1001      127     2087 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/bcf_reader.py
--rw-r--r--   0     1001      127     7988 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/biobear.pyi
--rw-r--r--   0     1001      127     1309 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/compression.py
--rw-r--r--   0     1001      127     1762 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/fasta_reader.py
--rw-r--r--   0     1001      127     1756 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/fastq_reader.py
--rw-r--r--   0     1001      127      858 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/genbank_reader.py
--rw-r--r--   0     1001      127     1564 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/gff_reader.py
--rw-r--r--   0     1001      127     1566 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/gtf_reader.py
--rw-r--r--   0     1001      127     1050 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/mzml_reader.py
--rw-r--r--   0     1001      127        0 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/py.typed
--rw-r--r--   0     1001      127     2910 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/reader.py
--rw-r--r--   0     1001      127     2129 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/vcf_reader.py
--rw-r--r--   0     1001      127   124562 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/BGC0000404.gbk
--rw-r--r--   0     1001      127     6152 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/bedcov.bam
--rw-r--r--   0     1001      127     7608 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/bedcov.bam.bai
--rw-r--r--   0     1001      127      939 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/cram/0500_mapped.cram
--rw-r--r--   0     1001      127     7275 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/cram/1404_index_multislice.cram
--rw-r--r--   0     1001      127      156 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/cram/1404_index_multislice.cram.crai
--rw-r--r--   0     1001      127  1060702 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/cram/ce.fa
--rw-r--r--   0     1001      127      230 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/cram/ce.fa.fai
--rw-r--r--   0     1001      127     3178 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/cram/test_input_1_a.cram
--rw-r--r--   0     1001      127   339527 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/fake_fastq_file.fastq.gz
--rw-r--r--   0     1001      127     1749 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/file.vcf
--rw-r--r--   0     1001      127     9521 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/index.bcf
--rw-r--r--   0     1001      127      143 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/index.bcf.csi
--rw-r--r--   0     1001      127     8638 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/index.vcf.gz
--rw-r--r--   0     1001      127      213 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/index.vcf.gz.tbi
--rw-r--r--   0     1001      127       41 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.fa
--rw-r--r--   0     1001      127       55 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.fa.gz
--rw-r--r--   0     1001      127       41 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.fasta
--rw-r--r--   0     1001      127       22 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.fasta.fai
--rw-r--r--   0     1001      127       58 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.fasta.gz
--rw-r--r--   0     1001      127      286 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.fastq
--rw-r--r--   0     1001      127      134 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.fastq.gz
--rw-r--r--   0     1001      127      286 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.fq
--rw-r--r--   0     1001      127      156 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.fq.gz
--rw-r--r--   0     1001      127      112 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.gff
--rw-r--r--   0     1001      127       91 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.gff.gz
--rw-r--r--   0     1001      127    17994 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.gtf
--rw-r--r--   0     1001      127     1478 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.gtf.gz
--rw-r--r--   0     1001      127    17171 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.mzML
--rw-r--r--   0     1001      127     2845 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.mzML.gz
--rw-r--r--   0     1001      127     1025 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/two-cram/rand1k.fa
--rw-r--r--   0     1001      127       20 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/two-cram/rand1k.fa.fai
--rw-r--r--   0     1001      127     1029 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/two-cram/twolib.sorted.cram
--rw-r--r--   0     1001      127       42 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/two-cram/twolib.sorted.cram.crai
--rw-r--r--   0     1001      127     1669 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/vcf-partition/sample=1/vcf_file.vcf.gz
--rw-r--r--   0     1001      127      254 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/vcf-partition/sample=1/vcf_file.vcf.gz.tbi
--rw-r--r--   0     1001      127     4302 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/vcf_file.vcf
--rw-r--r--   0     1001      127     1669 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/vcf_file.vcf.gz
--rw-r--r--   0     1001      127      254 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/vcf_file.vcf.gz.tbi
--rw-r--r--   0     1001      127    14881 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/test_session.py
--rw-r--r--   0     1001      127       47 2024-05-21 16:32:44.000000 biobear-0.20.2/requirements-dev.txt
--rw-r--r--   0     1001      127     3705 2024-05-21 16:32:44.000000 biobear-0.20.2/src/bam_reader.rs
--rw-r--r--   0     1001      127     3590 2024-05-21 16:32:44.000000 biobear-0.20.2/src/bcf_reader.rs
--rw-r--r--   0     1001      127     1397 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/bam.rs
--rw-r--r--   0     1001      127     1631 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/bcf.rs
--rw-r--r--   0     1001      127     1561 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/bed.rs
--rw-r--r--   0     1001      127     2572 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/bigwig.rs
--rw-r--r--   0     1001      127     1548 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/cram.rs
--rw-r--r--   0     1001      127     3265 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/fasta.rs
--rw-r--r--   0     1001      127     3322 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/fastq.rs
--rw-r--r--   0     1001      127     1353 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/fcs.rs
--rw-r--r--   0     1001      127     1380 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/genbank.rs
--rw-r--r--   0     1001      127     1913 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/gff.rs
--rw-r--r--   0     1001      127     1476 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/gtf.rs
--rw-r--r--   0     1001      127     1322 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/hmm_dom_tab.rs
--rw-r--r--   0     1001      127     1224 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/mod.rs
--rw-r--r--   0     1001      127     1517 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/mzml.rs
--rw-r--r--   0     1001      127     1071 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/sam.rs
--rw-r--r--   0     1001      127     2839 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/vcf.rs
--rw-r--r--   0     1001      127     2606 2024-05-21 16:32:44.000000 biobear-0.20.2/src/error.rs
--rw-r--r--   0     1001      127     4634 2024-05-21 16:32:44.000000 biobear-0.20.2/src/execution_result.rs
--rw-r--r--   0     1001      127     3784 2024-05-21 16:32:44.000000 biobear-0.20.2/src/exon_reader.rs
--rw-r--r--   0     1001      127     3225 2024-05-21 16:32:44.000000 biobear-0.20.2/src/file_compression_type.rs
--rw-r--r--   0     1001      127     2706 2024-05-21 16:32:44.000000 biobear-0.20.2/src/lib.rs
--rw-r--r--   0     1001      127     1247 2024-05-21 16:32:44.000000 biobear-0.20.2/src/runtime.rs
--rw-r--r--   0     1001      127     9978 2024-05-21 16:32:44.000000 biobear-0.20.2/src/session_context.rs
--rw-r--r--   0     1001      127     3752 2024-05-21 16:32:44.000000 biobear-0.20.2/src/vcf_reader.rs
--rw-r--r--   0     1001      127   111359 2024-05-21 16:32:48.000000 biobear-0.20.2/Cargo.lock
--rw-r--r--   0     1001      127      725 2024-05-21 16:32:44.000000 biobear-0.20.2/pyproject.toml
--rw-r--r--   0        0        0     8469 1970-01-01 00:00:00.000000 biobear-0.20.2/PKG-INFO
+-rw-r--r--   0        0        0      413 1970-01-01 00:00:00.000000 biobear-0.20.3/Cargo.toml
+-rw-r--r--   0     1001      127       18 2024-05-23 22:20:00.000000 biobear-0.20.3/.github/FUNDING.yml
+-rw-r--r--   0     1001      127     3295 2024-05-23 22:20:00.000000 biobear-0.20.3/.github/biobear.svg
+-rw-r--r--   0     1001      127      100 2024-05-23 22:20:00.000000 biobear-0.20.3/.github/dependabot.yml
+-rw-r--r--   0     1001      127     4104 2024-05-23 22:20:00.000000 biobear-0.20.3/.github/workflows/release.yml
+-rw-r--r--   0     1001      127     1517 2024-05-23 22:20:00.000000 biobear-0.20.3/.github/workflows/smoke-test.yml
+-rw-r--r--   0     1001      127      143 2024-05-23 22:20:00.000000 biobear-0.20.3/.github/workflows/smoketest.py
+-rw-r--r--   0     1001      127     1160 2024-05-23 22:20:00.000000 biobear-0.20.3/.github/workflows/test.yml
+-rw-r--r--   0     1001      127     4135 2024-05-23 22:20:00.000000 biobear-0.20.3/.gitignore
+-rw-r--r--   0     1001      127     4618 2024-05-23 22:20:00.000000 biobear-0.20.3/CHANGELOG.md
+-rw-r--r--   0     1001      127     1055 2024-05-23 22:20:00.000000 biobear-0.20.3/LICENSE
+-rw-r--r--   0     1001      127      273 2024-05-23 22:20:00.000000 biobear-0.20.3/Makefile
+-rw-r--r--   0     1001      127     7956 2024-05-23 22:20:00.000000 biobear-0.20.3/README.md
+-rw-r--r--   0     1001      127      393 2024-05-23 22:20:00.000000 biobear-0.20.3/benchmarks/biobear-scan.py
+-rw-r--r--   0     1001      127      467 2024-05-23 22:20:00.000000 biobear-0.20.3/benchmarks/biopython-scan.py
+-rw-r--r--   0     1001      127      979 2024-05-23 22:20:00.000000 biobear-0.20.3/benchmarks/results.json
+-rw-r--r--   0     1001      127     1569 2024-05-23 22:20:00.000000 biobear-0.20.3/bin/test.sh
+-rw-r--r--   0     1001      127      285 2024-05-23 22:20:00.000000 biobear-0.20.3/cz.json
+-rw-r--r--   0     1001      127      252 2024-05-23 22:20:00.000000 biobear-0.20.3/docs.bash
+-rw-r--r--   0     1001      127     2587 2024-05-23 22:20:00.000000 biobear-0.20.3/python/biobear/__init__.py
+-rw-r--r--   0     1001      127     2304 2024-05-23 22:20:00.000000 biobear-0.20.3/python/biobear/bam_reader.py
+-rw-r--r--   0     1001      127     2087 2024-05-23 22:20:00.000000 biobear-0.20.3/python/biobear/bcf_reader.py
+-rw-r--r--   0     1001      127     7988 2024-05-23 22:20:00.000000 biobear-0.20.3/python/biobear/biobear.pyi
+-rw-r--r--   0     1001      127     1309 2024-05-23 22:20:00.000000 biobear-0.20.3/python/biobear/compression.py
+-rw-r--r--   0     1001      127     1762 2024-05-23 22:20:00.000000 biobear-0.20.3/python/biobear/fasta_reader.py
+-rw-r--r--   0     1001      127     1756 2024-05-23 22:20:00.000000 biobear-0.20.3/python/biobear/fastq_reader.py
+-rw-r--r--   0     1001      127      858 2024-05-23 22:20:00.000000 biobear-0.20.3/python/biobear/genbank_reader.py
+-rw-r--r--   0     1001      127     1564 2024-05-23 22:20:00.000000 biobear-0.20.3/python/biobear/gff_reader.py
+-rw-r--r--   0     1001      127     1566 2024-05-23 22:20:00.000000 biobear-0.20.3/python/biobear/gtf_reader.py
+-rw-r--r--   0     1001      127     1050 2024-05-23 22:20:00.000000 biobear-0.20.3/python/biobear/mzml_reader.py
+-rw-r--r--   0     1001      127        0 2024-05-23 22:20:00.000000 biobear-0.20.3/python/biobear/py.typed
+-rw-r--r--   0     1001      127     2910 2024-05-23 22:20:00.000000 biobear-0.20.3/python/biobear/reader.py
+-rw-r--r--   0     1001      127     2129 2024-05-23 22:20:00.000000 biobear-0.20.3/python/biobear/vcf_reader.py
+-rw-r--r--   0     1001      127   124562 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/BGC0000404.gbk
+-rw-r--r--   0     1001      127     6152 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/bedcov.bam
+-rw-r--r--   0     1001      127     7608 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/bedcov.bam.bai
+-rw-r--r--   0     1001      127      939 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/cram/0500_mapped.cram
+-rw-r--r--   0     1001      127     7275 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/cram/1404_index_multislice.cram
+-rw-r--r--   0     1001      127      156 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/cram/1404_index_multislice.cram.crai
+-rw-r--r--   0     1001      127  1060702 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/cram/ce.fa
+-rw-r--r--   0     1001      127      230 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/cram/ce.fa.fai
+-rw-r--r--   0     1001      127     3178 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/cram/test_input_1_a.cram
+-rw-r--r--   0     1001      127   339527 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/fake_fastq_file.fastq.gz
+-rw-r--r--   0     1001      127     1749 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/file.vcf
+-rw-r--r--   0     1001      127     9521 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/index.bcf
+-rw-r--r--   0     1001      127      143 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/index.bcf.csi
+-rw-r--r--   0     1001      127     8638 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/index.vcf.gz
+-rw-r--r--   0     1001      127      213 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/index.vcf.gz.tbi
+-rw-r--r--   0     1001      127       41 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/test.fa
+-rw-r--r--   0     1001      127       55 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/test.fa.gz
+-rw-r--r--   0     1001      127       41 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/test.fasta
+-rw-r--r--   0     1001      127       22 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/test.fasta.fai
+-rw-r--r--   0     1001      127       58 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/test.fasta.gz
+-rw-r--r--   0     1001      127      286 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/test.fastq
+-rw-r--r--   0     1001      127      134 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/test.fastq.gz
+-rw-r--r--   0     1001      127      286 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/test.fq
+-rw-r--r--   0     1001      127      156 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/test.fq.gz
+-rw-r--r--   0     1001      127      112 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/test.gff
+-rw-r--r--   0     1001      127       91 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/test.gff.gz
+-rw-r--r--   0     1001      127    17994 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/test.gtf
+-rw-r--r--   0     1001      127     1478 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/test.gtf.gz
+-rw-r--r--   0     1001      127    17171 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/test.mzML
+-rw-r--r--   0     1001      127     2845 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/test.mzML.gz
+-rw-r--r--   0     1001      127     1025 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/two-cram/rand1k.fa
+-rw-r--r--   0     1001      127       20 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/two-cram/rand1k.fa.fai
+-rw-r--r--   0     1001      127     1029 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/two-cram/twolib.sorted.cram
+-rw-r--r--   0     1001      127       42 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/two-cram/twolib.sorted.cram.crai
+-rw-r--r--   0     1001      127     1669 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/vcf-partition/sample=1/vcf_file.vcf.gz
+-rw-r--r--   0     1001      127      254 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/vcf-partition/sample=1/vcf_file.vcf.gz.tbi
+-rw-r--r--   0     1001      127     4302 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/vcf_file.vcf
+-rw-r--r--   0     1001      127     1669 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/vcf_file.vcf.gz
+-rw-r--r--   0     1001      127      254 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/data/vcf_file.vcf.gz.tbi
+-rw-r--r--   0     1001      127    14881 2024-05-23 22:20:00.000000 biobear-0.20.3/python/tests/test_session.py
+-rw-r--r--   0     1001      127       47 2024-05-23 22:20:00.000000 biobear-0.20.3/requirements-dev.txt
+-rw-r--r--   0     1001      127     3705 2024-05-23 22:20:00.000000 biobear-0.20.3/src/bam_reader.rs
+-rw-r--r--   0     1001      127     3590 2024-05-23 22:20:00.000000 biobear-0.20.3/src/bcf_reader.rs
+-rw-r--r--   0     1001      127     1397 2024-05-23 22:20:00.000000 biobear-0.20.3/src/datasources/bam.rs
+-rw-r--r--   0     1001      127     1631 2024-05-23 22:20:00.000000 biobear-0.20.3/src/datasources/bcf.rs
+-rw-r--r--   0     1001      127     1561 2024-05-23 22:20:00.000000 biobear-0.20.3/src/datasources/bed.rs
+-rw-r--r--   0     1001      127     2572 2024-05-23 22:20:00.000000 biobear-0.20.3/src/datasources/bigwig.rs
+-rw-r--r--   0     1001      127     1548 2024-05-23 22:20:00.000000 biobear-0.20.3/src/datasources/cram.rs
+-rw-r--r--   0     1001      127     3265 2024-05-23 22:20:00.000000 biobear-0.20.3/src/datasources/fasta.rs
+-rw-r--r--   0     1001      127     3322 2024-05-23 22:20:00.000000 biobear-0.20.3/src/datasources/fastq.rs
+-rw-r--r--   0     1001      127     1353 2024-05-23 22:20:00.000000 biobear-0.20.3/src/datasources/fcs.rs
+-rw-r--r--   0     1001      127     1380 2024-05-23 22:20:00.000000 biobear-0.20.3/src/datasources/genbank.rs
+-rw-r--r--   0     1001      127     1913 2024-05-23 22:20:00.000000 biobear-0.20.3/src/datasources/gff.rs
+-rw-r--r--   0     1001      127     1476 2024-05-23 22:20:00.000000 biobear-0.20.3/src/datasources/gtf.rs
+-rw-r--r--   0     1001      127     1322 2024-05-23 22:20:00.000000 biobear-0.20.3/src/datasources/hmm_dom_tab.rs
+-rw-r--r--   0     1001      127     1224 2024-05-23 22:20:00.000000 biobear-0.20.3/src/datasources/mod.rs
+-rw-r--r--   0     1001      127     1517 2024-05-23 22:20:00.000000 biobear-0.20.3/src/datasources/mzml.rs
+-rw-r--r--   0     1001      127     1071 2024-05-23 22:20:00.000000 biobear-0.20.3/src/datasources/sam.rs
+-rw-r--r--   0     1001      127     2839 2024-05-23 22:20:00.000000 biobear-0.20.3/src/datasources/vcf.rs
+-rw-r--r--   0     1001      127     2606 2024-05-23 22:20:00.000000 biobear-0.20.3/src/error.rs
+-rw-r--r--   0     1001      127     4634 2024-05-23 22:20:00.000000 biobear-0.20.3/src/execution_result.rs
+-rw-r--r--   0     1001      127     3784 2024-05-23 22:20:00.000000 biobear-0.20.3/src/exon_reader.rs
+-rw-r--r--   0     1001      127     3225 2024-05-23 22:20:00.000000 biobear-0.20.3/src/file_compression_type.rs
+-rw-r--r--   0     1001      127     2706 2024-05-23 22:20:00.000000 biobear-0.20.3/src/lib.rs
+-rw-r--r--   0     1001      127     1247 2024-05-23 22:20:00.000000 biobear-0.20.3/src/runtime.rs
+-rw-r--r--   0     1001      127     9978 2024-05-23 22:20:00.000000 biobear-0.20.3/src/session_context.rs
+-rw-r--r--   0     1001      127     3752 2024-05-23 22:20:00.000000 biobear-0.20.3/src/vcf_reader.rs
+-rw-r--r--   0     1001      127   111360 2024-05-23 22:20:06.000000 biobear-0.20.3/Cargo.lock
+-rw-r--r--   0     1001      127      725 2024-05-23 22:20:00.000000 biobear-0.20.3/pyproject.toml
+-rw-r--r--   0        0        0     8469 1970-01-01 00:00:00.000000 biobear-0.20.3/PKG-INFO
```

### Comparing `biobear-0.20.2/.github/biobear.svg` & `biobear-0.20.3/.github/biobear.svg`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/.github/workflows/release.yml` & `biobear-0.20.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/.github/workflows/smoke-test.yml` & `biobear-0.20.3/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/.github/workflows/test.yml` & `biobear-0.20.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/.gitignore` & `biobear-0.20.3/.gitignore`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/CHANGELOG.md` & `biobear-0.20.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+## v0.20.3 (2024-05-23)
+
 ## v0.20.2 (2024-05-21)
 
 ### Fix
 
 - new exon to fix overflow (#135)
 
 ## v0.20.1 (2024-05-16)
```

### Comparing `biobear-0.20.2/LICENSE` & `biobear-0.20.3/LICENSE`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/README.md` & `biobear-0.20.3/README.md`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/benchmarks/results.json` & `biobear-0.20.3/benchmarks/results.json`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/bin/test.sh` & `biobear-0.20.3/bin/test.sh`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/biobear/__init__.py` & `biobear-0.20.3/python/biobear/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from .biobear import FCSReadOptions
 from .biobear import CRAMReadOptions
 from .biobear import connect
 from .biobear import new_session
 from .biobear import __runtime
 
 
-__version__ = "0.20.2"
+__version__ = "0.20.3"
 
 __all__ = [
     "FastaReader",
     "FastqReader",
     "VCFReader",
     "VCFIndexedReader",
     "BamReader",
```

### Comparing `biobear-0.20.2/python/biobear/bam_reader.py` & `biobear-0.20.3/python/biobear/bam_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/biobear/bcf_reader.py` & `biobear-0.20.3/python/biobear/bcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/biobear/biobear.pyi` & `biobear-0.20.3/python/biobear/biobear.pyi`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/biobear/compression.py` & `biobear-0.20.3/python/biobear/compression.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/biobear/fasta_reader.py` & `biobear-0.20.3/python/biobear/fasta_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/biobear/fastq_reader.py` & `biobear-0.20.3/python/biobear/fastq_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/biobear/genbank_reader.py` & `biobear-0.20.3/python/biobear/genbank_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/biobear/gff_reader.py` & `biobear-0.20.3/python/biobear/gff_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/biobear/gtf_reader.py` & `biobear-0.20.3/python/biobear/gtf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/biobear/mzml_reader.py` & `biobear-0.20.3/python/biobear/mzml_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/biobear/reader.py` & `biobear-0.20.3/python/biobear/reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/biobear/vcf_reader.py` & `biobear-0.20.3/python/biobear/vcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/BGC0000404.gbk` & `biobear-0.20.3/python/tests/data/BGC0000404.gbk`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/bedcov.bam` & `biobear-0.20.3/python/tests/data/bedcov.bam`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/bedcov.bam.bai` & `biobear-0.20.3/python/tests/data/bedcov.bam.bai`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/cram/0500_mapped.cram` & `biobear-0.20.3/python/tests/data/cram/0500_mapped.cram`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/cram/1404_index_multislice.cram` & `biobear-0.20.3/python/tests/data/cram/1404_index_multislice.cram`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/cram/ce.fa` & `biobear-0.20.3/python/tests/data/cram/ce.fa`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/cram/test_input_1_a.cram` & `biobear-0.20.3/python/tests/data/cram/test_input_1_a.cram`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/fake_fastq_file.fastq.gz` & `biobear-0.20.3/python/tests/data/fake_fastq_file.fastq.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/file.vcf` & `biobear-0.20.3/python/tests/data/file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/index.bcf` & `biobear-0.20.3/python/tests/data/index.bcf`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/index.vcf.gz` & `biobear-0.20.3/python/tests/data/index.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/test.gtf` & `biobear-0.20.3/python/tests/data/test.gtf`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/test.gtf.gz` & `biobear-0.20.3/python/tests/data/test.gtf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/test.mzML` & `biobear-0.20.3/python/tests/data/test.mzML`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/test.mzML.gz` & `biobear-0.20.3/python/tests/data/test.mzML.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/two-cram/rand1k.fa` & `biobear-0.20.3/python/tests/data/two-cram/rand1k.fa`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/two-cram/twolib.sorted.cram` & `biobear-0.20.3/python/tests/data/two-cram/twolib.sorted.cram`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/vcf-partition/sample=1/vcf_file.vcf.gz` & `biobear-0.20.3/python/tests/data/vcf-partition/sample=1/vcf_file.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/vcf_file.vcf` & `biobear-0.20.3/python/tests/data/vcf_file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/data/vcf_file.vcf.gz` & `biobear-0.20.3/python/tests/data/vcf_file.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/python/tests/test_session.py` & `biobear-0.20.3/python/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/bam_reader.rs` & `biobear-0.20.3/src/bam_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/bcf_reader.rs` & `biobear-0.20.3/src/bcf_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/datasources/bam.rs` & `biobear-0.20.3/src/datasources/bam.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/datasources/bcf.rs` & `biobear-0.20.3/src/datasources/bcf.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/datasources/bed.rs` & `biobear-0.20.3/src/datasources/bed.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/datasources/bigwig.rs` & `biobear-0.20.3/src/datasources/bigwig.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/datasources/cram.rs` & `biobear-0.20.3/src/datasources/cram.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/datasources/fasta.rs` & `biobear-0.20.3/src/datasources/fasta.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/datasources/fastq.rs` & `biobear-0.20.3/src/datasources/fastq.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/datasources/fcs.rs` & `biobear-0.20.3/src/datasources/fcs.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/datasources/genbank.rs` & `biobear-0.20.3/src/datasources/genbank.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/datasources/gff.rs` & `biobear-0.20.3/src/datasources/gff.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/datasources/gtf.rs` & `biobear-0.20.3/src/datasources/gtf.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/datasources/hmm_dom_tab.rs` & `biobear-0.20.3/src/datasources/hmm_dom_tab.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/datasources/mod.rs` & `biobear-0.20.3/src/datasources/mod.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/datasources/mzml.rs` & `biobear-0.20.3/src/datasources/mzml.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/datasources/sam.rs` & `biobear-0.20.3/src/datasources/sam.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/datasources/vcf.rs` & `biobear-0.20.3/src/datasources/vcf.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/error.rs` & `biobear-0.20.3/src/error.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/execution_result.rs` & `biobear-0.20.3/src/execution_result.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/exon_reader.rs` & `biobear-0.20.3/src/exon_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/file_compression_type.rs` & `biobear-0.20.3/src/file_compression_type.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/lib.rs` & `biobear-0.20.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/runtime.rs` & `biobear-0.20.3/src/runtime.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/session_context.rs` & `biobear-0.20.3/src/session_context.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/src/vcf_reader.rs` & `biobear-0.20.3/src/vcf_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.2/Cargo.lock` & `biobear-0.20.3/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -415,17 +415,17 @@
 name = "autocfg"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "aws-config"
-version = "1.4.0"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "40ddbfb5db93d62521f47b3f223da0884a2f02741ff54cb9cda192a0e73ba08b"
+checksum = "1234b742ac4a40a7d3459c6e3c99818271976a5a6ae3732cb415f4a9a94da7b6"
 dependencies = [
  "aws-credential-types",
  "aws-runtime",
  "aws-sdk-sso",
  "aws-sdk-ssooidc",
  "aws-sdk-sts",
  "aws-smithy-async",
@@ -481,17 +481,17 @@
  "pin-project-lite",
  "tracing",
  "uuid",
 ]
 
 [[package]]
 name = "aws-sdk-sso"
-version = "1.25.0"
+version = "1.27.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fef2d9ca2b43051224ed326ed9960a85e277b7d554a2cd0397e57c0553d86e64"
+checksum = "aef53f254e16c00cfbfd69fa6eca4d858b7c161878db2cd248410af402d1951e"
 dependencies = [
  "aws-credential-types",
  "aws-runtime",
  "aws-smithy-async",
  "aws-smithy-http",
  "aws-smithy-json",
  "aws-smithy-runtime",
@@ -503,17 +503,17 @@
  "once_cell",
  "regex-lite",
  "tracing",
 ]
 
 [[package]]
 name = "aws-sdk-ssooidc"
-version = "1.26.0"
+version = "1.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c869d1f5c4ee7437b79c3c1664ddbf7a60231e893960cf82b2b299a5ccf2cc5d"
+checksum = "d1b673b2972c38463955e27d76c9d2ebb0452a9ce8059a0e2c9ed67efe69ef35"
 dependencies = [
  "aws-credential-types",
  "aws-runtime",
  "aws-smithy-async",
  "aws-smithy-http",
  "aws-smithy-json",
  "aws-smithy-runtime",
@@ -525,17 +525,17 @@
  "once_cell",
  "regex-lite",
  "tracing",
 ]
 
 [[package]]
 name = "aws-sdk-sts"
-version = "1.25.0"
+version = "1.27.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e2b4a632a59e4fab7abf1db0d94a3136ad7871aba46bebd1fdb95c7054afcdb"
+checksum = "0d461680731ce37d14396ceeb4ef326998bf9c848123f93a6191958ecd7f6cc0"
 dependencies = [
  "aws-credential-types",
  "aws-runtime",
  "aws-smithy-async",
  "aws-smithy-http",
  "aws-smithy-json",
  "aws-smithy-query",
@@ -621,17 +621,17 @@
 dependencies = [
  "aws-smithy-types",
  "urlencoding",
 ]
 
 [[package]]
 name = "aws-smithy-runtime"
-version = "1.5.0"
+version = "1.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c9ac79e9f3a4d576f3cd4a470a0275b138d9e7b11b1cd514a6858ae0a79dd5bb"
+checksum = "607e8b53aeb2bc23fb332159d72a69650cd9643c161d76cd3b7f88ac00b5a1bb"
 dependencies = [
  "aws-smithy-async",
  "aws-smithy-http",
  "aws-smithy-runtime-api",
  "aws-smithy-types",
  "bytes",
  "fastrand",
@@ -647,34 +647,34 @@
  "rustls",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "aws-smithy-runtime-api"
-version = "1.6.0"
+version = "1.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04ec42c2f5c0e7796a2848dde4d9f3bf8ce12ccbb3d5aa40c52fa0cdd61a1c47"
+checksum = "5b7d790d553d163c7d80a4e06e2906bf24b9172c9ebe045fc3a274e9358ab7bb"
 dependencies = [
  "aws-smithy-async",
  "aws-smithy-types",
  "bytes",
  "http 0.2.12",
  "http 1.1.0",
  "pin-project-lite",
  "tokio",
  "tracing",
  "zeroize",
 ]
 
 [[package]]
 name = "aws-smithy-types"
-version = "1.1.9"
+version = "1.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "baf98d97bba6ddaba180f1b1147e202d8fe04940403a95a3f826c790f931bbd1"
+checksum = "5b6764ba7e1c5ede1c9f9e4046645534f06c2581402461c559b481a420330a83"
 dependencies = [
  "base64-simd",
  "bytes",
  "bytes-utils",
  "http 0.2.12",
  "http 1.1.0",
  "http-body 0.4.6",
@@ -696,17 +696,17 @@
 checksum = "d123fbc2a4adc3c301652ba8e149bf4bc1d1725affb9784eb20c953ace06bf55"
 dependencies = [
  "xmlparser",
 ]
 
 [[package]]
 name = "aws-types"
-version = "1.2.1"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a807d90cd50a969b3d95e4e7ad1491fcae13c6e83948d8728363ecc09d66343a"
+checksum = "02fa328e19c849b20ef7ada4c9b581dd12351ff35ecc7642d06e69de4f98407c"
 dependencies = [
  "aws-credential-types",
  "aws-smithy-async",
  "aws-smithy-runtime-api",
  "aws-smithy-types",
  "http 0.2.12",
  "rustc_version",
@@ -783,15 +783,15 @@
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "biobear"
-version = "0.20.2"
+version = "0.20.3"
 dependencies = [
  "arrow",
  "datafusion",
  "exon",
  "noodles",
  "pyo3",
  "tokio",
@@ -1545,17 +1545,17 @@
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "exon"
-version = "0.21.1"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4db976195ae0c60902a35065692958c67abb20eb229687bd657d066b87009be"
+checksum = "4af8bca51561989e6db2fd199d61a1d60a5660a2c49e4cc84fcb9e9c0eb1dc93"
 dependencies = [
  "arrow",
  "async-trait",
  "bytes",
  "coitrees",
  "datafusion",
  "exon-bam",
@@ -1589,212 +1589,212 @@
  "tracing",
  "tracing-subscriber",
  "url",
 ]
 
 [[package]]
 name = "exon-bam"
-version = "0.21.1"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd9b95b31b8d8a6bbe37aa64303a03136d1035ec7185b1a44914f22e5f1be7a0"
+checksum = "9e18aa81cf5781f5fa801cf2ae005ceccfcd89f67225fdd2161f3022ef501e94"
 dependencies = [
  "arrow",
  "exon-common",
  "exon-sam",
  "futures",
  "itertools 0.13.0",
  "noodles",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-bcf"
-version = "0.21.1"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da121f3b2c602eeece0b1d44f3a9cf838f71618a7e754151196e6c32c4ab129f"
+checksum = "2d373eea49a7c378d490003cc08e17266698a7d60d9908a8236b56158a1faf7d"
 dependencies = [
  "arrow",
  "exon-common",
  "exon-vcf",
  "futures",
  "noodles",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-bed"
-version = "0.21.1"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4799af616d89b424450e286914043469d8eaeafd9fb23287cba9aaa877a4124"
+checksum = "2c6c0423d9ef74c12add2416f643287c21b29a6d1a32ec161606497bc2c5d581"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "exon-bigwig"
-version = "0.21.1"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06399ae57ddff134f0db19dfd3f96e385993cc15768942c62736ea29d9b1f409"
+checksum = "8d407792af98eed9789f4104c01a588ba8278739c8df573098c6b2b379334da9"
 dependencies = [
  "arrow",
  "bigtools",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "exon-common"
-version = "0.21.1"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae04f53aef64634ffbc45dc0dafd2e5fb5f30eaece28b8f206bc1e5c756058a8"
+checksum = "68a26591c155f4f049ef40d21babd32f0f8c8d0b087eab388585f6978cd1418d"
 dependencies = [
  "arrow",
  "datafusion",
  "futures",
  "glob",
  "object_store",
  "url",
 ]
 
 [[package]]
 name = "exon-cram"
-version = "0.21.1"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb3e4efc7df09ce07d638c1eeed3c2ac34faf33e48f5e52911d26eee78137ad"
+checksum = "6af32ed7e428397c0b7b7ebadc991ec38b3643bf26b44109d5d5c77620ec7413"
 dependencies = [
  "arrow",
  "coitrees",
  "exon-common",
  "exon-sam",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "exon-fasta"
-version = "0.21.1"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1930a9127842fc218e959c70a48f2235f38e532207abaa607bbf509563320348"
+checksum = "280a7c270ed1ea3b02205266041a34706133e1f59d532ef00f1dc2eb2efb6339"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "exon-fastq"
-version = "0.21.1"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44e0d93b39464c0a7985912ee5746bd54e6b543daed969ae1a6e278c2bc8d860"
+checksum = "8a2a283ea6efca2aaa695f4190fa87bfd24616190bbd51b9a80f9df9a5bb9c7a"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "exon-fcs"
-version = "0.21.1"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d62b7c4b6fecfcb32981e7a9b2156dee12efa7fefbcfb89a6cc5802919248c5b"
+checksum = "bf7dcdf258cd28c371aecd0c9f0e94313495548a24196738e1476735f9b49cc1"
 dependencies = [
  "arrow",
  "byteorder",
  "exon-common",
  "futures",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-genbank"
-version = "0.21.1"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d9c74945da538f254aa5c2f35680ae9dfcb25d9fd90df8ed011bf339d34fdb7"
+checksum = "f9e4f2fb4c1c323c536fb84c727eecfae244821d2bfcea693831e4121b7c6707"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "gb-io",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-gff"
-version = "0.21.1"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4ff0a1b56a57230a09344cf9f4c0eb390a70631d973decb1797d9f77c8a05fc3"
+checksum = "1da08945e833eed06154d5c45e7541f21b0c5f123aecf88449b2b1b167595a2c"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "noodles-gff",
  "object_store",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "exon-gtf"
-version = "0.21.1"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cace0693f2a5df616b290eb22315ace0f8b85cb98eb48290bc05412d73ebacc9"
+checksum = "a8f8af70985dfc08d881ef4b8ec65925b32050b9942c5ec55180fee03742d98f"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-io"
-version = "0.21.1"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93751b18742c4562f6a7b297db4a0af448b9781b66e7002b6fcefe3c26658ad6"
+checksum = "2f72e2d01f942968a17972c9e84036d5e4746cb94ec98dff1db3e2b4aff06377"
 dependencies = [
  "async-trait",
  "aws-config",
  "aws-credential-types",
  "object_store",
  "tokio",
  "url",
 ]
 
 [[package]]
 name = "exon-mzml"
-version = "0.21.1"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4877eaba359662d2934dffce0342e0cfd85a973e4f39b9810e5c2f3bd26b806c"
+checksum = "226e62e3fa40a87dbc0a1524fcdb1c22cc64749ea5f6daea8d39b8cbd7f15cd3"
 dependencies = [
  "arrow",
  "base64 0.22.1",
  "byteorder",
  "exon-common",
  "flate2",
  "futures",
@@ -1802,32 +1802,32 @@
  "quick-xml",
  "serde",
  "tokio",
 ]
 
 [[package]]
 name = "exon-sam"
-version = "0.21.1"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "afc3ce5645b3a32ea71eea35a9ca8db98baebfde644505cdb926214b44929897"
+checksum = "153316c6343b033fea32f3b75f4bfcb97f4df87b1bc1af17775d34a90c992284"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "itertools 0.13.0",
  "noodles",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-vcf"
-version = "0.21.1"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f7a856ac28fe0d4d119a61b03acae4a5458c66e52cfa0d5b44a911f59cca9bf3"
+checksum = "bd4803e4134523c7b447ca37c5563d6d1da7f9af7cbcc7edcd967586cd8c3df2"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
```

### Comparing `biobear-0.20.2/pyproject.toml` & `biobear-0.20.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 dependencies = ["pyarrow>=15"]
 license = { file = "LICENSE" }
 name = "biobear"
 readme = "README.md"
 requires-python = ">=3.8"
 description = "A package for working with Bioinformatics data with SQL and Arrow"
 summary = "A package for working with Bioinformatics data with SQL and Arrow"
-version = "0.20.2"
+version = "0.20.3"
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 python-source = "python"
```

### Comparing `biobear-0.20.2/PKG-INFO` & `biobear-0.20.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: biobear
-Version: 0.20.2
+Version: 0.20.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pyarrow >=15
 License-File: LICENSE
 Summary: A package for working with Bioinformatics data with SQL and Arrow
 Author-email: WHERE TRUE devs <thauck+biobear@wheretrue.com>
```

