# gnomon_datasets
This repository contains two datasets used to evaluate Gnomon **add link to paper here**.

Each dataset (`dev`, `test`) contains documentation tables extracted from Open Data repositories. 
The first line corresponds to the table header, and the following lines correspond to the table data. 
Headers designate different metadata semantics. 
Each row corresponds to metadata for a particular data attribute in a different file. 

## `<dataset>`_table_list.csv

This file records the original url the source file of each table was downloaded from.

## `<dataset>`_column_mappings.csv

This file records for each table, the mapping between table columns and fields of a flat attribute metadata model.
