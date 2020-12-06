# gnufinder
A bash script I made to help find things easier.
### if you would like to use the wikipedia functions of this tool please do the following installs if not already done.
sudo apt install nodejs npm     #Debian/Ubuntu
sudo yum install nodejs npm     #RHEL/CentOS
sudo dnf install nodejs npm     #Fedora 22+
##############################################
###once you make sure you have the updated version of nodejs and npm please run
sudo npm install wikit -g

#################################################################

gnufinder -h to list arguments available. At least one argument must be given.

#####################################################################################
 Please make sure you have the following or something of your own to constitute the dda command or you should not use the -d option. 
I believe dda is one of the snap packages ubuntu gives you now not sure on other releases and either way it can be installed with;
sudo snap install dda 
If you do not have snap installed; 
sudo apt install snap
#######################################################################################
#!/usr/bin/env python3
# EASY-INSTALL-ENTRY-SCRIPT: 'duckduckgoapi==0.0.2','console_scripts','dda'
__requires__ = 'duckduckgoapi==0.0.2'
import re
import sys 
from pkg_resources import load_entry_point

if __name__ == '__main__':
    sys.argv[0] = re.sub(r'(-script\.pyw?|\.exe)?$', '', sys.argv[0])
    sys.exit(
        load_entry_point('duckduckgoapi==0.0.2', 'console_scripts', 'dda')()
    )   

