# RabbitMQ

**1. Preparation**


yum install socat logrotate -y

yum install wget -y


**2. Installing on RPM based Linux**
Support (RedHat Enterprise Linux, CentOS, Fedora, openSUSE)

yum install -y erlang-23.3.4.5-1.el7.x86_64.rpm

yum install -y rabbitmq-server-3.9.0-1.el7.noarch.rpm


**3. Run RabbitMQ Server**

Start the Server
The server is not started as a daemon by default when the RabbitMQ server package is installed. To start the daemon by default when the system boots, as an administrator run

chkconfig rabbitmq-server on

As an administrator, start and stop the server as usual, e.g. using service:

/sbin/service rabbitmq-server start

/sbin/service rabbitmq-server status

/sbin/service rabbitmq-server stop
If the service tool is not installed on the system, it can be installed using yum:

yum -y install initscripts


**Reference**: 
https://www.rabbitmq.com/install-rpm.html

**RabbitMQ Erlang Version Requirements**:
https://www.rabbitmq.com/which-erlang.html
