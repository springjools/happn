# Happn Hack website

This folder contains a tiny website to play with the API.

Features:
* User information (self & others)
* List of notifications
* List of conversations & messages
* Accept user (aka like) / cancel accept
* List of accepted users
* Reject user / cancel reject
* List of rejected users
* Proof (experimental)
* List of achievement types (experimental)
* List of user's achievements (experimental)
* List of report types (experimental)
* List of user's reports (experimental)
* List of devices (experimental)

This website allows some operations that are not available in the official application GUI (_'cancel accept'_ and _'list of accepted users'_). It is also more convenient for browsing on desktop large screens.

## Installation

Requirements:
- any web server
- any recent PHP engine with CURL activated
- CURL library with SSL/TLS support

Just upload the content of the `/php` folder to your webserver.

The only configuration data is the Facebook token, that should be set in the `/lib/fb.json` file:
```
{"fb_token":"XXXXX"}

replace XXXX by your Facebook token
```

Write access shall be allowed to the following files to cache data between two HTTP requests:
- `/lib/auth.json` for authentication data
- `/lib/dev.json` for device data

Now open the `/site/index.php` main page in your browser, and enjoy !
