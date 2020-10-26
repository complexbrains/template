## Get started

### 1. Fork this repository

### 2. Create a GitHub access token

Read the warning below and follow [these steps](https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/creating-a-personal-access-token#creating-a-token). 

| ⚠️ Warning|
| :--- |
|Make sure that you check the **repo**, **admin:repo_hook** and **workflow** boxes while creating your access token. Please not lose the generated key, at least until the next step :)|

### 3. Create an encrypted secret for your repo

Simply follow [these steps](https://docs.github.com/en/free-pro-team@latest/actions/reference/encrypted-secrets#creating-encrypted-secrets-for-a-repository).

The name of the secret must be `PAT_BOT` and the value must be the key you obtained from the previous step.

### 4. Create your report

* Place your figures in the [`figures`](figures) folder. 

* Edit [`report.md`](report.md) file to create your own report. The template markdown will walk you through how to cite references, add figures and equations etc.

* Edit [`report.bib`](report.bib) to add your bibliography in [BibTeX](http://www.bibtex.org/) format.  

| ⚠️ Warning|
| :--- |
|Please do not change the name or the location of [report.md](report.md) and [report.bib](report.bib). Unless you provide an absolute path for your figures, they will be looked for in the `figures` folder.|

### 5. Push your changes 

Whenever you push your changes to the `main` branch, GitHub actions will create a nice web page (your_github_handle.github.io/template unless you don't change the name of the repo) where people can download its PDF. 
