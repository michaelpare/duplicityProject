# Duplicity Backups to Google Drive with Encryption

This project shows a step by step guide to enable full backups to a Google Drive of their entire mysql database with full backups every hour. It utilizes Duplicity, an app that allows uploads of files to a remote location.

The use cases of this is to provide an off-site backup to your data while being encyrpted to prevent any man in the middle or compromise if the cloud account is breached. 

## How it works:

Duplicity encrypts data and sends them to a different location. Using pydrive, a python api client that interacts with Google Drive, we can allow Duplicity to upload these backups to a cloud location. In the case of this project, mysql databases are subject to backup using the mysqldump command. 

