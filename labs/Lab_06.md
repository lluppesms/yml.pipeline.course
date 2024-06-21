# Lab 6: Creating a YML Pipeline with a Reusable Template

In this lab we will create the a YML pipeline that pulls out the code in pipeline 05 and creates a reusable template for deploying resources.

This pipeline extracts the code from the previous pipeline and puts it into a template file. This template file is then called from the pipeline.

Variables have been moved from [vars/var-common-01.yml](../.azdo/pipelines/vars/var-common-01.yml) to [vars/var-common-02.yml](../.azdo/pipelines/vars/var-common-02.yml). Please check the values in the var-common-02 file and make sure your storage account name matches.

It should deploy and run exactly the same as the previous pipeline, but now the code is in a template file.

---

[Next Lab](./Lab_07.md) | [Previous Lab](./Lab_05.md) | [Table of Contents](./README.md)
