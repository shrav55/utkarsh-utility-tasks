# Utkarsh Utility tasks

A set of utility build and release tasks to help you in your Azure Pipelines. The tasks in this extension are written in `node` and hence can be run in both Windows or Linux based agents.

## Tasks

This extension currently provides following tasks. I plan to add more in the future.

### Generate Secrets

This task generates a secure string based on the given criteria. The task will be useful 

- When you do not want to mantain the passwords, secrets in your files and commit in the source control. Use this task to generate passwords/secrets on the fly. 
- You would like to rotate your passwords every few days and hence would like to generate new passwords in your pipeline.  

[Read more](./tasks/secrets-for-strings)

![generate-secret](images/screenshots/genrate-secrets.png)


### Publish Secrets to Azure Key vault

As the name suggests this task publishes the secrets to selected azure key vault. The advantage of using this task is you can publish secrets in bulk. Useful especially when you need to publish multiple secrets at once. The task also allows you to add optional tags to each secret you write. 

[Read more](./tasks/publish-secrets-to-kv)


![publish-to-kv](images/screenshots/publish-to-kv.png)


## Changes

> - 1.0 - Initial release

## Feedback

Please rate the extension and share/tweet to spread the word!!

- Found a bug or need to make a feature request? - Raise it as an [issue](https://github.com/onlyutkarsh/utkarsh-utility-tasks/issues).
- Have a question? - Raise it here in the Q and A section.