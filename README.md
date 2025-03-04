# Host-Ticketing-system
Self Host a Ticketing Software easily utilizing the cloud and docker.

### Steps

First, go to https://www.linode.com and create an account. You can use any Cloud platform, we will use Linode for this.
Once the account is set up, you should be on the main screen.
Click on create on the top right and click on linode.

![image](https://github.com/user-attachments/assets/c87508c1-cc10-40ce-85c6-857739141009)

Once the oage loads up, we will  click on Marketplace and search for "Peppermint"
Then we will scroll down and setup where you are and your linode plan, I picked the cheapest option.
![image](https://github.com/user-attachments/assets/b2bf24c1-701d-4684-83a3-080cb6ada2ba)

![image](https://github.com/user-attachments/assets/4c05af75-334d-49dd-947d-588c6fec69a0)

Put in label and use a STRONG password.
![image](https://github.com/user-attachments/assets/2fa3b04f-8608-4637-b3f2-600abe108ec1)

click create

![image](https://github.com/user-attachments/assets/52b26e83-b3aa-4d95-9c27-841b9fa0330d)

let it provision for us. Once it is running, we will hit "launch LISH Console" if its not done configuring then wait.

![image](https://github.com/user-attachments/assets/c47ea3f6-c32e-4b45-9fba-a1c6f8fe1415)

It should look like this.

![image](https://github.com/user-attachments/assets/d61865f7-e638-4acd-bc14-dc1dce5d1c8d)

lets make sure we are running a docker container by entering in the login "root" and whatver password you used.
should look like this. 
![image](https://github.com/user-attachments/assets/9905bfcd-a92f-4e26-af6d-686a665faa87)

Type "Docker ps" and pay attention to your Port number that the Software website will be on.
![image](https://github.com/user-attachments/assets/63378132-6109-4dac-ada5-31e6b84fc67d)
 next we will need our Reverse DNS. Go to the menu and click on "Network" then scroll down and look on the far right side of the webpage.

![image](https://github.com/user-attachments/assets/d1924819-f559-438b-ad05-1f64b1d4ad1a)
![image](https://github.com/user-attachments/assets/cba90d9a-1f24-48d2-8128-3cb79bb25556)

next, using the "reverse DNS" and port number we can get access to our ticketing system.

![image](https://github.com/user-attachments/assets/190a7fb6-282e-4bc4-9089-753374fd405b)

The page should then popup.
![image](https://github.com/user-attachments/assets/f60a08a3-fbd1-48e9-b124-ab0e30f76afd)

Email - admin@admin.com
password - 1234

![image](https://github.com/user-attachments/assets/c39f2b67-0fd5-4d60-b061-f866d9a7acd6)

just like that you have an easy to understand Ticketing software you can host. 

![image](https://github.com/user-attachments/assets/ec765a15-e6b3-431e-a520-353ab99ab457)

Now lets add a new user since we have a broken printer we need fixing.
Since we are an admin we can add new users. Click on "admin" on the left then "Users" and add a new user.
fill in credentials for this User.
![image](https://github.com/user-attachments/assets/4c67f024-c8ea-48b6-9d9b-383a22c57c6a)

![image](https://github.com/user-attachments/assets/7cff922c-a8de-4939-9263-85789f92b2de)
we now have another user "Ana"
![image](https://github.com/user-attachments/assets/43ece63a-6b19-4ad0-9054-439a50f0d2b1)

Now lets create a ticket so Ana can fix or printer.
go back to the main menu and click on "new issue"
![image](https://github.com/user-attachments/assets/5b44104c-d951-42c8-9426-75f69ff4c002)

Enter what needs to be fixed with any necessary details and create ticket.
![image](https://github.com/user-attachments/assets/590a5c67-2ac3-4e15-96f7-16f70865cbc7)

Now log in as Ana.
Our ticket we just created will show up on her dashboard.

![image](https://github.com/user-attachments/assets/3124a7d1-3bda-4bc1-b204-394dc13e8676)
click on the ticket and we can transfer the ticket, set the priority, write comments, and close them when we are done with any issues we have in these tickets.

![image](https://github.com/user-attachments/assets/84d2e631-1305-4c1f-a180-9ae04e26bc54)

This is a simple, easy to host and use Ticketing system. 
You can use this process to download many other more sophisticated Ticketing softwares that have a knowledge base and more features that any enterprise might need. 

If you would like to install this on a Linux Host you would need to Install Docker and use a docker compose file.
first Install Docker, Make a new directory and name it whatever ticketing software you will use (we will use peppermint again), Inside the new directory make a new file.

![image](https://github.com/user-attachments/assets/abcfbd3a-ef38-4e48-ad0e-170964640e9d)

paste docker configuration from https://github.com/Peppermint-Lab/peppermint.

![image](https://github.com/user-attachments/assets/3e0206aa-8936-43b7-b7e9-dac8e5069701)

use this Command to bring it up.

![image](https://github.com/user-attachments/assets/d7bf45ea-1272-450d-80f3-9c3b87b0a194)

when done, docker should be installed and ready to use for whatever ticketing system you picked. (each ticketing system has their own Docker compose file they are all not the same)
like before type in the command prompt "docker ps" get the port number and the local machine IP address you are using and it will take you to the log in screen once again but using your local machine instead of the cloud.

![image](https://github.com/user-attachments/assets/1ad98de5-13dd-44f8-b891-0050d418bd9c)

search bar on the internet type you IP and port number "X.X.X.X.5000" and BOOM

![image](https://github.com/user-attachments/assets/34e6343e-df91-42f5-a487-9fcdab0337ec)
