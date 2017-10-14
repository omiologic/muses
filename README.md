# Muses

Menu manager
Event manager
Reservation History
Customer manager

## Prerequisites

The following set of tools and configurations are required in order to build and run the application as a developer.

### 1. Install Xcode

* Open App Store.
* Search for Xcode.
* Double-click to install.


### 2. Install XCode Command Line Tools

* Open Terminal window.
* Type `xcode-select --install`
* Follow the prompts to install the command line developer tools
* It may be necessary to perform the following, depending on the order of installation: sudo xcode-select -switch /Library/Developer/CommandLineTools
* See Stack Overflow for more details

### 3. Install git

#### Mac**
  * `brew update`
  * `brew install git`
  * Follow [these instructions](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/) to add an ssh key to your bitbucket account.

#### CENTOS Linux**
  * By default CENTOS RPM repositories have only git 1.8.3.1, which is from June 2013 will not work for us.  We need git v2.
  * See [instructions here](https://tecadmin.net/install-git-2-x-on-centos-rhel-and-fedora/#)
  * We have to install from source
  * `yum install curl-devel expat-devel gettext-devel openssl-devel zlib-devel`
  * `yum install gcc perl-ExtUtils-MakeMaker`
  * `cd /usr/src`
  * `wget https://www.kernel.org/pub/software/scm/git/git-2.14.1.tar.gz`
  * `tar xzf git-2.14.0.tar.gz`
  * `cd git-2.14.1`
  * `make prefix=/usr/local/git all`
  * `make prefix=/usr/local/git install`
  * Add the following to `.bashrc` `export PATH=/usr/local/git/bin:$PATH`
  * `git --version`   > git version 2.14.1

### 4. Install Node Version Manager (nvm)

Nvm allows you to install multiple versions of Node.JS and switch between them easily. This is very important if you are maintaining multiple applications or multiple versions of the same application.

  * See installation instructions on the [GitHub nvm page](https://github.com/creationix/nvm)
  * Execute install script `curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash`
  * Verify that nvm is installed correctly `nvm ls`
  * You should not see any errors
  * Check the version `nvm --version` it should be 0.33.0


### 5. Install Node.JS

  * See latest version [here](https://nodejs.org/en/download)
  * Install version 6.11.3 `nvm install 6.11.3`
  * Set 6.11.3 to be the default version `nvm alias default 6.11.3`
  * Make sure everything is set correctly: `nvm ls`


## Frontend


