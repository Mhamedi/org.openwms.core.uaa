# Purpose
This service is built to fulfill two different requirements regarding to user handling.
At first the service is capable to work as [OpenID Connect](http://openid.net/connect) authentication endpoint and can
authenticate user credentials against data stored in a persistent storage.
The second part deals with user administration like creating new users, updating properties 
of existing ones or deleting them at all. Most application permissions are not directly 
assigned to users explicitly, but to roles. Users are assigned to roles and application
permissions are granted for particular roles. Administration of roles and permissions
is especially required from an UI point of view.

# Deployment

The UAA is an essential component for all kind of applications and requires the highest
degree of availability level (Highest). Therefore it is deployed in an redundant setup
in different locations, on different cloud platforms with different ISP.

| endpoints | billed | SLA |
| --------- | ------ | --- |
| https://openwms-core-uaa.herokuapp.com 
  https://openwms.org/uaa | no | Heroku SLA for Europe region depends on AWS Europe region |

