ergw-gtp-c-node
===============

[![Build Status](https://travis-ci.org/travelping/ergw-gtp-c-node.svg?branch=master)](https://travis-ci.org/travelping/ergw-gtp-c-node)

OTP application to package a erGW GTP-C Node.

Installing on Ubuntu 16.04
--------------------------

Package for Ubuntu 16.04 are build on every commit to this repository and uploaded to bintray. In order to install them do this:

    sudo echo "deb http://ppa.launchpad.net/ergw/xenial/ubuntu xenial main" > /etc/apt/sources.list.d/ergw-xenial-ppa.list
    sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 58A14C3D
    curl -s https://packagecloud.io/install/repositories/ergw/ci/script.deb.sh | sudo bash
    apt-get -y install ergw-gtp-c-node

After installation adjust /opt/ergw-gtp-u-node/releases/<version>/sys.config

Build
-----

    $ rebar3 compile
