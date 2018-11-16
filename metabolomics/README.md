# Metabolomics

## Files

Workflow: [`metabolomics.ga`](metabolomics.ga)

History files:
  - [dataMatrix.tabular](dataMatrix.tabular)
  - [sampleMetadata.tabular](sampleMetadata.tabular)
  - [variableMetadata.tabular](variableMetadata.tabular)

## Required Galaxy Tools

If you wish to run the metaproteomics workflow on your own Galaxy instance you will need to install the following, versioned, tools:

| Tool Name       | Owner  | Version |
|-----------------|--------|---------|
| `query_tabular` | iuc    | [1ea4e668bf73](https://toolshed.g2.bx.psu.edu/repos/iuc/query_tabular/rev/1ea4e668bf73) |
| `vkmz_qt`       | eslerm | [e85e0a79bb9b](https://testtoolshed.g2.bx.psu.edu/repos/eslerm/vkmz_qt/rev/e85e0a79bb9b) |

## Workflow Instructions

The example metabolomics workflow using Query Tabular has been implemented within the same accessible instance as described above for the metaproteomics example. To access this example workflow, follow these steps:

1. Go to [https://z.umn.edu/metaproteomicsgateway](https://z.umn.edu/metaproteomicsgateway). To utilize this instance, you must be registered and logged in. Follow the instructions above for steps to register and log in to a Galaxy instance.

2. The use case of Query Tabular for metabolomics uses a workflow named `Query Tabular F1000: Mass Adjustment`. A History has been generated that provides input data for the workflow. Use of this workflow and History require similar steps as described above for the metaproteomics example.
   - The `Query Tabular F1000: Mass Adjustment` workflow requires loading the XCMS files dataMatrix, sampleMetadata, and variableMetadata as input parameters in the first, VKMZ, step. These files can be found in the `Input for Query Tabular F1000 Metabolomics Workflow` History. Import this History using steps described above for the metaproteomics example.
   - Once the History has been imported, next imported the workflow `Query Tabular F1000 Metabolomics: Mass Adjustment` from the `Shared Data > Workflows` location.
   - After selecting `Run workflow`, the user needs to set the correct input data from the History in the workflow interface:
     - For the XCMS Data Matrix input, select `dataMatrix.tabular` (Item 1 in the History)
     - For the XCMS Sample Metadata input, select `sampleMetadata.tabular` (Item 2 in the History)
     - For the XCMS Variable Metadata input, select `variableMetadata.tabular` (Item 3 in the History)
   - The standards utilized for mass shift calibration are: 1,3-naphthalenediol (C10H8O2), 7-amino-4-methylcoumarin (C10H9NO2), 2-phenylindole (C14H11N), abscisic acid (C15H20O4), di-n-pentyl phthalate (C18H26O4), chlorogenic acid (C16H18O9), & cortisone (C21H28O5)
   - The History contains deleted steps which demonstrate running the workflow. Clicking `deleted` in the right hand History Pane will show deleted steps which can be restored and viewed.
