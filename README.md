# odoo10-install


sudo apt-get update && sudo apt-get upgrade -y
sudo apt-get install npm -y && sudo npm install -g less less-plugin-clean-css -y
sudo apt-get install python-dateutil -y && sudo apt-get install python-psycopg2 -y 
sudo apt-get install python-dateutil python-docutils python-feedparser python-jinja2 python-ldap python-libxslt1 python-lxml python-mako python-mock python-openid python-psycopg2 python-psutil python-pybabel python-pychart python-pydot python-pyparsing python-reportlab python-simplejson python-tz python-unittest2 python-vatnumber python-vobject python-webdav python-werkzeug python-xlwt python-yaml python-zsi poppler-utils python-pip python-pypdf python-passlib python-decorator gcc python-dev mc bzr python-setuptools python-markupsafe python-reportlab-accel python-zsi python-yaml python-argparse python-openssl python-egenix-mxdatetime python-usb python-serial lptools make python-pydot python-psutil python-paramiko poppler-utils python-pdftools antiword python-requests python-xlsxwriter python-suds python-psycogreen python-ofxparse python-gevent

sudo apt install postgresql -y 

sudo apt-get install python-pip

pip install passlib
pip install -U Werkzeug
pip install lxml
pip install decorator
pip install pyyaml
pip install Python-Chart
pip install reportlab
pip install "Werkzeug==0.16.1"
pip install psutil
pip install jinja2
pip install mock
pip install requests
pip install pyPdf
pip install prettytable Mako pyaml dateutils --upgrade

#usuaio odoo para linux
useradd -m -g sudo -s /bin/bash odoo
passwd odoo



# se conecta ocn el usuario odoo


mkdir odoo-dev
cd odoo-dev/

git clone --depth=1 --branch=10.0 https://github.com/odoo/odoo.git /opt/odoo
git clone https://github.com/odoo/odoo.git -b 10.0 --depth=1  




Quick fix
Simply copy and paste this in your terminal:
1) sudo su postgres
2) createuser odoo -s
3) psql template1
4) \q
5) exit





PATH=/sbin:/bin:/usr/sbin:/usr/bin:/usr/local/bin
DAEMON=/usr/bin/odoo
NAME=odoo
DESC=odoo
CONFIG=/etc/odoo.conf
LOGFILE=/var/log/odoo/odoo-server.log
PIDFILE=/var/run/${NAME}.pid
USER=root
export LOGNAME=$USER
/

update-rc.d odoo defaults
