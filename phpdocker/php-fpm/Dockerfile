FROM phpdockerio/php71-fpm:latest

# Install selected extensions and other stuff
RUN apt-get update \
    && apt-get -y --no-install-recommends install  php7.1-bcmath php7.1-cli php7.1-common php7.1-curl  php7.1-fpm php7.1-gd php7.1-json php7.1-ldap php7.1-mbstring php7.1-mcrypt  php7.1-opcache php7.1-pgsql php7.1-pspell php7.1-readline php7.1-recode php7.1-redis php7.1-sqlite3 php7.1-tidy php7.1-xml php7.1-xmlrpc php7.1-zip nginx nginx-extras postgresql postgresql-client postgresql-contrib redis-server redis-tools supervisor \
    && apt-get clean; rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*


WORKDIR "/application"
