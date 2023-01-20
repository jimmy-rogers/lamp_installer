LAMP Stack Automation Script

This script automates the installation of the LAMP stack (Linux, Apache, MySQL, and PHP) on Red Hat servers. It also includes optional installation of additional packages such as pip and pipenv, as well as expect. The script also includes the configuration of firewall to open port 80.
Usage

    Make the script executable by running chmod +x lamp_install_rhel
    Run the script with ./lamp_install_rhel

What the script does

    Installs pip
    Installs pipenv
    Installs Apache web server if not already installed
    Installs MariaDB server if not already installed
    Starts the MariaDB service
    Installs expect if not already installed
    Runs the mysql_secure_installation script with expect
    Installs PHP and related packages if not already installed
    Starts the Apache service
    Configures firewall to open port 80
    Prints "Done" message upon successful completion

Please note that the script assumes that you are running it with sufficient permissions (e.g. as a root user) to install packages and configure services.
Future plans

This script is designed for Red Hat servers, but will be expanded to support other distros such as Ubuntu.
