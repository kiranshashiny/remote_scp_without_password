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
            
            Set the permissions as shown - or else it wont work

                [dpeuser@dpev559 ~]$ ls -ld .ssh/
                drwx------ 2 dpeuser dpeuser 28 Sep 22 05:34 .ssh/


        Copy this id_rsa.pub from source server above, to  'authorized_keys' file on the remote server.

        [dpeuser@dpev559 ~]$ vi authorized_keys 
         
        [dpeuser@dpev559 .ssh]$ ls -ld authorized_keys 
        -rw------- 1 dpeuser dpeuser 416 Sep 22 05:31 authorized_keys
