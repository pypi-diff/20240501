# Comparing `tmp/nci_cidc_schemas-0.26.32.tar.gz` & `tmp/nci_cidc_schemas-0.26.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nci_cidc_schemas-0.26.32.tar", last modified: Mon Apr 29 19:04:33 2024, max compression
+gzip compressed data, was "nci_cidc_schemas-0.26.33.tar", last modified: Wed May  1 18:15:44 2024, max compression
```

## Comparing `nci_cidc_schemas-0.26.32.tar` & `nci_cidc_schemas-0.26.33.tar`

### file list

```diff
@@ -1,264 +1,264 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.343147 nci_cidc_schemas-0.26.32/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-29 19:04:33.343147 nci_cidc_schemas-0.26.32/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.295146 nci_cidc_schemas-0.26.32/cidc_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    20035 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/json_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.295146 nci_cidc_schemas-0.26.32/cidc_schemas/metaschema/
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/metaschema/strict_meta_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    14766 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/migrations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.299146 nci_cidc_schemas-0.26.32/cidc_schemas/pipeline_configs/
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/pipeline_configs/rna_level1_analysis_config.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.299146 nci_cidc_schemas-0.26.32/cidc_schemas/prism/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/prism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/prism/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    19294 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/prism/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/prism/extra_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    12431 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/prism/merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    33532 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/prism/pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.299146 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/aliquot.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.307146 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_bam.json
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_bam_bai.json
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_bed.json
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_bigwig.json
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_clinical_csv.json
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_clinical_docx.json
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_clinical_xlsx.json
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_cncf.json
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_cns.json
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_core.json
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_csv.json
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_elisa_xlsx.json
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_fastq_gz.json
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_fcs.json
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_file.json
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_gz.json
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_image.json
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_jpg.json
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_json.json
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_junction.json
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_log.json
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_maf.json
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_narrowPeak.json
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_npx.json
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_pdf.json
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_png.json
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_rcc.json
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_rdata.json
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_tbi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_text.json
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_tsv.json
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_vcf.json
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_vcf_gz.json
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_xlsx.json
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_yaml.json
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_zip.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.311147 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/atacseq_assay.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.315147 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/antibody.json
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/assay_core.json
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/available_assays.json
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/available_ngs_analyses.json
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/composite_image.json
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/controls.json
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/enrichment_core.json
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/excluded_samples.json
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/image.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.315147 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging/mif_entry.json
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging/mif_export.json
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging/mif_input.json
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging/mif_roi.json
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging_data.json
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/local_file.json
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/mapping.json
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/mibi_antibody.json
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/mif_antibody.json
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/multiple_local_files.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.315147 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.315147 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/atacseq/
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/atacseq/atacseq_analysis.json
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/ngs_assay_record.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.319147 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/fusion.json
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/microbiome.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/msisensor.json
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/neoantigen.json
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/rna_analysis.json
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/rna_level1_analysis.json
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/rseqc.json
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/salmon.json
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/star.json
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/trust4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs_assay_core.json
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs_assay_record.json
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/reads_core.json
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/reads_with_index.json
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/ctdna_analysis.json
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/ctdna_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/cytof_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/cytof_assay_core.json
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/elisa_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/hande_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/ihc_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/mibi_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/microbiome_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/mif_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/misc_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/nanostring_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/olink_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/rna_assay-v0.json
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/rna_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/tcr_analysis.json
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/tcr_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/wes_analysis.json
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/wes_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)    12858 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/wes_core.json
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/wes_tumor_only_analysis.json
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/clinical_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/clinical_trial.json
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/participant.json
--rw-r--r--   0 runner    (1001) docker     (127)    16296 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/sample.json
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/shipping_core.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.291146 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.319147 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/atacseq_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/ctdna_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/cytof_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/rna_level1_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/tcr_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/wes_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    16240 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/wes_tumor_only_analysis_template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.323147 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/atacseq_fastq_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/clinical_data_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/ctdna_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    13328 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/cytof_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/elisa_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/hande_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/ihc_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/mibi_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/microbiome_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    19272 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/mif_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/misc_data_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/nanostring_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/olink_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/rna_bam_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/rna_fastq_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/tcr_adaptive_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/tcr_fastq_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/wes_bam_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/wes_fastq_template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.327147 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/h_and_e_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/microbiome_dna_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    13346 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/normal_blood_dna_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    12989 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/normal_tissue_dna_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/pbmc_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/plasma_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    11024 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/tissue_slide_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/tumor_normal_pairing_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    13276 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/tumor_tissue_dna_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/tumor_tissue_rna_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    49891 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/template_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    18236 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/template_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/unprism.py
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.343147 nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-29 19:04:33.000000 nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10838 2024-04-29 19:04:33.000000 nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:04:33.000000 nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-29 19:04:33.000000 nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:04:33.000000 nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-29 19:04:33.000000 nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 19:04:33.000000 nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-29 19:04:33.343147 nci_cidc_schemas-0.26.32/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.331147 nci_cidc_schemas-0.26.32/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.335147 nci_cidc_schemas-0.26.32/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.1.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.1.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.2.bom.csv
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.2.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.2.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.3.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.docx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.335147 nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/
--rw-r--r--   0 runner    (1001) docker     (127)    19111 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_1.json
--rw-r--r--   0 runner    (1001) docker     (127)    24203 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_1PA_multiWES.json
--rw-r--r--   0 runner    (1001) docker     (127)    14837 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_cytof_with_analysis.json
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_ihc.json
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_minimal.json
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/date_examples.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/elisa_test_file.1.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/elisa_test_file.2.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    26605 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/hande_err_template.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.335147 nci_cidc_schemas-0.26.32/tests/data/olink/
--rw-r--r--   0 runner    (1001) docker     (127)    13070 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/olink/invalid_olink_assay_1_NPX.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    17905 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/olink/olink_assay_1_NPX.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    12969 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/olink/olink_assay_2_NPX.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    21276 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/olink/olink_assay_combined.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    13301 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/pbmc_invalid.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.335147 nci_cidc_schemas-0.26.32/tests/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/1.json
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/a.json
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/b.json
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/c.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.335147 nci_cidc_schemas-0.26.32/tests/data/schemas/d1/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/d1/3.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.335147 nci_cidc_schemas-0.26.32/tests/data/schemas/d1/d2/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/d1/d2/2.json
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/invalid_ref.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.339147 nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/atacseq_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/ctdna_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    12507 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/rna_level1_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    35065 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/wes_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    16256 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/wes_tumor_only_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/tiny_invalid_manifest.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/tiny_valid_manifest.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.339147 nci_cidc_schemas-0.26.32/tests/prism/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.343147 nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   146616 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/analysis_data.py
--rw-r--r--   0 runner    (1001) docker     (127)   167922 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/assay_data.py
--rw-r--r--   0 runner    (1001) docker     (127)   104350 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/manifest_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.343147 nci_cidc_schemas-0.26.32/tests/prism/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/schema/test_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/test_cidc_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    31916 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/test_extra_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    13867 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/test_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    29150 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    17706 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_assays.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_clinicaltrial_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)    14541 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_json_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_strict_meta_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    26123 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_template_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_template_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_trial_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_unprism.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.343147 nci_cidc_schemas-0.26.32/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/utils/test_template_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.635250 nci_cidc_schemas-0.26.33/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-01 18:15:44.635250 nci_cidc_schemas-0.26.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.587250 nci_cidc_schemas-0.26.33/cidc_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20035 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/json_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.587250 nci_cidc_schemas-0.26.33/cidc_schemas/metaschema/
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/metaschema/strict_meta_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14766 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.587250 nci_cidc_schemas-0.26.33/cidc_schemas/pipeline_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/pipeline_configs/rna_level1_analysis_config.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.587250 nci_cidc_schemas-0.26.33/cidc_schemas/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/prism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/prism/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19294 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/prism/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/prism/extra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12431 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/prism/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33532 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/prism/pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.591250 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/aliquot.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.599250 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_bam.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_bam_bai.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_bed.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_bigwig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_clinical_csv.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_clinical_docx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_clinical_xlsx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_cncf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_cns.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_core.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_csv.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_elisa_xlsx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_fastq_gz.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_fcs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_gz.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_image.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_jpg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_json.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_junction.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_log.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_maf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_narrowPeak.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_npx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_pdf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_png.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_rcc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_rdata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_tbi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_text.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_tsv.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_vcf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_vcf_gz.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_xlsx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_yaml.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_zip.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.603250 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/atacseq_assay.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.607250 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/antibody.json
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/assay_core.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/available_assays.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/available_ngs_analyses.json
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/composite_image.json
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/controls.json
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/enrichment_core.json
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/excluded_samples.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/image.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.607250 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/imaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/imaging/mif_entry.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/imaging/mif_export.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/imaging/mif_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/imaging/mif_roi.json
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/imaging_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/local_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/mapping.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/mibi_antibody.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/mif_antibody.json
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/multiple_local_files.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.607250 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.607250 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/atacseq/
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/atacseq/atacseq_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/ngs_assay_record.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.607250 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/rna/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/rna/fusion.json
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/rna/microbiome.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/rna/msisensor.json
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/rna/neoantigen.json
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/rna/rna_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/rna/rna_level1_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/rna/rseqc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/rna/salmon.json
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/rna/star.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/rna/trust4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs_assay_core.json
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs_assay_record.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/reads_core.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/reads_with_index.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/ctdna_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/ctdna_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/cytof_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/cytof_assay_core.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/elisa_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/hande_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/ihc_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/mibi_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/microbiome_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/mif_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/misc_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/nanostring_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/olink_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/rna_assay-v0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/rna_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/tcr_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/tcr_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/wes_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/wes_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12858 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/wes_core.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/wes_tumor_only_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/clinical_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/clinical_trial.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/participant.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16296 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/shipping_core.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.583250 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.611250 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/analyses/
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/analyses/atacseq_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/analyses/ctdna_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/analyses/cytof_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/analyses/rna_level1_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/analyses/tcr_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/analyses/wes_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16240 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/analyses/wes_tumor_only_analysis_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.615250 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/atacseq_fastq_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/clinical_data_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/ctdna_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13328 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/cytof_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/elisa_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/hande_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/ihc_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/mibi_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/microbiome_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19272 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/mif_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/misc_data_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/nanostring_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/olink_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/rna_bam_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/rna_fastq_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/tcr_adaptive_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/tcr_fastq_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/wes_bam_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/wes_fastq_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.615250 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/h_and_e_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/microbiome_dna_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13346 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/normal_blood_dna_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12989 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/normal_tissue_dna_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/pbmc_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/plasma_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11024 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/tissue_slide_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/tumor_normal_pairing_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13276 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/tumor_tissue_dna_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/tumor_tissue_rna_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    49891 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/template_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18236 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/template_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/unprism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/cidc_schemas/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.635250 nci_cidc_schemas-0.26.33/nci_cidc_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-01 18:15:44.000000 nci_cidc_schemas-0.26.33/nci_cidc_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10838 2024-05-01 18:15:44.000000 nci_cidc_schemas-0.26.33/nci_cidc_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:15:44.000000 nci_cidc_schemas-0.26.33/nci_cidc_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-01 18:15:44.000000 nci_cidc_schemas-0.26.33/nci_cidc_schemas.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:15:44.000000 nci_cidc_schemas-0.26.33/nci_cidc_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-01 18:15:44.000000 nci_cidc_schemas-0.26.33/nci_cidc_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-01 18:15:44.000000 nci_cidc_schemas-0.26.33/nci_cidc_schemas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-01 18:15:44.635250 nci_cidc_schemas-0.26.33/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.623250 nci_cidc_schemas-0.26.33/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.623250 nci_cidc_schemas-0.26.33/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/clinical_test_file.1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/clinical_test_file.1.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/clinical_test_file.2.bom.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/clinical_test_file.2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/clinical_test_file.2.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/clinical_test_file.3.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/clinical_test_file.docx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.627250 nci_cidc_schemas-0.26.33/tests/data/clinicaltrial_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    19111 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/clinicaltrial_examples/CT_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24203 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/clinicaltrial_examples/CT_1PA_multiWES.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14837 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/clinicaltrial_examples/CT_cytof_with_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/clinicaltrial_examples/CT_ihc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/clinicaltrial_examples/CT_minimal.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/date_examples.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/elisa_test_file.1.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/elisa_test_file.2.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    26605 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/hande_err_template.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.627250 nci_cidc_schemas-0.26.33/tests/data/olink/
+-rw-r--r--   0 runner    (1001) docker     (127)    13070 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/olink/invalid_olink_assay_1_NPX.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    17905 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/olink/olink_assay_1_NPX.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    12969 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/olink/olink_assay_2_NPX.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    21276 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/olink/olink_assay_combined.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    13301 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/pbmc_invalid.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.627250 nci_cidc_schemas-0.26.33/tests/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/schemas/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/schemas/a.json
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/schemas/b.json
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/schemas/c.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.627250 nci_cidc_schemas-0.26.33/tests/data/schemas/d1/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/schemas/d1/3.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.627250 nci_cidc_schemas-0.26.33/tests/data/schemas/d1/d2/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/schemas/d1/d2/2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/schemas/invalid_ref.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.631250 nci_cidc_schemas-0.26.33/tests/data/schemas/target-templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/schemas/target-templates/atacseq_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/schemas/target-templates/ctdna_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12507 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/schemas/target-templates/rna_level1_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35065 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/schemas/target-templates/wes_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16256 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/schemas/target-templates/wes_tumor_only_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/tiny_invalid_manifest.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/data/tiny_valid_manifest.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.631250 nci_cidc_schemas-0.26.33/tests/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/prism/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.635250 nci_cidc_schemas-0.26.33/tests/prism/cidc_test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/prism/cidc_test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   146616 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/prism/cidc_test_data/analysis_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)   166417 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/prism/cidc_test_data/assay_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104350 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/prism/cidc_test_data/manifest_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/prism/cidc_test_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.635250 nci_cidc_schemas-0.26.33/tests/prism/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/prism/schema/test_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/prism/test_cidc_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/prism/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31916 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/prism/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/prism/test_extra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13867 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/prism/test_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29150 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/prism/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17706 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/test_assays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/test_clinicaltrial_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14541 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/test_json_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/test_strict_meta_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26123 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/test_template_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/test_template_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/test_trial_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/test_unprism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:15:44.635250 nci_cidc_schemas-0.26.33/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-01 18:15:38.000000 nci_cidc_schemas-0.26.33/tests/utils/test_template_generator.py
```

### Comparing `nci_cidc_schemas-0.26.32/LICENSE` & `nci_cidc_schemas-0.26.33/LICENSE`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/PKG-INFO` & `nci_cidc_schemas-0.26.33/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci_cidc_schemas
-Version: 0.26.32
+Version: 0.26.33
 Summary: The CIDC data model and tools for working with it.
 Home-page: https://github.com/NCI-CIDC/cidc-schemas
 Author: NCI
 Author-email: nci-cidc-tools-admin@mail.nih.gov
 License: MIT license
 Keywords: cidc_schemas
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nci_cidc_schemas-0.26.32/README.md` & `nci_cidc_schemas-0.26.33/README.md`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/cli.py` & `nci_cidc_schemas-0.26.33/cidc_schemas/cli.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/constants.py` & `nci_cidc_schemas-0.26.33/cidc_schemas/constants.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/json_validation.py` & `nci_cidc_schemas-0.26.33/cidc_schemas/json_validation.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/metaschema/strict_meta_schema.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/metaschema/strict_meta_schema.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/migrations.py` & `nci_cidc_schemas-0.26.33/cidc_schemas/migrations.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/pipeline_configs/rna_level1_analysis_config.yaml.j2` & `nci_cidc_schemas-0.26.33/cidc_schemas/pipeline_configs/rna_level1_analysis_config.yaml.j2`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/prism/__init__.py` & `nci_cidc_schemas-0.26.33/cidc_schemas/prism/__init__.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/prism/constants.py` & `nci_cidc_schemas-0.26.33/cidc_schemas/prism/constants.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/prism/core.py` & `nci_cidc_schemas-0.26.33/cidc_schemas/prism/core.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/prism/extra_metadata.py` & `nci_cidc_schemas-0.26.33/cidc_schemas/prism/extra_metadata.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/prism/merger.py` & `nci_cidc_schemas-0.26.33/cidc_schemas/prism/merger.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/prism/pipelines.py` & `nci_cidc_schemas-0.26.33/cidc_schemas/prism/pipelines.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/aliquot.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/aliquot.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_bam.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_bam.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_bam_bai.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_bam_bai.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_bed.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_bed.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_bigwig.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_bigwig.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_binary.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_binary.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_clinical_csv.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_clinical_csv.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_clinical_docx.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_clinical_docx.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_clinical_xlsx.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_clinical_xlsx.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_cncf.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_cncf.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_cns.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_cns.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_core.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_csv.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_csv.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_elisa_xlsx.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_elisa_xlsx.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_fastq_gz.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_fastq_gz.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_fcs.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_fcs.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_file.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_file.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_gz.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_gz.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_image.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_image.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_jpg.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_jpg.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_json.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_json.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_junction.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_junction.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_log.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_log.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_maf.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_maf.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_narrowPeak.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_narrowPeak.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_npx.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_npx.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_pdf.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_pdf.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_png.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_png.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_rcc.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_rcc.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_rdata.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_rdata.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_tbi.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_tbi.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_text.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_text.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_tsv.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_tsv.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_vcf.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_vcf.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_vcf_gz.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_vcf_gz.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_xlsx.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_xlsx.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_yaml.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_yaml.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_zip.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/artifacts/artifact_zip.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/atacseq_assay.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/atacseq_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/antibody.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/antibody.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/available_assays.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/available_assays.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/available_ngs_analyses.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/available_ngs_analyses.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/composite_image.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/composite_image.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/enrichment_core.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/enrichment_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/excluded_samples.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/excluded_samples.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/image.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/image.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging/mif_entry.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/imaging/mif_entry.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging/mif_export.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/imaging/mif_export.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging/mif_input.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/imaging/mif_input.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging/mif_roi.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/imaging/mif_roi.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging_data.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/imaging_data.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/mapping.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/mapping.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/mibi_antibody.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/mibi_antibody.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/mif_antibody.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/mif_antibody.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/atacseq/atacseq_analysis.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/atacseq/atacseq_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/ngs_assay_record.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/ngs_assay_record.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/rna_analysis.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/rna/rna_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/rna_level1_analysis.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/rna/rna_level1_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/rseqc.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/rna/rseqc.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/salmon.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/rna/salmon.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/star.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs/rna/star.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs_assay_core.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs_assay_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs_assay_record.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/ngs_assay_record.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/reads_core.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/reads_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/reads_with_index.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/components/reads_with_index.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/ctdna_analysis.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/ctdna_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/ctdna_assay.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/ctdna_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/cytof_assay.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/cytof_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/cytof_assay_core.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/cytof_assay_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/elisa_assay.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/elisa_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/hande_assay.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/hande_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/ihc_assay.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/ihc_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/mibi_assay.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/mibi_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/microbiome_assay.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/microbiome_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/mif_assay.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/mif_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/misc_data.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/misc_data.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/nanostring_assay.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/nanostring_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/olink_assay.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/olink_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/rna_assay-v0.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/rna_assay-v0.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/tcr_analysis.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/tcr_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/tcr_assay.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/tcr_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/wes_analysis.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/wes_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/wes_assay.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/wes_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/wes_core.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/wes_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/wes_tumor_only_analysis.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/assays/wes_tumor_only_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/clinical_data.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/clinical_data.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/clinical_trial.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/clinical_trial.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/participant.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/participant.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/sample.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/sample.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/shipping_core.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/shipping_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/atacseq_analysis_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/analyses/atacseq_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/ctdna_analysis_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/analyses/ctdna_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/cytof_analysis_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/analyses/cytof_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/rna_level1_analysis_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/analyses/rna_level1_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/tcr_analysis_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/analyses/tcr_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/wes_analysis_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/analyses/wes_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/wes_tumor_only_analysis_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/analyses/wes_tumor_only_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/atacseq_fastq_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/atacseq_fastq_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/clinical_data_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/clinical_data_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/ctdna_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/ctdna_template.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999632352941177%*

 * *Differences: {"'properties'": "{'worksheets': {'ctDNA': {'data_columns': {'Samples': {'on premise corrected "*

 * *                 "depth file': {'allow_empty': True}, 'on premise parameters file': "*

 * *                 "{'allow_empty': True}, 'on premise rdata file': {'allow_empty': True}}}}}}"}*

```diff
@@ -47,26 +47,29 @@
                         "genome-wide plots": {
                             "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/genome-wide_plots.pdf",
                             "is_artifact": 1,
                             "merge_pointer": "0/genome-wide_plots",
                             "type_ref": "assays/components/local_file.json#properties/file_path"
                         },
                         "on premise corrected depth file": {
+                            "allow_empty": true,
                             "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/OnPrem.correctedDepth.txt",
                             "is_artifact": 1,
                             "merge_pointer": "0/on_premise_corrected_depth_file",
                             "type_ref": "assays/components/local_file.json#properties/file_path"
                         },
                         "on premise parameters file": {
+                            "allow_empty": true,
                             "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/OnPrem.params.txt",
                             "is_artifact": 1,
                             "merge_pointer": "0/on_premise_parameters_file",
                             "type_ref": "assays/components/local_file.json#properties/file_path"
                         },
                         "on premise rdata file": {
+                            "allow_empty": true,
                             "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/OnPrem.RData",
                             "is_artifact": 1,
                             "merge_pointer": "0/on_premise_rdata_file",
                             "type_ref": "assays/components/local_file.json#properties/file_path"
                         },
                         "optimal solution": {
                             "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/optimal_solution.zip",
```

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/cytof_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/cytof_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/elisa_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/elisa_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/hande_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/hande_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/ihc_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/ihc_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/mibi_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/mibi_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/microbiome_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/microbiome_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/mif_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/mif_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/misc_data_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/misc_data_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/nanostring_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/nanostring_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/olink_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/olink_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/rna_bam_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/rna_bam_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/rna_fastq_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/rna_fastq_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/tcr_adaptive_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/tcr_adaptive_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/tcr_fastq_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/tcr_fastq_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/wes_bam_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/wes_bam_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/wes_fastq_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/assays/wes_fastq_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/h_and_e_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/h_and_e_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/microbiome_dna_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/microbiome_dna_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/normal_blood_dna_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/normal_blood_dna_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/normal_tissue_dna_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/normal_tissue_dna_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/pbmc_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/pbmc_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/plasma_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/plasma_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/tissue_slide_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/tissue_slide_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/tumor_normal_pairing_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/tumor_normal_pairing_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/tumor_tissue_dna_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/tumor_tissue_dna_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/tumor_tissue_rna_template.json` & `nci_cidc_schemas-0.26.33/cidc_schemas/schemas/templates/manifests/tumor_tissue_rna_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/template.py` & `nci_cidc_schemas-0.26.33/cidc_schemas/template.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/template_reader.py` & `nci_cidc_schemas-0.26.33/cidc_schemas/template_reader.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/template_writer.py` & `nci_cidc_schemas-0.26.33/cidc_schemas/template_writer.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/unprism.py` & `nci_cidc_schemas-0.26.33/cidc_schemas/unprism.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/cidc_schemas/util.py` & `nci_cidc_schemas-0.26.33/cidc_schemas/util.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/PKG-INFO` & `nci_cidc_schemas-0.26.33/nci_cidc_schemas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci_cidc_schemas
-Version: 0.26.32
+Version: 0.26.33
 Summary: The CIDC data model and tools for working with it.
 Home-page: https://github.com/NCI-CIDC/cidc-schemas
 Author: NCI
 Author-email: nci-cidc-tools-admin@mail.nih.gov
 License: MIT license
 Keywords: cidc_schemas
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/SOURCES.txt` & `nci_cidc_schemas-0.26.33/nci_cidc_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/setup.py` & `nci_cidc_schemas-0.26.33/setup.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/conftest.py` & `nci_cidc_schemas-0.26.33/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.1.xlsx` & `nci_cidc_schemas-0.26.33/tests/data/clinical_test_file.1.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.2.xlsx` & `nci_cidc_schemas-0.26.33/tests/data/clinical_test_file.2.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.3.xlsx` & `nci_cidc_schemas-0.26.33/tests/data/clinical_test_file.3.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.docx` & `nci_cidc_schemas-0.26.33/tests/data/clinical_test_file.docx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_1.json` & `nci_cidc_schemas-0.26.33/tests/data/clinicaltrial_examples/CT_1.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_1PA_multiWES.json` & `nci_cidc_schemas-0.26.33/tests/data/clinicaltrial_examples/CT_1PA_multiWES.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_cytof_with_analysis.json` & `nci_cidc_schemas-0.26.33/tests/data/clinicaltrial_examples/CT_cytof_with_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_ihc.json` & `nci_cidc_schemas-0.26.33/tests/data/clinicaltrial_examples/CT_ihc.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_minimal.json` & `nci_cidc_schemas-0.26.33/tests/data/clinicaltrial_examples/CT_minimal.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/date_examples.xlsx` & `nci_cidc_schemas-0.26.33/tests/data/date_examples.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/elisa_test_file.1.xlsx` & `nci_cidc_schemas-0.26.33/tests/data/elisa_test_file.1.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/elisa_test_file.2.xlsx` & `nci_cidc_schemas-0.26.33/tests/data/elisa_test_file.2.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/hande_err_template.xlsx` & `nci_cidc_schemas-0.26.33/tests/data/hande_err_template.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/olink/invalid_olink_assay_1_NPX.xlsx` & `nci_cidc_schemas-0.26.33/tests/data/olink/invalid_olink_assay_1_NPX.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/olink/olink_assay_1_NPX.xlsx` & `nci_cidc_schemas-0.26.33/tests/data/olink/olink_assay_1_NPX.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/olink/olink_assay_2_NPX.xlsx` & `nci_cidc_schemas-0.26.33/tests/data/olink/olink_assay_2_NPX.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/olink/olink_assay_combined.xlsx` & `nci_cidc_schemas-0.26.33/tests/data/olink/olink_assay_combined.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/pbmc_invalid.xlsx` & `nci_cidc_schemas-0.26.33/tests/data/pbmc_invalid.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/atacseq_analysis_template.json` & `nci_cidc_schemas-0.26.33/tests/data/schemas/target-templates/atacseq_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/ctdna_analysis_template.json` & `nci_cidc_schemas-0.26.33/tests/data/schemas/target-templates/ctdna_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/rna_level1_analysis_template.json` & `nci_cidc_schemas-0.26.33/tests/data/schemas/target-templates/rna_level1_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/wes_analysis_template.json` & `nci_cidc_schemas-0.26.33/tests/data/schemas/target-templates/wes_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/wes_tumor_only_analysis_template.json` & `nci_cidc_schemas-0.26.33/tests/data/schemas/target-templates/wes_tumor_only_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/tiny_invalid_manifest.xlsx` & `nci_cidc_schemas-0.26.33/tests/data/tiny_invalid_manifest.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/data/tiny_valid_manifest.xlsx` & `nci_cidc_schemas-0.26.33/tests/data/tiny_valid_manifest.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/analysis_data.py` & `nci_cidc_schemas-0.26.33/tests/prism/cidc_test_data/analysis_data.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/assay_data.py` & `nci_cidc_schemas-0.26.33/tests/prism/cidc_test_data/assay_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -3527,23 +3527,14 @@
                             },
                             "optimal_solution": {
                                 "upload_placeholder": "289068fe-4c00-4a67-9a98-74223266c1e0"
                             },
                             "other_solutions": {
                                 "upload_placeholder": "f63988e4-948d-4d55-8822-600754d5259c"
                             },
-                            "on_premise_corrected_depth_file": {
-                                "upload_placeholder": "4c409c82-dff7-4f78-801c-1222"
-                            },
-                            "on_premise_parameters_file": {
-                                "upload_placeholder": "4c409c82-dff7-4f78-801c-111"
-                            },
-                            "on_premise_rdata_file": {
-                                "upload_placeholder": "4c409c82-dff7-4f78-801c-323fff"
-                            },
                             "fraction_cna_subclonal": 0.2,
                             "fraction_genome_subclonal": 0.3,
                             "gc_map_correction_mad": 0.05,
                             "subclone_fraction": 0.16,
                             "tumor_fraction": 0.26,
                             "tumor_ploidy": 2.699,
                             "comments": "note about sample 2",
@@ -3600,49 +3591,28 @@
             local_path="CTTTPP111.00/OnPrem.correctedDepth.txt",
             upload_placeholder="4c409c82-dff7-4f78-801c-11ddf",
             gs_key="test_prism_trial_id/ctdna/test_batch/CTTTPP111.00/OnPrem.correctedDepth.txt",
             metadata_availability=False,
             allow_empty=False,
         ),
         LocalFileUploadEntry(
-            local_path="CTTTPP121.00/OnPrem.correctedDepth.txt",
-            upload_placeholder="4c409c82-dff7-4f78-801c-1222",
-            gs_key="test_prism_trial_id/ctdna/test_batch/CTTTPP121.00/OnPrem.correctedDepth.txt",
-            metadata_availability=False,
-            allow_empty=False,
-        ),
-        LocalFileUploadEntry(
             local_path="CTTTPP111.00/OnPrem.params.txt",
             upload_placeholder="4c409c82-dff7-4f78-801c-33ssf",
             gs_key="test_prism_trial_id/ctdna/test_batch/CTTTPP111.00/OnPrem.params.txt",
             metadata_availability=False,
             allow_empty=False,
         ),
         LocalFileUploadEntry(
-            local_path="CTTTPP121.00/OnPrem.params.txt",
-            upload_placeholder="4c409c82-dff7-4f78-801c-111",
-            gs_key="test_prism_trial_id/ctdna/test_batch/CTTTPP121.00/OnPrem.params.txt",
-            metadata_availability=False,
-            allow_empty=False,
-        ),
-        LocalFileUploadEntry(
             local_path="CTTTPP111.00/OnPrem.RData",
             upload_placeholder="4c409c82-dff7-4f78-801c-222ssff",
             gs_key="test_prism_trial_id/ctdna/test_batch/CTTTPP111.00/OnPrem.RData",
             metadata_availability=False,
             allow_empty=False,
         ),
         LocalFileUploadEntry(
-            local_path="CTTTPP121.00/OnPrem.RData",
-            upload_placeholder="4c409c82-dff7-4f78-801c-323fff",
-            gs_key="test_prism_trial_id/ctdna/test_batch/CTTTPP121.00/OnPrem.RData",
-            metadata_availability=False,
-            allow_empty=False,
-        ),
-        LocalFileUploadEntry(
             local_path="CTTTPP121_00.bam",
             upload_placeholder="189068fe-4c00-4a67-9a98-74223266c1e0",
             gs_key="test_prism_trial_id/ctdna/test_batch/CTTTPP121.00/demultiplexed.bam",
             metadata_availability=False,
             allow_empty=False,
         ),
         LocalFileUploadEntry(
```

### Comparing `nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/manifest_data.py` & `nci_cidc_schemas-0.26.33/tests/prism/cidc_test_data/manifest_data.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/utils.py` & `nci_cidc_schemas-0.26.33/tests/prism/cidc_test_data/utils.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/prism/schema/test_schema.json` & `nci_cidc_schemas-0.26.33/tests/prism/schema/test_schema.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/prism/test_cidc_data_model.py` & `nci_cidc_schemas-0.26.33/tests/prism/test_cidc_data_model.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/prism/test_core.py` & `nci_cidc_schemas-0.26.33/tests/prism/test_core.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/prism/test_extra_metadata.py` & `nci_cidc_schemas-0.26.33/tests/prism/test_extra_metadata.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/prism/test_merger.py` & `nci_cidc_schemas-0.26.33/tests/prism/test_merger.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/prism/test_pipelines.py` & `nci_cidc_schemas-0.26.33/tests/prism/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/test_artifacts.py` & `nci_cidc_schemas-0.26.33/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/test_assays.py` & `nci_cidc_schemas-0.26.33/tests/test_assays.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/test_clinicaltrial_examples.py` & `nci_cidc_schemas-0.26.33/tests/test_clinicaltrial_examples.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/test_json_validation.py` & `nci_cidc_schemas-0.26.33/tests/test_json_validation.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/test_migrations.py` & `nci_cidc_schemas-0.26.33/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/test_schemas.py` & `nci_cidc_schemas-0.26.33/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/test_strict_meta_schema.py` & `nci_cidc_schemas-0.26.33/tests/test_strict_meta_schema.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/test_template.py` & `nci_cidc_schemas-0.26.33/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/test_template_reader.py` & `nci_cidc_schemas-0.26.33/tests/test_template_reader.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/test_template_writer.py` & `nci_cidc_schemas-0.26.33/tests/test_template_writer.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/test_templates.py` & `nci_cidc_schemas-0.26.33/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/test_trial_core.py` & `nci_cidc_schemas-0.26.33/tests/test_trial_core.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/test_unprism.py` & `nci_cidc_schemas-0.26.33/tests/test_unprism.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/test_util.py` & `nci_cidc_schemas-0.26.33/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.32/tests/utils/test_template_generator.py` & `nci_cidc_schemas-0.26.33/tests/utils/test_template_generator.py`

 * *Files identical despite different names*

