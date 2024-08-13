## Nginx Important Directories and Files

### Content Directory
- **`/var/www/html`**: This directory contains the actual web content served by Nginx. By default, it includes the default Nginx page. You can change the content directory by modifying the Nginx configuration files.

### Server Configuration
- **`/etc/nginx`**: The main Nginx configuration directory. All Nginx configuration files are located here.
- **`/etc/nginx/nginx.conf`**: The main Nginx configuration file for global settings. Changes to this file affect the global configuration of Nginx.
- **`/etc/nginx/sites-available/`**: This directory holds per-site server block configurations. Nginx does not use these configurations directly until they are linked to the `sites-enabled` directory.
- **`/etc/nginx/sites-enabled/`**: This directory contains links to the server block configuration files from `sites-available` that are currently enabled.
- **`/etc/nginx/snippets`**: Contains reusable configuration fragments that can be included in other Nginx configuration files. This helps to avoid repetition of configuration segments.

### Server Logs
- **`/var/log/nginx/access.log`**: Records every request made to your web server, unless otherwise configured.
- **`/var/log/nginx/error.log`**: Logs any errors encountered by Nginx.
