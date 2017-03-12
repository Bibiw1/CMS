# CMS
simple cms php 

INSTALLING

You need: 
1) installed WEB-server(apache2; nginx; IIS; etc.)
2) installed php5 module for your server
3) mysql and mysql module for php

PHP need to be setted for translating files *.php and *.html

Copy all files of project to your root site folder.

You need to rewrite config.php for your admin login/password, mysql login/password and other settings.

Run commands in mysql shell:

<code>
mysql> CREATE DATABASE cms;

DROP TABLE IF EXISTS articles;

CREATE TABLE articles
(
  id              smallint unsigned NOT NULL auto_increment,
  publicationDate date NOT NULL,
  title           varchar(255) NOT NULL
  summary         text NOT NULL,
  content         mediumtext NOT NULL,
  
  PRIMARY KEY     (id)
);</code>

Continue, try launch it: http://127.0.0.1/
