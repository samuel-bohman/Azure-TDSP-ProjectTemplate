# TDSP Project Structure, and Documents and Artifact Templates

This is a general project directory structure for Team Data Science Process developed by Microsoft. It also contains templates for various documents that are recommended as part of executing a data science project when using TDSP. 

[Team Data Science Process (TDSP)](https://docs.microsoft.com/en-us/azure/machine-learning/team-data-science-process/overview) is an agile, iterative, data science methodology to improve collaboration and team learning. It is supported through a lifecycle definition, standard project structure, artifact templates, and [tools](https://github.com/Azure/Azure-TDSP-Utilities) for productive data science. 

**NOTE: Data (raw, processed, or feature sets ready for modeling) should NEVER be stored on GitHub**. Ensure all data file types are listed in the .gitignore file in the project root folder. Instead, use Microsoft OneDrive for temporary data transfer and storage. 

The two documents under Docs/Project, namely the [Charter](./Docs/Project/Charter.md) and [Exit Report](./Docs/Project/Exit%20Report.md) are particularly important to consider. They help to define the project at the start of an engagement, and provide a final report to the customer or client.

**NOTE:** In some projects, e.g. short term proof of principle (PoC) or proof of value (PoV) engagements, it can be relatively time consuming to create and all the recommended documents and artifacts. In that case, at least the Charter and Exit Report should be created and delivered to the customer or client. As necessary, organizations may modify certain sections of the documents. But it is strongly recommended that the content of the documents be maintained, as they provide important information about the project and deliverables.
