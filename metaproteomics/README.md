# Metaproteomics

## Files

Workflow: [`metaproteomics.ga`](metaproteomics.ga)

History file: [`Sample_Peptide_Shaker_PSM_Report.tabular`](Sample_Peptide_Shaker_PSM_Report.tabular)

## Required Galaxy Tools

If you wish to run the metaproteomics workflow on your own Galaxy instance you will need to install the following, versioned, tools:

| Tool Name                | Owner     | Version |
|--------------------------|-----------|---------|
| `fasta_compute_length`   | devteam   | [de2db1bdfbf8](https://toolshed.g2.bx.psu.edu/repos/devteam/fasta_compute_length/rev/de2db1bdfbf8) |
| `fasta_filter_by_length` | devteam   | [2fd6033d0e9c](https://toolshed.g2.bx.psu.edu/repos/devteam/fasta_filter_by_length/rev/2fd6033d0e9c) |
| `fasta_to_tabular`       | devteam   | [7e801ab2b70e](https://toolshed.g2.bx.psu.edu/repos/devteam/fasta_to_tabular/rev/7e801ab2b70e) | 
| `query_tabular`          | iuc       | [1ea4e668bf73](https://toolshed.g2.bx.psu.edu/repos/iuc/query_tabular/rev/1ea4e668bf73) |
| `tabular_to_fasta`       | devteam   | [0b4e36026794](https://toolshed.g2.bx.psu.edu/repos/devteam/tabular_to_fasta/rev/0b4e36026794) |
| `text_processing`        | bgruening | [6378f8384f30](https://toolshed.g2.bx.psu.edu/repos/bgruening/text_processing/rev/6378f8384f30) |

## Workflow Instructions

The example metaproteomics workflow using Query Tabular has been implemented within the same accessible instance as described above for the proteogenomics examples.    - To access this example workflow, follow these steps:

1. Go to [https://z.umn.edu/metaproteomicsgateway](https://z.umn.edu/metaproteomicsgateway). To utilize this instance, you must be registered and logged in. Follow the instructions above for the proteogenomics example above to do this.

2. Once registered, workflows and sample input data can be accessed within the Shared Data tab. 
   - To run the workflow, first appropriate input data must be loaded into your active History. Clickon `Shared data` and select `Histories`. From the list of shared Histories, select `QueryTabular_input_F1000`. In the page that appears, select `Import History` and click on `Import` when the window appears.
   - Next click on `Shared Data`, select `Workflows`
   - When the shared Published Workflows page appears, type `Query` in the search field 
   - The workflow titled `Query Tabular F1000 Metaproteomics: PSM Report to Blast Input Peptides` will come up. Click on the drop down arrow on the right of the workflow button, and select `Import`
   - In the green box that appears, click on `Start using this workflow`.
   - This will now show up in `Your workflows`. Click on the dropdown arrow and select `Run`. 
   - The next window will show the steps in the workflow. The first item shows the input data that you just imported into your History that will be processed by the workflow (`Sample_Peptide_Shaker_PSM_Report.tabular`)
   - Click on `Run workflow` and the analysis will proceed.
