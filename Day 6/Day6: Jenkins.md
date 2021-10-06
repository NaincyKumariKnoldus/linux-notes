### Is Continuous delivery and Continuous Deployment alternate process ?
Both are the process of software release. The only difference is that in Continuous Deployment the deployment to the production environment is fully automated and does not require manual intervention but in Continuous Delivery some amount of manual intervention with the managers approval is needed.


### Packaging is a part of CI or CD ?
Packaging is a part of Continuous Integration in which code gets packaged and stored in a repository.

### What is Monitoring?
Continuous Monitoring comes in at the end of the DevOps pipeline. Once the software is released into production, Continuous Monitoring will notify dev and QA teams in the event of specific issues arising in the prod environment. It provides feedback on what is going wrong, which allows the relevant people to work on necessary fixes as soon as possible.

### What is credential in Jenkins ?
Credentials are used to authenticate users for login. In Jenkins credential manager plugin is used to manage credentials like username and password for private repositories, ssh keys etc. \
Jenkins can store the following types of credentials:

`Secret text `- a token such as an API token (e.g. a GitHub personal access token),

`Username and password `- which could be handled as separate components or as a colon separated string in the format username:password

`Secret file `- which is essentially secret content in a file,

`SSH Username with private key `- an SSH public/private key pair,

`Certificate `- a PKCS#12 certificate file and optional password, or

`Docker Host Certificate Authentication `credentials.

