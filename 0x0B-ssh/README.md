File 0 - Write a Bash script that uses ssh to connect to your server using the private key ~/.ssh/school with the user ubuntu.

Requirements:

Only use ssh single-character flags
You cannot use -l
You do not need to handle the case of a private key protected by a passphrase

File 1 - Write a Bash script that creates an RSA key pair.

Requirements:

Name of the created private key must be school
Number of bits in the created key to be created 4096
The created key must be protected by the passphrase betty


File 2 - Your machine has an SSH configuration file for the local SSH client, let’s configure it to our needs so that you can connect to a server without typing a password. Share your SSH client configuration in your answer file.

Requirements:

Your SSH client configuration must be configured to use the private key ~/.ssh/school
Your SSH client configuration must be configured to refuse to authenticate using a password

File 3 - Now that you have successfully connected to your server, we would also like to join the party.

Add the SSH public key below to your server so that we can connect using the ubuntu user.

PROCEDURE

log into your server, using the ssh Ubuntu@yourserverip, then in the server terminal, type vi ~/.ssh/authorized_keys, enter insert mode then copy the key in the intranet  and paste it down below on a new line, the :wq to save then check your code on the intranet.

File 4 - Let’s practice using Puppet to make changes to our configuration file. Just as in the previous configuration file task, we’d like you to set up your client SSH configuration file so that you can connect to a server without typing a password.

Requirements:

Your SSH client configuration must be configured to use the private key ~/.ssh/school
Your SSH client configuration must be configured to refuse to authenticate using a password

to  created my ssh key:
1. Run the line "ip a" on your Ubuntu terminal to get your ip address.
2. Then run the line "ssh-keygen -t RSA -b 4096"
3. Click enter to use their default path to store the key
4. Set a password or click enter to leave it without a password
5. Copy the ssh  to your agent: run the line ssh-copy-id username@ip_address.
Username is the name of your Ubuntu terminal. When you open your terminal, the name on top of the terminal (without the @ that follows) is your username
IP address= you generated it at step 1.
6. Run the line: ssh username@ip_address
7. cd .ssh, ls , vi id_rsa.pub then copy the content and paste in your intranet profile for ssh key
