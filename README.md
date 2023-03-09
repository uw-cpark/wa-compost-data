# WA Compost Data README
This dataset was curated for University of Washington iSchool class LIS 545 Data Curation I (Winter Quarter 2023). The data are obtained through State of Washington Department of Ecology about their waste reduction compost program, which include tonnage of various different types of materials composted, the total tonnage of materials composted, and the total tonnage of compost produced. The data contain information from years 2015 until 2020. The curated dataset is available in .XLSX format, and the two original datasets from the Department of Ecology are also available in .XLSX format.

This dataset is relevant to policymakers interested in seeing different types of materials composted in order to create policies and incentives to boost composting. Citizens who have an interest in protecting and aiding the environment could also gain valuable insight through this dataset.

### Data Normalization
The curated dataset combines both original datasets' information and removing any values that are "0.00." It should be noted that the dataset has no values for the "Other food" variable from 2018 to 2020 because the values were counted in the "Food processing - pre-consumer" variable. In the "Mixed paper" variable, the year 2020 contains one value while the rest of the years are blank. It is unknown whether there is a lack of data or if the value is zero. Therefore, the dataset is normalized by removing any zero values to make those fields blank.

## Naming Convention

Naming convention for the files is as follows:
```
yyyy-yyyy_materials_composted_{description}
```
`{description}` is replaced by the description of materials contained in the dataset. In the case of this dataset, `all` means a list of all the materials composted, `foods` breaks down the different food types composted, and `consolidated` is the curated dataset that combines both `all` and `foods`.

## Data Dictionary

| **Variable** | **Variable Type** | **Measurement Unit** | **Allowed Values** | **Description** |
| --- | --- | --- | --- | --- |
| **Year** | Integer | Year | Calendar year | The year the materials composted were counted |
| **Agricultural** | Integer | Numeric | Positive integer | Total tons of agricultural materials composted that year |
| **Animal parts** | Integer | Numeric | Positive integer | Total tons of animal parts composted that year |
| **Biosolids** | Integer | Numeric | Positive integer | Total tons of biosolids composted that year |
| **Food - mixed with yard debris** | Integer | Numeric | Positive integer | Total tons of food mixed with yard debris composted that year |
| **Food processing - post-consumer** | Integer | Numeric | Positive integer | Total tons of post-consumer food composted that year |
| **Food processing - pre-consumer** | Integer | Numeric | Positive integer | Total tons of pre-consumer processed food composted that year |
| **Industrial organics** | Integer | Numeric | Positive integer | Total tons of industrial organics composted that year |
| **Landclearing** | Integer | Numeric | Positive integer | Total tons of landclearing materials composted that year |
| **Manure** | Integer | Numeric | Positive integer | Total tons of manure composted that year |
| **Mixed paper** | Integer | Numeric | Positive integer | Total tons of mixed paper materials composted that year |
| **Other food** | Integer | Numeric | Positive integer | Total tons of various other food materials composted that year |
| **Other org** | Integer | Numeric | Positive integer | Total tons of various other organic materials composted that year |
| **Sawdust** | Integer | Numeric | Positive integer | Total tons of sawdust composted that year |
| **Wood (other)** | Integer | Numeric | Positive integer | Total tons of various other wood materials composted that year |
| **Yard waste** | Integer | Numeric | Positive integer | Total tons of yard waste composted that year |
| **Total feedstocks** | Integer | Numeric | Positive integer | Total tonnage of  materials composted that year |
| **Compost produced** | Integer | Numeric | Positive integer | Total cubic yards of compost produced out of composted materials that year |
