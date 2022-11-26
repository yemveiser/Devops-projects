## Install Python

sudo yum search python3
sudo yum install python3
sudo yum upgrade python3

## Install NTP using chronyd
dnf install chrony
systemctl start chronyd
systemctl status chronyd
systemctl enable chronyd
vi /etc/chrony.conf
allow <NTP-server-ip>>

## Install Epel-release
yum -y install https://dl.fedoraproject.org/pub/epel/epel-release-latest-8.noarch.rpm

##Install Htop
sudo yum install htop