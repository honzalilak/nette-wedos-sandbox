Nette Framework Sandbox for 3rd domain level on Wedos hosting 
=============================================================
The basic nette sandbox prepared to be used on a subdomain on wedos.com hosting (eg. sandbox.yourdomain.com).

Installation
------------
1. Upload this project to your 'subdom' folder.
2. Set up privilege for folder `log/` and `temp/`.
3. Locate the `www` folder in your browser.

Are you interested in [dibi](http://dibiphp.com/), a database layer which is at the moment more reliable than [Nette\Database](http://doc.nette.org/cs/database)? Then you might find helpful [Nette Framework Sandbox extended with dibi](https://github.com/xlilien/nette-sandbox)


Find below the original Nette Sandbox [readme](https://github.com/nette/sandbox/blob/master/readme.md).

What is [Nette Framework](http://nette.org)?
------------------------

Nette Framework is a popular tool for PHP web development. It is designed to be
the most usable and friendliest as possible. It focuses on security and
performance and is definitely one of the safest PHP frameworks.

Nette Framework speaks your language and helps you to easily build better websites.


Installing
----------

The best way to install Nette Framework is to download latest package
from http://nette.org/download or create new project using
[Composer](http://doc.nette.org/composer):

	curl -s http://getcomposer.org/installer | php
	php composer.phar create-project nette/sandbox myApp dev-release-2.0.x
	cd myApp

Make directories `temp` and `log` writable. Navigate your browser
to the `www` directory and you will see a welcome page. PHP 5.4 allows
you run `php -S localhost:8888 -t www` to start the webserver and
then visit `http://localhost:8888` in your browser.


It is CRITICAL that file `app/config/config.neon` & whole `app`, `log`
and `temp` directory are NOT accessible directly via a web browser! If you
don't protect this directory from direct web access, anybody will be able to see
your sensitive data. See [security warning](http://nette.org/security-warning).