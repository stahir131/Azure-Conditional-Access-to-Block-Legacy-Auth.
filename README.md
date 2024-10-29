### Block legacy authentication with Conditional Access

#### What are Legacy Authentications<br />
Also known as Basic authentication, it is a traditional method of verifying a user's identity that uses a username and password to access a system. <br />
Examples of legacy authentication include:<br />
* Microsoft Office 2013 or older.<br />
* Apps using mail protocols like POP, IMAP, and SMTP AUTH

According to Microsoft’s analysis, over 97% of credential stuffing attacks and more than 99% of password spray attacks rely on legacy authentication protocols. Disabling or blocking basic authentication would effectively prevent these types of attacks.<br />
##### User exclusions<br />
In case of misconfiguration, Microsoft recommend to exclude the following accounts from the policy:<br />
* **Emergency access or break-glass accounts** to prevent lockout due to policy misconfiguration, so the account can be used to access the tenant.<br />
* **Service accounts and Service principals** such as Microsoft Entra Connect Sync Account. Service accounts are non-interactive accounts that are not tied to any user. They are used by back-end services to allow programmatic access to applications.
