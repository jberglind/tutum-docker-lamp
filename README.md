Docker LAMP image
=================

###Note, this is a fork from tutum's LAMP repository. 

This is a general LAMP stack used for local Drupal/general PHP development with some added features such as php5-gd. I've also added another user with permissions to administer the drupal DB, with username: `drupaluser` with the uncrackable password: `password`.

**Please do not even consider using this docker image for deployments, this is ment to be a local development environment.**


Usage
-----

1. Build docker image: `docker build -t johanberglind/lamp .`


2. Run image: `docker run -d -v /webapp-folder:/app  -p 80:80 -p 3306:3306 johanberglind/lamp`

