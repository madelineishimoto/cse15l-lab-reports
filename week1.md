# Week 1 Lab 
![Image](https://user-images.githubusercontent.com/114532765/195748694-d515bfed-c083-4d3e-ae67-47b69abb4b7d.png)

After you have set up your new password for your CS15L account, download Visual Studio Code. You can find it by searching VS code up on your browser. The image on top shows what it should look like before you download VScode. 

![Image](https://user-images.githubusercontent.com/114532765/195757162-1c01913a-33d6-43b4-93bb-40b643f3301c.png)
Your screen should look similar to this after you have downloaded vscode. Next, open a new terminal by clicking terminal at the top, then new terminal. 

![Image](https://user-images.githubusercontent.com/114532765/195757521-a4b5e122-00f5-4d4a-a336-03ca4a772458.png)
Next, type in ssh cs15lfa22(your specific two letters that were assigned to your account)@ieng.ucsd.edu. It will then ask for your password. Type in your new password. 
Here, you are connecting remotely.

![Image](https://user-images.githubusercontent.com/114532765/195757654-5fb9629e-b337-4ec2-962b-4dd4d7d5a37f.png)
This is what it looks like when you are logged in. Now you can start running the commands. 

![Image](https://user-images.githubusercontent.com/114532765/195757967-4864cd17-0037-41dc-9898-8dd22cd8e6d6.png)
There is a list of different commands you can try typing in the terminal 

![Image](https://user-images.githubusercontent.com/114532765/195758192-e288bc70-88ee-4fbe-bdf9-891676fe605f.png)
Here is an example of what your terminal should look like after running a command (la -a in this case) 

![Image](https://user-images.githubusercontent.com/114532765/195758343-ac563167-152d-4607-86f3-c410cef4f6cb.png)

![Image](https://user-images.githubusercontent.com/114532765/195758629-7dd15da6-45fe-4af4-9b9f-462293e4941c.png)
Once you’ve created a new file called WhereAmI.java, run the following commands. 
Run this scp command in the terminal. It will ask you to type your password in order to login. I typed in the directory path, which was each of the folders that the file was in. If successful, the terminal will show how long it took to compile and at what percentage complete it is. This is also where you are moving files over ssh using SCP. 

![Image](https://user-images.githubusercontent.com/114532765/195758817-87e7bad4-a608-48e1-be04-581c82db4f2a.png)
Next, to make sure you are on your computer and not a remote computer, type in cd ~, press enter, and then type in the given command ssh-keygen. Continue to press enter until you see the keys randomart image. This is where you have created your own ssh key. 

![Image](https://user-images.githubusercontent.com/114532765/195758972-d8f0e28c-2289-43c0-9e2c-886ee45a920b.png)
After, log onto the server using ssh. Include the command “ls” a space after you write your login username. Below is another example is using a command to directly run on the remote server.

![Image](https://user-images.githubusercontent.com/114532765/195759113-77a12030-b4c9-4cd7-b668-170d95ec2ec6.png)
