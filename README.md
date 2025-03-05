# XUI
Just a suggestion for installing the panel. It works perfect with MariaDB version 10.5.xx so, normally when you install it choses 10.3 or 10.6 or random and that causes stopping in backup creation and restoration within the panel. So, would suggest to install MariaDB 10.5.XX version earlier and lock it not to be removed or updated so, when you install the panel it will be done within the same version.

Follow steps to install MariaDB 10.5.XX before starting the installation:

sudo apt update ;  apt-get install software-properties-common dirmngr -y ; sudo apt-key adv --fetch-keys 'https://mariadb.org/mariadb_release_signing_key.asc' ; sudo add-apt-repository 'deb [arch=amd64,arm64,ppc64el] http://mirror.lstn.net/mariadb/repo/10.5/ubuntu focal main' ; sudo apt-get install mariadb-server=1:10.5.27+maria~ubu2004 mariadb-client=1:10.5.27+maria~ubu2004 ﻿

apt-mark hold maria*


Fresh Installation Script

Copy and run following command for version 1.5.5 Official.

wget "https://update.xui.one/XUI_1.5.5.zip" -O /tmp/XUI_1.5.5.zip ; cd /tmp ; apt update ; apt install zip unzip -y ; unzip XUI_1.5.5.zip ; ./install

Copy and run following command 1.5.12 Beta.

wget "https://update.xui.one/XUI_1.5.12.zip" -O /tmp/XUI_1.5.12.zip ; cd /tmp ; apt update ; apt install zip unzip -y ; unzip XUI_1.5.12.zip ; ./install

Copy and run following command 1.5.13 NEW

wget "https://update.xui.one/XUI_1.5.13.zip" -O /tmp/XUI_1.5.13.zip ; cd /tmp ; apt update ; apt install zip unzip -y ; unzip XUI_1.5.13.zip ; ./install


When you’ve installed 1.5.13 update your load balancers from the Servers page. Once all load balancers are updated or reinstalled, click the red Lock icon in the top right and then select Regenerate Security Key. This will increase security and ensure nobody can replicate your streaming key and do anything malicious.

Now, it will ask you to add the license key to it, add it and then you’ll be redirected to creation of fresh new admin, create and you’re in.

So, that hard was your panel installation. You can easily connect unlimited loadbalancers to it, the auto LB installation do work perfectly.



ALTERNATE WAY:

Instructions:
1. Download and install XUI one latest version (1.5.5) - https://update.xui.one/XUI_1.5.12.zip

Done!
