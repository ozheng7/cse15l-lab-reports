## CSE 15L Week 2 Lab Report 1
Oscar Zheng, A16880333

- **Installing VS Code**
  - This is not that hard, just go to the VSCode [site](https://code.visualstudio.com/) and download VSCode.
  - After installing, you should see this front page.
    - ![Image](https://cdn.discordapp.com/attachments/856335317203681280/962143518267158528/unknown.png)
-------------------------------------------------------------------------------------------------------------------
- **Remotely Connecting**
  - To remotely connect to the UCSD lab computer, open a terminal and type these commands
   - `ssh cse15lsp22ajw@ieng6.ucsd.edu`
   - *type in your password*
    - ![Image](https://cdn.discordapp.com/attachments/856335317203681280/962149296399069264/unknown.png)
--------------------------------------------------------------------------------------------------------------------
- **Trying Some Commands**
  - You can try some commands and mess around with the different list commands.
  - ![Image](https://cdn.discordapp.com/attachments/856335317203681280/962149779108941894/unknown.png)
---------------------------------------------------------------------------------------------------------------------
- **Moving Files with `scp`**
  - You can move files from your local system to the computer that you are connected to within the terminal.
    - Make a file on your system that you want to move to the remote system
    - Type this command 
      - `scp WhereAmI.java cs15lsp22zz@ieng6.ucsd.edu:~/`
    - You will be asked to enter your password and after, you can login to the remote computer again and use `ls` to check if the file was sucessfully copied.
    - ![Image](https://cdn.discordapp.com/attachments/856335317203681280/962150405037494312/unknown.png)
---------------------------------------------------------------------------------------------------------------------
- **Setting an SSH Key**
  -  Setting a key allows you to sign onto the remote desktop without the password, as long as you have the key on your local machine.
  -  On your local machine
    - ```$ssh-keygen
      Generating public/private rsa key pair.
      Enter file in which to save the key (/Users/<user-name>/.ssh/id_rsa): /Users/<user-name>/.ssh/id_rsa
      Enter passphrase (empty for no passphrase):
      ```
    - *do not add a passphrase*
    - ```Enter same passphrase again: 
      Your identification has been saved in /Users/<user-name>/.ssh/id_rsa.
      Your public key has been saved in /Users/<user-name>/.ssh/id_rsa.pub.
      The key fingerprint is:
      SHA256:jZaZH6fI8E2I1D35hnvGeBePQ4ELOf2Ge+G0XknoXp0 <user-name>@<system>.local
      ```
    - ![Image](https://cdn.discordapp.com/attachments/856335317203681280/962164594024017960/unknown.png)

------------------------------------------------------------------------
- **Optimizing Remote Running**
  - To understand the change that was made to the process of accessing your remote desktop, you can try and time yourself copying files over from one machine to the other. 
  - Try to copy a file without the password on a new machine and then try again on the machine with the passkey on it. 
  - How fast are you on the machine with the passkey on it? What about when manually typing in your passkey?
  - ![Image](https://cdn.discordapp.com/attachments/852041958067273761/965391214713118780/unknown.png)
  - ![Image](https://cdn.discordapp.com/attachments/856335317203681280/962168172172157019/unknown.png)

