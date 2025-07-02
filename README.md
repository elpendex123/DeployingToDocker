1. Create a repository using github
2. For other users to be able to access this github , owner must add them as collaborators through github
3. Setting up SSH:
   a.) Run this command and it will create a .ssh directory and create Public and Private keys : ssh-keygen -t rsa -b 4096 -C "prithviatani@gmail.com"
   b.) cat id_rsa (Private Key)
   c.) cat id_rsa.pub (Public Key)
   d.) Copy the cat id_rsa.pub (Public Key) into your github under settings ssh key and new ssh key
   ![image](https://github.com/user-attachments/assets/0e53a08a-ab1e-4a3b-9d65-b544822d5291)
   e.) Optionally save SSH key in your local directory where you like - touch sshkey.txt

5. Configuring SSH
   a.) git config --global user.name "PrithviA"
   b.) git config --global user.email "prithviatani@gmail.com"
   c.) Test Connection to Github: ssh -T git@github.com
   d.) Shows if repository is setup to use ssh or http : git remote -v
   e.) Setting it from http to ssh : git remote set-url origin git@github.com:elpendex123/DeployingToDocker.git
   d.) Test is ssh is running on a pid: eval "$(ssh-agent -s)" 
