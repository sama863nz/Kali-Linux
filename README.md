# Kali-Linux setup pre-requisites

# Spin a EC2 instance using AMI Catalog and ssh into it by:
ssh -i "kali-key-pair.pem" root@ec2-18-234-111-238.compute-1.amazonaws.com

# Change root to kali in the above command
ssh -i "kali-key-pair.pem" kali@ec2-18-234-111-238.compute-1.amazonaws.com


sudo apt update    

sudo apt install xfce4 xfce4-goodies tightvncserver

sudo apt-get install gnome-core kali-defaults kali-root-login desktop-base

tightvncserver -geometry 1024x768

# to give all the internet connections and local addresses. Two among them are 6001 and 5901
Netstat -tulpn 


# For every new connection:
# Open a new cmd 
# Cd to the location of .pem file
cd "C:\Users\sama8\OneDrive\AWS KEY PAIR openSSH"
ssh -L 5901:localhost:5901 -N -f kali@34.229.204.253  -i  kali-key-pair.pem  

# command to setup VNC in kali linux server
tightvncserver -geometry 1024x768  
ssh -L 5901:localhost:5901 -N -f kali@54.221.54.137  -i  kali-key-pair.pem  


