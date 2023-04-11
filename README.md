Role Name
=========
This role installs the google and/or ldap identity providers.

Requirements
------------
This role requires Ansible 2.9 or higher, molecule, an OpenShift cluster and a user logged, a ldap server with users created (for ldap idp), a oauth configuration in google cloud (for google idp).

Collections
-----------
kubernetes.core

Role Variables
--------------

| Name | Default value | Description |
|------|---------------|-------------|
| idp.state | present | State of the identity provider |
| idp.ldap.enabled | false | Enable ldap identity provider |
| idp.ldap.attributes.url | "" | LDAP server URL |
| idp.ldap.attributes.email | "" | LDAP email attribute |
| idp.ldap.attributes.name | "" | LDAP name attribute |
| idp.ldap.attributes.preferredUsername | "" | LDAP preferred username attribute |
| idp.ldap.attributes.id | "" | LDAP id attribute |
| idp.ldap.attributes.ca | "" | LDAP CA certificate |
| idp.ldap.attributes.insecure | false | LDAP insecure |
| idp.ldap.mapping.method | "" | LDAP mapping method |
| idp.ldap.mapping.name | "" | LDAP mapping name |
| idp.ldap.type | "LDAP" | LDAP type |
| idp.ldap.name | "ldap" | LDAP name |
| idp.google.enabled | false | Enable google identity provider |
| idp.google.attributes.clientID | "" | Google client ID |
| idp.google.attributes.clientSecret.name | "" | Google client secret name |
| idp.google.attributes.clientSecret.value | "" | Google client secret value |
| idp.google.attributes.hostedDomain | "" | Google hosted domain |
| idp.google.type | "Google" | Google type |
| idp.google.name | "" | Google name |
| idp.user.name | "" | User name |
| idp.user.permissions | "" | User permissions |



