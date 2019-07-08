# node-webhook
little node app for testing webhooks

## How to

Download the `index.js` file and run:

```
$ node index.js
Server running at http://localhost:3000/
```

## Basic AUTH

Install necessary software:

`apt update && apt install -y nginx apache2-utils`

Generate a password for your user:

`htpasswd -b -c /etc/nginx/htpass user pass`

Configure NGINX by adding the file default.conf and linked it to sites enabled:

`vim /etc/nginx/sites-available/default`

paste the content and create the link:

`ln -s /etc/nginx/sites-available/default /etc/nginx/sites-enabled/default`

then reload NGINX:

`systemctl restart nginx`

## Credits

[StackOverflow](https://stackoverflow.com/a/46787467/3616147)
