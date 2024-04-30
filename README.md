# rae-test

Instructions to test 

1. Create a fork of this project
2. All commits that is completed needs to be called "<lasstname>-rtest> in your repo

3. setup ssh keys to server 192.168.1.99. User= rtest , password= test123
4. setup ssh keys to your local server and user 

5. Set up an inventory file with two group. One called localhosts and the other should be called rae
6. The IP in your local hosts group should be 127.0.0.1. The IP in your rae group should be 192.168.1.99


Write the following playbook. 

1. Do a ping on these servers and save the results in ping-output.txt
2. Copy the httpd.conf file to /tmp/<lastname><firstname>/ , and tag this task called push 
3. Set a variable for the .99 server and call it stype=jump
4. Set a variable for the 127.0.0.1 server and call it stype=local
5. Add a task to print out the values of the stype value for each node
6. Create a task to tar the /tmp/<lastname> directory only when the variable stype=service 



Push all changes up to the repo 
