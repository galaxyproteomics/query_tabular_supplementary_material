# Proteogenomics

## Files

Workflow: [`proteogenomics.ga`](proteogenomics.ga)

History file: [`PSM_Report.tabular`](PSM_Report.tabular)

## Required Galaxy Tools

If you wish to run the proteogenomics workflow on your own Galaxy instance you will need to install the following, versioned, tools:

| Tool Name                | Owner   | Version |
|--------------------------|---------|---------|
| `column_maker`           | devteam | [626658afe4cb](https://toolshed.g2.bx.psu.edu/repos/devteam/column_maker/rev/626658afe4cb) |
| `fasta_filter_by_length` | devteam | [2fd6033d0e9c](https://toolshed.g2.bx.psu.edu/repos/devteam/fasta_filter_by_length/rev/2fd6033d0e9c) |
| `ncbi_blast_plus`        | devteam | [d724d9af93ee](https://testtoolshed.g2.bx.psu.edu/repos/devteam/ncbi_blast_plus/rev/d724d9af93ee) |
| `query_tabular`          | iuc     | [1ea4e668bf73](https://toolshed.g2.bx.psu.edu/repos/iuc/query_tabular/rev/1ea4e668bf73) |
| `tabular_to_fasta`       | devteam | [0b4e36026794](https://toolshed.g2.bx.psu.edu/repos/devteam/tabular_to_fasta/rev/0b4e36026794) |

## Workflow Instructions

We have set-up a publically accessible Galaxy instance on the Jetstream cloud-based cyberinfrastructure resource. Here we provide instructions on accessing this public instance.

1. Go to [https://z.umn.edu/proteogenomicsgateway](https://z.umn.edu/proteogenomicsgateway)

2. Register to use the Galaxy instance. Galaxy requires that all users input an email address to use tools and build workflows etc. To register do the following:
    - Click on the `User` tab and then click on `Register`
    - Enter an email address, password and public name of your choosing

> NOTE: Users who want to remain anonymous can enter an email in the form of guestX@galaxyp.org (where X is any number of your choosing), along with a password and public name of your choosing. Please note that if the email entered is not valid, the administrators of this instance will not be able to contact the user regarding any issues related to the instance. If the desire it to use this instance for long-term research use, we suggest using a valid email address. 
 
3. Once registered, workflows and sample input data can be accessed within the Shared Data tab. 
    - To run the workflow, first appropriate input data must be loaded into your active History. Clickon `Shared data` and select `Histories`. From the list of shared Histories, select `Input for Query Tabular F1000 Workflow`. In the page that appears, select `Import History` and click on `Import` when the window appears.
    - Next click on `Shared Data`, select `Workflows`
    - When the shared Published Workflows page appears, type `Query` in the search field 
    - The workflow titled `Query Tabular F1000: PSM Report ---> Novel Peptides` will come up. Click on the drop down arrow on the right of the workflow button, and select `Import`
    - In the green box that appears, click on `Start using this workflow`.
    - This will now show up in `Your workflows`. Click on the dropdown arrow and select `Run`. 
    - The next window will show the steps in the workflow. The first item shows the input data that you just imported into your History that will be processed by the workflow (`PSM_report.tabular`)
    - Click on `Run workflow` and the analysis will proceed.

