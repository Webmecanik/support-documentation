# Setting Up An Instance

## Introduction ##

Setting up the domain name for sending emails is an important step. Without this established, no email will be sent from the platform.
You can find all of this information in the technical details section of the instance.

![image](instance-details.png)

## TXT File : Domain Name Use Authorisation ##

For each account, you will be asked to upload a '.txt' file at the root of the domain name (via FTP access). This file has a unique name that will verify that you are the owner of the domain, and allows the email router to send emails in its name.

1. Create the file (empty) with the name indicated (e.g. `jlbzgoh89Y4IOUEOI.txt`)
2. Upload this to the root of the domain name (for example, the following URL must link to the empty '.txt' file: `http://mydomain.comjlbzgoh89Y4IOUEOI.txt`)
3. Return to the instance details on myWebmecanik and click on the **validate** button.

## SPF Redirection : Deliverability Improvement ##

1. On the DNS settings of your domain name, create an SPF entry with the details stated on myWebmecanik for the instance. **Note** It may be the case that you already have an SPF entry, and unfortunately it is not possible to have multiple SPF entries. Consult the [Google documentation for multi SPF entries](https://support.google.com/a/answer/4568483)
2. Return to the instance details on myWebmecanik and click on the **validate** button.

## DKIM Redirection : Deliverability Improvement ##

1. On the DNS settings of your domain name, create a DKIM entry with the details stated on myWebmecanik for the instance.
2. Return to the instance details on myWebmecanik and click on the **validate** button.
