ISPConfig 3 Installer
This script is based on dclardy64 and will will install all of the necessary programs and changes that need to be made to get ISPConfig running successfully. It uses the Perfect Server guide from Falko Timme as the guide. If you would like, you can manually install all of the things needed using the guides that he has provided. I am just trying to streamline the process.

There are some things to note.

I edited your fstab for the Quota installation. I only do this when you select to install Quota. This will not work on OpenVZ containers.
I make no guarantees that this will work for you. It should, but I am not responsible for anything that happens to your system. It should be installed on a clean install. If you choose not to follow these directions, you are responsible for the damage that you have done.
Debian Installation Instructions:

Run this command:

cd /tmp; wget --no-check-certificate -O ISPConfig3.tgz https://github.com/W3Space/ISPConfig-3-AutoInstaller/tarball/master; tar zxvf ISPConfig3.tgz; cd *Installer*; bash debian_install.sh
Answer the onscreen prompts. The script stops so that you can see the appropriate answers.

Enjoy the completed installation.

Ubuntu Installation Instructions:

Run this command:

cd /tmp; wget --no-check-certificate -O ISPConfig3.tgz https://github.com/W3Space/ISPConfig-3-AutoInstaller/tarball/master; tar zxvf ISPConfig3.tgz; cd *Installer*; bash ubuntu_install.sh
Answer the onscreen prompts. The script stops so that you can see the appropriate answers.

Enjoy the completed installation.

RoundCube Installation Instructions:

Please make sure that you have set the PHP Timezone in the appropriate files.
Run this command:

cd /tmp; wget --no-check-certificate -O ISPConfig3.tgz https://github.com/W3Space/ISPConfig-3-AutoInstaller/tarball/master; tar zxvf ISPConfig3.tgz; cd *Installer*; bash roundcube_install.sh
Enjoy the completed installation. For Apache, Roundcube can be accessed at /webmail for all hosts. For NginX, RoundCube can be accessed at webmail.* for all hosts. You will have to add this into DNS records.

TO DO

See what other options I can add. Please feel free to submit an issue for any ideas that you have.
