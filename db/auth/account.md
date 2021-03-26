# account

# Table: account**
**

This table holds information on all available accounts.

## Structure

<table>
<tbody>
<tr>
<td><p><strong>Field</strong></p></td>
<td><p><strong>Type</strong></p></td>
<td><p><strong>Attributes</strong></p></td>
<td><p><strong>Key</strong></p></td>
<td><p><strong>Null</strong></p></td>
<td><p><strong>Default</strong></p></td>
<td><p><strong>Extra</strong></p></td>
<td><p><strong>Comment</strong></p></td>
</tr>
<tr>
<td><p><a href="#id">id</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>Auto increment</p></td>
<td><p>Identifier</p></td>
</tr>
<tr>
<td><p><a href="#username">username</a></p></td>
<td><p>varchar(32)</p></td>
<td><p><br />
</p></td>
<td><p>UNI</p></td>
<td><p>NO</p></td>
<td><p>&quot;</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#sessionkey">sessionkey</a></p></td>
<td><p>varchar(80)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>&quot;</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#v">v</a></p></td>
<td><p>varchar(64)</p></td>
<td><br />
</td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>&quot;</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#s">s</a></p></td>
<td><p>varchar(64)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>&quot;</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><a href="#token_key">token_key</a></td>
<td>varchar(100)</td>
<td><br />
</td>
<td><br />
</td>
<td>NO</td>
<td>''</td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><p><a href="#email">email</a></p></td>
<td><p>varchar(255)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>&quot;</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><a href="#reg_mail">reg_mail</a></td>
<td>varchar(255)</td>
<td><br />
</td>
<td><br />
</td>
<td>NO</td>
<td>''</td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><p><a href="#joindate">joindate</a></p></td>
<td><p>timestamp</p></td>
<td><p>signed</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>CURRENT_TIMESTAMP</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#last_ip">last_ip</a></p></td>
<td><p>varchar(15)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>127.0.0.1</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#failed_logins">failed_logins</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#locked">locked</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#last_login">last_login</a></p></td>
<td><p>timestamp</p></td>
<td><p>signed</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0000-00-00 00:00:00</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#online">online</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>signed</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#expansion">expansion</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>2</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#mutetime">mutetime</a></p></td>
<td><p>bigint(20)</p></td>
<td><p>signed</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><a href="#mutereason">mutereason</a></td>
<td>varchar(255)</td>
<td>signed</td>
<td><br />
</td>
<td>NO</td>
<td><p>&quot;</p></td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><a href="#muteby">muteby</a></td>
<td>varchar(50)</td>
<td>signed</td>
<td><br />
</td>
<td>NO</td>
<td><p>&quot;</p></td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><p><a href="#locale">locale</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#os">os</a></p></td>
<td><p>varchar(3)</p></td>
<td><p>signed</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>&quot;</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#recruiter">recruiter</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
</tbody>
</table>

## Description of the fields

### id

The unique account ID.

### username

The account username.

**NOTE**: Usernames are limited to 20 characters and are case insensitive.

### sessionkey

Session key negotiated between the client and the server. Allows clients to reconnect to their previous session.

### v
### s

Contains the verifier "v" and the salt "s" used to verify the username/password. See <https://en.wikipedia.org/wiki/Secure_Remote_Password_protocol> for more information on the SRP6 protocol.

**NOTE**: Passwords are limited to 16 characters and are case insensitive.

### **token\_key**

The authenticator key.

Key can be generated through the Google Authenticator API, a 3rd-party TOTP generator, or manually specified (must be a Base32-compliant expression that is 16 characters).

Implementation link on Wikipedia for the Google Authenticator API

<http://en.wikipedia.org/wiki/Google_Authenticator#Implementations>

### email

The e-mail address associated with this account.

### reg\_mail

The registration e-mail address associated with this account.

### joindate

The date when the account was created.

### last\_ip

The last IP used by the person who logged in the account.

### failed\_logins

The number of failed logins attempted on the account.

### locked

Boolean 0 or 1 controlling if the account has been locked or not. This can be controlled with the ".account lock" GM command. If locked (1), the user can only log in with their [last\_ip](#last_ip). If unlocked (0), a user can log in from any IP, and their last\_ip will be updated if it is different. ".Ban account" does not lock it.

### last\_login

The date when the account was last logged into.

### online

Boolean 0 or 1 controlling if the account is currently logged in and online.

### expansion

Integer 0, 1 or 2 controlling if the client logged in on the account has any expansions. (for example if client is TBC, but expansion is set to 0, it will not be able to enter outlands and etc.)

-   0 = Classic
-   1 = The Burning Crusade (TBC)
-   2 = Wrath of the Lich King (WotLK)

### mutetime

The time, in Unix time, when the account will be unmuted. To see when mute will be expired you can use this query:

``` cpp
SELECT FROM_UNIXTIME(`mutetime`);
```

### mutereason

The reason for the mute.

### muteby

The character name with the rights to the .mute command that give the mute.

### locale

The locale used by the client logged into this account. If multiple locale data has been configured and added to the world servers, the world servers will return the proper locale strings to the client. See [localization IDs](../../dbc/Localization_lang.md)

### os

Stores information about client's OS. Used by Warden system.

-   Win
-   Mac

### recruiter

The account ID of another account. Used for recuit-a-friend system. See [account.id](#id)
