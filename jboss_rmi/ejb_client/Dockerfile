FROM tutum/jboss:as5
MAINTAINER Che Yang <cheyang@163.com>

ADD packages/run.sh /
ADD packages/ear/jboss-rmi.ear  /jboss-5.1.0.GA/server/all/deploy/
ADD packages/ejb-war/common/monit.jar /jboss-5.1.0.GA/server/all/lib/

RUN chmod +x /*.sh

EXPOSE 8080 1099 3528

CMD ["/run.sh"]



