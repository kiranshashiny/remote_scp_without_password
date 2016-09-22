# remote_scp_without_password

###  On the laptop :

        [user@server1]# ssh-keygen -t rsa -b 2048
        Generating public/private rsa key pair.
        Enter file in which to save the key (/root/.ssh/id_rsa): # Hit Enter
        Enter passphrase (empty for no passphrase): # Hit Enter
        Enter same passphrase again: # Hit Enter
        Your identification has been saved in /root/.ssh/id_rsa.
        Your public key has been saved in /root/.ssh/id_rsa.pub.

### On the remote server:

        Create a folder .ssh 
        Copy this id_rsa.pub to authorized_keys 
