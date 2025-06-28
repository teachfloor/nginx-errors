# Teachfloor Nginx error pages

A custom set of 4xx and 5xx error pages for Nginx.

## Installation

1. Navigate into Nginx's default document directory:
	```
    cd /usr/share/nginx/html
    ```

2. Clone the repository:
	```
    git clone https://github.com/bartosjiri/nginx-errors.git
    ```

3. Add the custom error pages to the server's default configuration in `/etc/nginx/sites-enabled/default` file:
	```
    server {
    ...
    include /usr/share/nginx/html/nginx-errors/nginx-errors.conf
    }
    ```

4. Verify the configuration and reload Nginx:
	```
    sudo nginx -t
    sudo service nginx reload
    ```