# Email Grouping #

<div align="center">

![GitHub](https://img.shields.io/github/license/AshishBhoi/EmailGroups-IITDH)
![Docker Image CI](https://github.com/AshishBhoi/EmailGroups-IITDH/workflows/Docker%20Image%20CI/badge.svg)

</div>

## Github Link ##

https://github.com/AshishBhoi/EmailGroups-IITDH

## Given files ##

### Persons.csv ###

- Name
- ID
- Email

### Keywords.csv ###

- Contents all the keywords with one keyword per line.

### Emails.csv ###

- Email ID
- Sender ID
- List of receiver ID
- Date and Time
- List of keywords
- If it is a reply previous Email ID else "null"

## Input ##

- Email.csv (Contains all the email exchanged)
- Keywords.csv (Contains all the keywords)
- Persons.csv (Contains details about the person)

## Output ##

Groups of people who have strongly communicated among themselves on a given keyword.
The group should contain persons who have sent at least 5 emails on the topic and also replied to 5 emails that she received on that topic in the last one month.

## Docker ##

- 'Dockerfile' added to create image.

    $ docker build . --file Dockerfile --tag email-transactions
- Run that image.

    $ docker run email-groups
- Creating .tar of docker image

    $ docker save email-groups > email-groups.tar

## Additional Details ##

- VERSION: 1.0.0
- Programming Language: JAVA
- Tools: MAVEN, DOCKER
- Domain: Software Engineering
- License: MIT
- Author: Ashish Kumar Bhoi
