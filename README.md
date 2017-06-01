<p align="center">
  <img alt="Node JS by Omal Perera" src="https://nodejs.org/static/images/logo-light.svg" width="300"/>
</p>

# Node.JS Uni Session
A comprehensive guide to help you learn Node.Js with basic JavaScript &amp; strong basic architectural knowledge.

# Installing Node.Js
* [Linux](#installing-on-linux)
* [Mac](#installing-on-mac)
* [Windows](#installing-on-windows)


# Installing Visual Studio Code
* [Linux](#installing-on-linux)
* [Mac](#installing-on-mac)
* [Windows](#installing-on-windows)


## Session Lineup
1. Basic Concepts
2. Handling Multiple Requests
3. Understanding References to Objects
4. Prototype
5. Modules
6. Creating a Basic Server
7. Express
8. Understanding app.js

# Installing Node.Js

## Installing on Linux
You can install a pre-built version of node.js via [the downloads page](http://nodejs.org/download/) available in a **.tar.gz**.
Or you can use the automatic bash [Installer](https://github.com/taaem/nodejs-linux-installer/releases).

## Installing on Mac
You can install a pre-built version of node.js via [the downloads page](http://nodejs.org/download/) using a **.pkg** or available in a **.tar.gz**.

## Installing on Windows
You can install a pre-built version of node.js via [the downloads page](http://nodejs.org/download/) using a **.exe** or a **.msi**.

<br><br><br>



# Installing Visual Studio Code

## Installing on Linux

**Debian and Ubuntu based distributions**

The easiest way to install for Debian/Ubuntu based distributions is to download and install the .deb package (64-bit) either through the graphical software center if it's available or through the command line with:

<pre>
sudo dpkg -i <file>.deb
sudo apt-get install -f # Install dependencies
</pre>

Installing the .deb package will automatically install the apt repository and signing key to enable auto-updating using the regular system mechanism. Note that 32-bit and .tar.gz binaries are also available on the download page.

The repository and key can also be installed manually with the following script:

<pre>
curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg
sudo mv microsoft.gpg /etc/apt/trusted.gpg.d/microsoft.gpg
sudo sh -c 'echo "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main" > /etc/apt/sources.list.d/vscode.list'
</pre>
Then update the package cache and install the package using:

</pre>
sudo apt-get update
sudo apt-get install code # or code-insiders
</pre>

**RHEL, Fedora and CentOS based distributions**
We currently ship the stable 64-bit VS Code in a yum repository, the following script will install the key and repository:

<pre>
sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
sudo sh -c 'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/vscode.repo'
</pre>

Then update the package cache and install the package using dnf (Fedora 22 and above):

<pre>
dnf check-update
sudo dnf install code
</pre>

Or on older versions using yum:

<pre>
yum check-update
sudo yum install code
</pre>

**openSUSE and SLE based distributions**
The yum repository above also works for openSUSE and SLE based systems, the following script will install the key and repository:

<pre>
sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
sudo sh -c 'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/vscode.repo'
</pre>
Then update the package cache and install the package using:

<pre>
sudo zypper refresh
sudo zypper install code
</pre>

**AUR package for Arch Linux**
There is a community maintained Arch User Repository (AUR) package for VS Code.

Installing .rpm package manually
The .rpm package (64-bit) can also be manually downloaded and installed, however auto-updating won't work unless the repository above is installed. Once downloaded it can be installed using your package manager, for example with dnf:

<pre>
sudo dnf install <file>.rpm
Note that 32-bit and .tar.gz binaries are are also available on the download page.
</pre>

## Installing on Mac
You can install a pre-built version of node.js via [the downloads page](http://nodejs.org/download/) using a **.pkg** or available in a **.tar.gz**.

## Installing on Windows
You can install a pre-built version of node.js via [the downloads page](http://nodejs.org/download/) using a **.exe** or a **.msi**.

<hr>
