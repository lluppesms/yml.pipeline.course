# Lab 3: Creating a YML Pipeline with a variable YML file

In this lab we will create the a YML pipeline that shows how to use variables in another YML file.

Edit the [vars/var-common-01.yml](../.azdo/pipelines/vars/var-common-01.yml) file to have your unique storage account name and then save and commit that changes.

Note that now the [03-pipeline-with-variable-file.yml](../.azdo/pipelines/03-pipeline-with-variable-file.yml) pipeline file is now very generic and does not have any hard-coded values in it. Everything is in the [vars/var-common-01.yml](../.azdo/pipelines/vars/var-common-01.yml) file.

Deploy the [03-pipeline-with-variable-file.yml](../.azdo/pipelines/03-pipeline-with-variable-file.yml) using the steps in [Deploy a YML Pipeline](./CreateNewPipeline.md).

The pipeline can now be run and it should use the storage account name, resource group name, and all the other values in the variable file.
