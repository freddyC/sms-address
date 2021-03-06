
### Basic Usage

sms-address returns an email address that can be used to send an SMS
message.

It takes two arguments, phone number, and carrier.

```javascript
var sms = require('sms-address');

var email = sms('123-456-7890', 'Verizon');

email === '1234567890@vtext.com';
```

sms-address also exports the carriers it supports. US only for now.

```javascript
var sms = require('sms-address');

console.log(sms.carriers)

// outputs:
{
  "Alaska Communications": "msg.acsalaska.com",
  "Alltel": "sms.alltelwireless.com",
  "Ameritech": "paging.acswireless.com",
  "AT&T": "txt.att.net",
  "BellSouth": "bellsouth.cl",
  "Bluegrass Cellular": "sms.bluecell.com",
  // and so on and so forth ...
```
