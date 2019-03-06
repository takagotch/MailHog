### MailHog
---
https://github.com/mailhog/MailHog

```
gem install mailcatcher
mailcatcher

rvm default@mailcatcher --create do gem install mailcatcher
rvm wrapper default@mailcatcher --no-prefix mailcatcher catchmail

sendmail_path = /usr/local/bin/mhsendmail
sendmail_path = /usr/sbin/sendmail -S mail:1025

/usr/sbin/sendmail -S mail:1025
```

```rb
config.action_mailer.delivery_method = :smtp
config.action_mailer.smtp_settings = { :address => "localhost", :port => 1025 }
```

```php
sendmail_path = /usr/bin/env catchmail -f some@from.address
php_admin_value sendmail_path "/usr/bin/env catchmail -f some@from.address"
sendmail_path = /usr/bin/env catchmail --smtp-ip 192.168.0.1 --smtp-port 10025 -f someWfrom.address
```

```py
if DEBUG:
  EMAIL_HOST = '127.0.0.1'
  EMAIL_HOST_USER = ''
  EMAIL_HOST_PASSWORD = ''
  EMAIL_PORT = 1025
  EMAIL_USE_TLS = False
```
