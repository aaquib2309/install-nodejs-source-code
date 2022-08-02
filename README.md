# install-nodejs-source-code

yum update -y
yum install wget -y
yum install gcc-c++ python39 -y
wget https://nodejs.org/dist/v18.7.0/node-v18.7.0.tar.gz
tar -xvzf node-v18.7.0.tar.gz
rm node-v18.7.0.tar.gz
cd node-v18.7.0/
./configure --prefix=/usr/local/
make
make install
node --version
