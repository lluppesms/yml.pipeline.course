# Lab 1: Creating an Azure DevOps YML Pipeline

In this lab we will create the simplest YML file example with some hard-coded values.

To create an Azure DevOps pipeline from an existing YML file in a GitHub repository, follow these steps.

Note: these steps will be repeated almost exactly in each of the next labs.

---

Deploy the [01-simplest-pipeline.yml](../.azdo/pipelines/01-simplest-pipeline.yml) using the steps below:

**Step 1:** Click New pipeline from the Pipeline section of the Azure DevOps project

![Step 1](assets/images/NewPipeline-1.jpg)

**Step 2:** Select source as GitHub:

![Step 2](assets/images/NewPipeline-2.jpg)

**Step 3:** Select the GitHub repository

![Step 3](assets/images/NewPipeline-3.jpg)

**Step 4:** Select Existing Pipelines YAML file

![Step 4](assets/images/NewPipeline-4.jpg)

**Step 5:** Select the desired pipeline

![Step 5](assets/images/NewPipeline-5.jpg)

**Step 6:** For some cases, when the pipeline source is shown, you can just click Run and start your pipeline.  However, it's usually best the first time to just Save and not Run, so select More Actions and Save the file.

![Step 6](assets/images/NewPipeline-6.jpg)

**Step 7:** You may notice that by default a new pipeline created this was has the same name as the repository that it came from, not the name of the pipeline. It's best to rename it right now, to something more meaningful like the original name of the pipeline YML file.

![Step 7](assets/images/NewPipeline-7.jpg)

**Step 8:** Edit the pipeline and now change the StorageAccountName value on line 18 to be unique to you. This will create a resource in Azure that must be globally unique.

![Step 8](assets/images/NewPipeline-8.jpg)

**Step 9:** The pipeline can now be run and (assuming your service connection is right!) you should create a new storage account in your resource group.

---

[Next Lab](./Lab_02.md) | [Previous Lab](./Lab_00.md) | [Table of Contents](./README.md)
