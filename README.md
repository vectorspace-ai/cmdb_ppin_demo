# Vector Space Biosciences
This repository includes a notebook which demonstrates the following:
- How to call the Correlation Matrix Dataset Builder (CMDB) API
- How to generate a heatmap with High Charts using data from the correlation matrix dataset generated
- How to use the Protein-Protein Interaction Network (PPIN) API
- How to generate a hidden relationship network graph with High Charts using the data from the API

### Dependencies: pandas
- If using a notebook, you may need to run %pip install pandas or !pip install pandas
- If using a terminal, you may need to run pip install pandas



### Correlation Matrix Dataset Builder API arguments
- *language_model*: - string - The name of the desired language model
- *row_types*: - string - The types of rows to include in the results
- *column_labels*: - list[str] - The list of column labels to include in the results
- *context_dependency*: - string - used to filter results by the provided context
- *vxv_wallet_addr*: - string

### Protein-Protein Interaction Network API arguments
- *query*: - string - protein name or accession id
- *context_dependency*: - string - used to filter results by the provided context.
- *max_depth*: - int - Limit of how many levels from the root the network should span.
- *branches*: - int - Limit of how many children each node should have.
- *min_score*: - float - The minimum score a correlation should have for it to be added as a node in the network
- *cross_intersection*: - bool - Whether nodes on the same level in the network should be allowed to connect to each other
- *vxv_wallet_addr*: - string