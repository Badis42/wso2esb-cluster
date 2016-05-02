FROM dockerhub.private.wso2.com/ubuntu:14.04
MAINTAINER lakmal

EXPOSE 80

RUN apt-get install subversion apache2 libapache2-svn apache2-utils -y
RUN mkdir -p /var/svn/repo
RUN svnadmin create /var/svn/repo
RUN chown -R www-data:www-data /svn/repos/repo
COPY repo.conf /etc/apache2/sites-enable/
COPY  svnpasswd /etc/

CMD ["/var/www/run_apache.sh"]

