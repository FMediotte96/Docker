FROM centos:7

LABEL version=1.0
LABEL description="This is an apache image"
LABEL vendor=fmediotte

RUN \
	yum -y install \
	httpd \
	php \
	php-cli \
	php-common 

RUN echo "<?php phpinfo(); ?>" > /var/www/html/index.php
	
CMD apachectl -DFOREGROUND
