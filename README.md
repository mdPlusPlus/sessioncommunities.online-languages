# https://sessioncommunities.online language associations
Repository to crowdsource the language association for https://sessioncommunities.online/
## Contribute
Communities are identified by a string consisting of the concatenation of their `token`, the `plus sign` (+), and the `first four characters of the hexadecimal public key` of their server.  
To add a new server you add a new `array()` with the name `$lanuages_xxx`, where `xxxx` are the first four characters of the hexadecimal public key.
### Example
Given the following `invite link`: http://open.getsession.org/session?public_key=a03c383cf63c3c4efe67acc52112a6dd734b3a946b9545f488aaa93da7991238  
the `token` is "session",  
the hexadecimal public key is "a03c383cf63c3c4efe67acc52112a6dd734b3a946b9545f488aaa93da7991238",  
so the unique identifier of the "session" Community on the server "http://open.getsession.org/" is `session+a03c`.

To change the language of `session+a03c` you change the value of `session+a03c` in the array called `$languages_a03c`

```
	// https://open.getsession.org/
	$languages_a03c = array(
		"crypto+a03c"                   => "🇬🇧",
		"lokinet+a03c"                  => "🇬🇧",
		"oxen+a03c"                     => "🇬🇧",
		"session-farsi+a03c"            => "🇮🇷",
		"session-updates+a03c"          => "🇬🇧",
		"session+a03c"                  => "🇬🇧"
	);
```
