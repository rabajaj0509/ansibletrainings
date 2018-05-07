a) Create an inventory file that contains the ip address of 
the remote machine.

b) Create a ansible.cfg file that points to the inventory
file in the current directory and uses `sudo` method to 
become the `root` user.

c) Use the `yum` module to install the `httpd` package.

d) On the control node, create a a file `~/files/index,html`
with the content "This is a test page." 

e) Use the `copy` module to copy the `index.html` from the 
controlled node to the remote host at `/var/www/html/index.html`

f) Use the `service` module to start the `httpd` service.
