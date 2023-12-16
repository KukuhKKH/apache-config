## README.md

### Apache HTTP Server Configuration

This repository contains Apache HTTP server configuration files for managing server settings and hosts.

#### config.conf

The `config.conf` file is the main Apache HTTP server configuration file. It includes settings such as server root, module loading, user and group settings, and more. Below are some key configurations:

- **ServerRoot:** The top directory where server configuration, error, and log files are kept.
- **PHP Paths:** Paths to different PHP versions installed on the server.
- **Installation and Project Directories:** Directories for installation and project-related files.
- **Listen:** Specifies the IP address and port for Apache to listen on (default is 80).
- **Loaded Modules:** Various modules are loaded to enhance server functionality.
- **User and Group:** Specifies the user and group under which the server runs.
- **DocumentRoot:** The directory out of which documents are served.
- **ErrorLog and LogLevel:** Configuration for error logging.

#### host.conf

The `host.conf` file defines a host for a specific project with PHP configurations and URL rewriting. Key elements include:

- **ServerName and ServerAlias:** Defines the primary server name and additional aliases.
- **FcgidInitialEnv:** Sets the PHP runtime configuration for FastCGI.
- **DocumentRoot:** Specifies the root directory for serving documents.
- **Directory Configurations:** Defines access controls and URL rewriting for the project's frontend.
- **Alias and Directory for Backend:** Configures a backend alias and sets up PHP handling for the backend files.

### Usage

1. Clone this repository to your Apache HTTP server's configuration directory.
2. Modify the `config.conf` and `host.conf` files according to your server and project requirements.
3. Restart the Apache server for the changes to take effect.

### Important Notes

- Always make backups of your configuration files before making changes.
- Ensure that paths, permissions, and configurations are accurate to avoid issues.

For more details on Apache HTTP server configuration, refer to the [official documentation](http://httpd.apache.org/docs/2.4/).

Feel free to customize these files based on your specific server and project needs.
