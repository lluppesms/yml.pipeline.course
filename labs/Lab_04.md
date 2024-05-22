# Lab 4: Creating a YML Pipeline with a Bicep Parameter file

In this lab we will create the a YML pipeline that shows how to use a hard-coded Bicep Parameter file so that your YML is not hard-coded with variable names.

Edit the [infra/bicep/storageaccount-hardcoded.bicepparam](../infra/bicep/storageaccount-hardcoded.bicepparam) file to have your unique storage account name and then save and commit that changes.

Deploy the [04-pipeline-with-bicep-parm-file.yml](../.azdo/pipelines/04-pipeline-with-bicep-parm-file.yml) using the steps in [Deploy a YML Pipeline](./CreateNewPipeline.md).

The pipeline can now be run and it should use the storage account name from the Bicep Parameters file, and the resource group name and all the other values in the YML variable file.

We're getting closer to a more generic pipeline that can be used in multiple environments, but it's still using one file which is hard-coded.
