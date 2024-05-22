# Lab 5: Creating a YML Pipeline with a Merged Bicep Parameter file

In this lab we will create the a YML pipeline that shows how to merge variables into a Bicep Parameter File.

This lab combines the concepts from Lab 3 and Lab 4, and merges the variable file from Lab 3 with the Bicep Parameter file, similar to Lab 4.

This pipeline uses the [qetza.replacetokens](https://marketplace.visualstudio.com/items?itemName=qetza.replacetokens) Marketplace extension task to replace tokens in the Bicep Parameter file with values from the YML variable file. You will need to install this extension in your Azure DevOps organization before you proceed.

If you open the [infra/bicep/storageaccount-variables.bicepparam](../infra/bicep/storageaccount-variables.bicepparam) file you will see variable definitions that look like '#{storageAccountName}#'.  The qetza.replacetokens task will replace these tokens with the values from the YML variable file.

Notice the "Display Parameter File Contents" task on lines 33-40. This is an example of executing a random script in the pipeline. This is a good way to debug and see what is happening in the pipeline. This script with show the names of the files, then use the 'cat' command to display the contents of the Bicep Parameter file.

Deploy the [05-pipeline-merging-variable-file-and-bicep-parm-file.yml](../.azdo/pipelines/05-pipeline-merging-variable-file-and-bicep-parm-file) using the steps in [Deploy a YML Pipeline](./CreateNewPipeline.md).

The pipeline can now be run and it should will merge the storage account name from the YML variable file into a 'parameterized' Bicep Parameters file, and the resource group name and all the other values in the YML variable file.

We're getting closer to a more generic pipeline that can be used in multiple environments, but it's still using one file which is hard-coded.
