# spikein_barcode_parser
A tool to extract barcodes from spike-in sequencing data, particularly whole-plasmid sequencing.

## Purpose
This repository hosts a simple tool for extracting barcodes from sequencing data. It is intended to handle moderate amounts of data per sample, such as you would generate with a spike-in or using a whole-plasmid sequencing service (e.g. Primordium).

## Workflow
Each sample is listed in the 'samplelist.csv' file, with a unique name and a single `.fastq.gz` file. The barcode is parsed using [dms_variants `illuminabarcodeparser` function](https://jbloomlab.github.io/dms_variants/dms_variants.illuminabarcodeparser.html). The parsed barcodes and their counts are saved in a CSV output file with the same name as the sample. The distribution of barcode counts is displayed.

