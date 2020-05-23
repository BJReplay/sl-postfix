# Docker Image for SimpleLogin Postfix

**WARNING: This is Work In Progress. Don't use it on PROD yet!!**

No official Postfix image, tailor-made for [SimpleLogin](https://simplelogin.io/),
currently exists.

Let's fix that, by providing to the community something very lightweight and simple to use 💖

Can be configured with the following environment variables:

Setting     | Description
----------- | -------------------------------------------
**ALIASES_DEFAULT_DOMAIN** | Default domain to use for your aliases.
**DB_HOST** | Where is hosted your SimpleLogin PostgreSQL database.
**DB_USER** | User to connect to the database.
**DB_PASSWORD** | User's password to connect to the database.
**DB_NAME** | Name of the database.
**EMAIL_HANDLER_HOST** | Where is hosted your SimpleLogin email handler instance.
**POSTFIX_FQDN** | Fully Qualified Domain Name of your Postfix instance (i.e., the MX server address you configured in your DNS zone for your **ALIASES_DEFAULT_DOMAIN**).

Used by and made for [Kloügle](https://github.com/arugifa/klougle), the Google
alternative automated with [Terraform](https://www.terraform.io/).
