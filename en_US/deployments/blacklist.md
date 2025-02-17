<!-- markdownlint-disable MD001 -->

# Blacklist

The blacklist is used to prohibit client connections from being matched and is suitable for restricting a small number of clients. The control of the blacklist will expire after the validity period.

::: warning
The blacklist function only applies to Dedicated and BYOC deployments.
:::

From the left-navigation menu of EMQX Cloud Console, selet **Authentication & ACL** -> **Blacklist**. Click **+ Add** on the top right to add a client to the blacklist.

![blacklist](./_assets/blacklist_new.png)

**Type and Value**

The client to be added to the blacklist can be identified by the following types. Select the type and set the value accordingly based on the requirements:

- Clinet ID: Letters, numbers and some special characters (_, -, /, +, #, $, %, @, & and .), up to 256 characters.
- Username: Letters, numbers and some special characters (_, -, /, +, #, $, %, @, & and .), up to 256 characters.
- Clinet IP: IPv4 address.

**Expiration Time**

The maximum expiration time is 1 year. The minimum expiration time is 5 minutes, and it cannot be earlier than the current time.

**Note**

Optional.