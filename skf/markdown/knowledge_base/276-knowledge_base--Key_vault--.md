Description:

Keys should remain in a protected key vault at all times. 
In particular, ensure that there is a gap between the threat vectors 
that have direct access to the data and the threat vectors that have direct access to the keys. 
This implies that keys should not be stored on the application or web server 
(assuming that application attackers are part of the relevant threat model).

A key vault helps secure, store and tightly control access to tokens, passwords, certificates, 
encryption keys for protecting secrets and other sensitive data.  

Imagine the use of a keyvault in the following scenario's

* Running a docker container and provisioning it with secrets over CLI
* Checking in API keys in your source repositories
* etc

Solution:

centrally store, access, and distribute secrets like API keys,
AWS IAM/STS credentials, SQL/NoSQL databases, X.509 certificates, 
SSH credentials, etc by means of a key vault.