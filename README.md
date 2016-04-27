# Blog
Powered by [Ghost](http://ghost.org) and [Buster](https://github.com/axitkhurana/buster/).
# How to use
* Install Node.js 4.2
```shell
wget https://nodejs.org/dist/v4.2.2/node-v4.2.2-linux-x64.tar.gz
tar -xzvf node-v4.2.2-linux-x64.tar.gz && cd node-v4.2.2-linux-x64
cp ./bin/node /usr/local/bin/node
cp -r ./lib/node_modules /usr/local/lib/node_modules
ln -s /usr/local/lib/node_modules/npm/bin/npm-cli.js /usr/local/bin/npm
cp -r ./include/node /usr/local/include
mkdir -p /usr/local/man/man1 && cp ./share/man/man1/node.1
/usr/local/man/man1/node.1
```
* Install/Update npm
```shell
\curl -sSL https://npmjs.org/install.sh | bash
```
* Clone this repository
```shell
mkdir static
cd static
git clone https://github.com/acjohnson/acjohnson.github.io.git
```
* Start Ghost
```
cd acjohnson.github.io/ghost
npm install
npm start
```
* Browse to Ghost site:
http://<hostname>:2368
* Login to Ghost admin:
http://<hostname>:2368/ghost
* Install buster
```shell
pip install buster
```
* Create new static content with Buster
Note: Ensure ghost is running on port 2368
```shell
cd static
buster generate
```
* Preview the static content
```shell
buster preview
```
