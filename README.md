Firefox Developer Edition package for Debian / Ubuntu
=====================================================

![FirefoxDeveloperEdition](https://raw.githubusercontent.com/VitexSoftware/FirefoxDeveloperEditionDeb/master/mozicon300.png "DeveloperEdition logo")

A version of Firefox that's tailored for web developers.

Building package
----------------

    apt-get -y install devscripts dpkg-dev
    git clone https://github.com/VitexSoftware/FirefoxDeveloperEditionDeb.git
    debuild -i -us -uc -b


Installation
------------

Download from https://www.vitexsoftware.cz/pool/main/n/DeveloperEdition/firefox-devedition_1.0.0_all.deb or Build package. Then install:

    gdebi firefox-devedition_1.0.0_all.deb


Or you can use repo:

    wget -O - http://v.s.cz/info@vitexsoftware.cz.gpg.key|sudo apt-key add -
    echo deb http://v.s.cz/ stable main > /etc/apt/sources.list.d/vitexsoftware.list
    apt update
    apt install firefox-devedition

Testing
-------

    vagrant up
    vagrant ssh
    sudo apt install xfce4
    startxfce4


![Vagrant Test](https://raw.githubusercontent.com/VitexSoftware/FirefoxDeveloperEditionDeb/master/vagrantubuntu.png "DeveloperEdition in Ubuntu")
