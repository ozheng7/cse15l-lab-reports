## CSE 15L Week 2 Lab Report 1
Oscar Zheng, A16880333

- **Installing VS Code**
  - This is not that hard, just go to the VSCode [site](https://code.visualstudio.com/) and download VSCode.
  - After installing, you should see this front page.
    - ![Image](https://cdn.discordapp.com/attachments/856335317203681280/962143518267158528/unknown.png)

- **Remotely Connecting**
  - To remotely connect to the UCSD lab computer, open a terminal and type these commands
   - ssh cse15lsp22ajw@ieng6.ucsd.edu
   - *type in your password*
    - ![Image](https://cdn.discordapp.com/attachments/856335317203681280/962149296399069264/unknown.png)

- **Trying Some Commands**
  - You can try some commands and mess around with the different list commands.
  - ![Image](https://cdn.discordapp.com/attachments/856335317203681280/962149779108941894/unknown.png)

- **Moving Files with `scp`**
  - You can move files from your local system to the computer that you are connected to within the terminal.
    - Make a file on your system that you want to move to the remote system
    - Type this command 
      - `scp WhereAmI.java cs15lsp22zz@ieng6.ucsd.edu:~/`
    - You will be asked to enter your password and after, you can login to the remote computer again and use `ls` to check if the file was sucessfully copied.
    - ![Image](https://cdn.discordapp.com/attachments/856335317203681280/962150405037494312/unknown.png)

- **Setting an SSH Key**
  -  
