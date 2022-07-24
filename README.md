# NodeJS-MongoDB

Commands:

Install Node:
nvm install node

Create redirect from port 80 to 8000:
sudo iptables -t nat -A PREROUTING -p tcp --dport 80 -j REDIRECT --to-ports 8000

cd /etc/yum.repos.d sudo touch mongo-org-5.0.repo

[mongodb-org-5.0]
name=MongoDB Repository
baseurl=https://repo.mongodb.org/yum/amazon/2/mongodb-org/5.0/x86_64/
gpgcheck=1
enabled=1
gpgkey=https://www.mongodb.org/static/pgp/server-5.0.asc
Install MongoDB:
sudo yum install -y mongodb-org

directories:
cd /  
sudo mkdir data 
sudo mkdir db  
Navigate back to the home directory:
cd /home/ec2-user

Mongo Service:
sudo service mongod start

MongoDB:
mongo
use mern

Created database owner:
db.createUser({ user: "my_user", pwd: "my_pwd", roles: ["dbOwner"] })

Create database documents:

db.members.insert({ firstName: "Amazon", lastName: "Linux" })
db.members.insert({ firstName: "Amazon", lastName: "Linux" })
Install mongoose and express
npm install mongoose express

Install PM globally:
npm install pm2 -g

Run the app:
pm2 start server.js
