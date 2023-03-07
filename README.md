# ubuntu-lamp

Composer is failing.

$ sudo composer create-project drupal/recommended-project /var/www/drupal --no-dev
Do not run Composer as root/super user! See https://getcomposer.org/root for details
Continue as root/super user [yes]? yes
Creating a "drupal/recommended-project" project at "./drupal"
Info from https://repo.packagist.org: #StandWithUkraine
Installing drupal/recommended-project (10.0.4)
  - Installing drupal/recommended-project (10.0.4): Extracting archive
Created project in /var/www/drupal
Installing dependencies from lock file
Verifying lock file contents can be installed on current platform.
Your lock file does not contain a compatible set of packages. Please run composer update.

  Problem 1
    - drupal/core is locked to version 10.0.4 and an update of this package was not requested.
    - drupal/core 10.0.4 requires ext-dom * -> it is missing from your system. Install or enable PHP's dom extension.
  Problem 2
    - masterminds/html5 is locked to version 2.7.6 and an update of this package was not requested.
    - masterminds/html5 2.7.6 requires ext-dom * -> it is missing from your system. Install or enable PHP's dom extension.
  Problem 3
    - drupal/core 10.0.4 requires ext-dom * -> it is missing from your system. Install or enable PHP's dom extension.
    - drupal/core-recommended 10.0.4 requires drupal/core 10.0.4 -> satisfiable by drupal/core[10.0.4].
    - drupal/core-recommended is locked to version 10.0.4 and an update of this package was not requested.

To enable extensions, verify that they are enabled in your .ini files:
    - /etc/php/8.2/cli/php.ini
    - /etc/php/8.2/cli/conf.d/10-opcache.ini
    - /etc/php/8.2/cli/conf.d/10-pdo.ini
    - /etc/php/8.2/cli/conf.d/20-apcu.ini
    - /etc/php/8.2/cli/conf.d/20-calendar.ini
    - /etc/php/8.2/cli/conf.d/20-ctype.ini
    - /etc/php/8.2/cli/conf.d/20-exif.ini
    - /etc/php/8.2/cli/conf.d/20-ffi.ini
    - /etc/php/8.2/cli/conf.d/20-fileinfo.ini
    - /etc/php/8.2/cli/conf.d/20-ftp.ini
    - /etc/php/8.2/cli/conf.d/20-gettext.ini
    - /etc/php/8.2/cli/conf.d/20-iconv.ini
    - /etc/php/8.2/cli/conf.d/20-phar.ini
    - /etc/php/8.2/cli/conf.d/20-posix.ini
    - /etc/php/8.2/cli/conf.d/20-readline.ini
    - /etc/php/8.2/cli/conf.d/20-shmop.ini
    - /etc/php/8.2/cli/conf.d/20-sockets.ini
    - /etc/php/8.2/cli/conf.d/20-sysvmsg.ini
    - /etc/php/8.2/cli/conf.d/20-sysvsem.ini
    - /etc/php/8.2/cli/conf.d/20-sysvshm.ini
    - /etc/php/8.2/cli/conf.d/20-tokenizer.ini
You can also run `php --ini` in a terminal to see which files are used by PHP in CLI mode.
Alternatively, you can run Composer with `--ignore-platform-req=ext-dom` to temporarily ignore these required extensions.

