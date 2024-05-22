# Lab 7: Creating a YML Pipeline with a Code Scanning Template

In this lab we will create the a YML pipeline that utilizes a code scanning template.

This pipeline is the same as the previous pipeline, but it adds the dimension of calling multiple templates.  In this case we will add an additional template that scans the code for security vulnerabilities.

The pipeline will call the [templates/07-template-scan-code.yml](./.azdo/pipelines/templates/07-template-scan-code.yml) template file.  This template file will scan the code for security vulnerabilities using the [Microsoft Security Code Analysis](https://marketplace.visualstudio.com/items?itemName=MicrosoftSecurityCodeAnalysis) extension, and/or using the GitHub Advanced Security For Azure DevOps scanner (to use this option, you must enable GHAzDO for this repository in your Azure DevOps Project).

When this pipeline is run, the user will be prompted when it starts, allowing them to run (or not run) the security scans.
