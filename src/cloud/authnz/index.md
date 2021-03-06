---
title:  "Securely Authorize Galaxy to Access Protected Data on Cloud"
---

On this page we explain a method that enables a user to securely authorize Galaxy to access their privately 
hosted data on cloud. This method uses industry standards for user identification and their accesss control:
OpenID Connect protocol and role-based access control model. Accordingly, this method has the following 
advantages: 

* Users do **NOT** need to share their credentials with Galaxy;
* User's identity and granted previliges (theoretically) cannot be impersonated or hijacked;
* Galaxy accesses protected data on cloud assuming a *role*, which is defined by the user and has 
independent privileges;
* Galaxy's access can be audited, restricted, elevate, and revoked by the user at anytime, 
independent from any other service and the user themself.


To use this method a user needs to take the following steps: 

1. Login to Galaxy using Google account (or any other supported OIDC-based identity provider). [Read this page](/src/admin/authentication/index.md) for details;
2. Setup a provider-specific _cloud authorization_ in Galaxy:
	1. read [how to setup cloud authorization for AWS](/src/cloud/authnz/aws/index.md);
	1. read [how to setup cloud authorization for Azure](/src/cloud/authnz/azure/index.md).


