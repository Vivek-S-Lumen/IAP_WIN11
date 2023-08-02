# Debian_Problems
Debian WSL config in windows 11

when ever we open Debian, If it is showing some error and asking for the `Press any key…..`
just unregister the existing WSL in windows 11 using power shell

 <img width="312" alt="wsl" src="https://github.com/Vivek-S-Lumen/Debian_Problems/assets/129164424/25e37b6f-abf8-4652-9a27-255e42af8687">

Now click on the Debian icon in the start menu now it will ask for the usrname/pass
by default we need to provide admin/admin

<img width="312" alt="debian_user" src="https://github.com/Vivek-S-Lumen/Debian_Problems/assets/129164424/3437dcee-0161-45c1-95ab-bb0f9a6885f5">

If we want to create a new user use this and configure the user with sudo grants use this

<img width="455" alt="create_user" src="https://github.com/Vivek-S-Lumen/Debian_Problems/assets/129164424/520c7a7a-fd6c-4513-914e-295a8920aa24">
 
Now update the Debian using the 
``` Sudo apt update ``` 
If it is giving any errors shown below 

<img width="312" alt="update_error" src="https://github.com/Vivek-S-Lumen/Debian_Problems/assets/129164424/f8dae6a7-ec5e-4a07-9b4d-a43ad59dd679">
 
use the following 
``` echo "nameserver 8.8.8.8" | sudo tee /etc/resolv.conf > /dev/null ```
 
It will resolve the above error and we can able to update.

To check debian current version use ```lsb_release -a```
