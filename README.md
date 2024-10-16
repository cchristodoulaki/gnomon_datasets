# gnomon_datasets
This repository contains two datasets used to evaluate Gnomon **link to be added when camera ready is available**.
## Datasets
Each dataset (`dev`, `test`) contains documentation tables extracted from Open Data repositories. 

The first line in each file corresponds to the table header, and the following lines correspond to the table data. 
Headers designate different metadata semantics, which should be mapped to a unified metadata model. 
Each row corresponds to metadata for a particular data attribute in a different file (not available in this dataset currently). 

### `<dataset>`_table_list.csv

This file records the original url the source file of each table was downloaded from.

## Ground Truth Mappings
### Model

| Name | Description |
|------------|------------|
| dataset |  The name of the file the described attribute exists in. |
| name [mandatory] |  The attribute name, as seen in the data table. |
| title  | A human-readable version of the attribute name. |
| definition  | A text description of the attribute, may include context. |
| datatype |  Specifies which type of value the attribute can have. |
| scale  | For numeric attributes, the multiplier (e.g., millions). |
| format  | A definition of the structure of data (e.g., ‘YYYY-MM-DD’). |
| unit  | The unit of the associated values (e.g., meters, KWh). |
| key  | An indication that the attribute is a primary key. |
| nullable  | An indication that an attribute value is or isn’t mandatory. |
| schema |  Name/URL of an existing schema the attribute belongs to. |
| examples  | Sampled values from the attribute domain. |
| notes | Text with miscellaneous extra information |

### `<dataset>`_column_mappings.csv

This file records for each table, the mapping between table columns and fields of a flat attribute metadata model.

**Attributes:**
- datatable: the id of the csv file containing the table
- portal: the portal the table was originally sourced from
- csv_column: the index of a column in that table
- extracted_name: the name extracted from the header of that column 
- target: the ground truth target mapping to the attribute metadata model.
