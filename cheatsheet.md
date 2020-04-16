# Get command explanations from kmdr.sh

## Simple commands

```bash
# Program ls
ls -l
ls -al
ls -ltr

# Program grep

grep -RI "ERROR" .
grep -i "info" .

# Program rm 

rm --recursive --force
rm -f -r /
rm -rf /
rm -recursive -force # error due to single `-`

# Program tar

tar -xvzf file.tgz -C directory/
tar -x -v -z -f file.tgz
tar --extract --verbose --gzip --file file.tgz

# Program npm

npm list
npm uninstall

# Program git

git commit --all --message "Message"
git commit -am "Message"
git reset --hard
git clone git@github.com:facebook/react.git
git clone -b next https://github.com/ediardo/kmdr-ast
git clone -q https://opendev.org/openstack/devstack

# Program aws

aws ec2 describe-instances
aws configure --profile project1

# Program brew

brew install 

# Program Docker

docker ps -a
docker pull image
docker run -it --rm  kmdr-cli
 
# Program du

du -sh dir/
du -ah dir/

# Program mysql

mysql --user=root --password=root

# Program find

find . -name asdf
find . -P -L -H

# Program ps
ps -ef

# Program minikube
minikube start --vm-driver=none --image-mirror-country='cn'

# echo
echo 		 hello
echo "			hello"

# Iptables
iptables -t nat -A Clash -d 192.168.0.0/16 -j RETURN

# Rsync

rsync --stats -PSvahHAXx --log-file=$LOG --exclude-from=$EXCLUDE --link-dest=$DEST_ORIG $SOURCE $DEST_NEXT
rsync -avzh /source/path /destination/path/

# npm
/Users/ediardo/.nvm/versions/node/v12.16.1/bin/npm install --global kmdr
npm install typescript
npm i -g npm
npm install --save lodash
npm install chalk yargs inquirer
npm install ansi-regex
```

## Commands that take other commands

```
# Program sudo

sudo rm -rf
sudo apt install
sudo apt help
sudo -u admin /usr/bin/vim  /etc/config

# Program watch
watch date
watch -n 5 df -h
```

## List of commands

```bash
ls && rm

rm || ls || tar && cat

cat file.tx | grep "error"

cd dir/ ; ls -l ; rm file.txt
```

## Conditional Statements

```bash
if [ $1 -gt 100 ]
then
    echo Hey that\'s a large number.
    pwd
fi

[ -f /etc/resolv.conf ] && echo "$FILE exist" || echo "$FILE does not exist"

```

## Loop structures

```bash
for i in 1 2 3 4 5
do
   echo "Welcome $i times"
done
```

## Functions


```bash
test() {
  ls # show files
  rm -rf . # delete all files and directories
}

function anotherTest {
  ls # show files
  rm -rf . # delete all files and directories
}
```

## Command Substitution

```bash
$(ls)
$($($(ls))) 
```

## Redirection

```bash
# Redirect stdout to file 
ls -alh > allfiles.txt
   
# Redirect and append stdout to file "filename."
ls 1>> filename

# Redirect stderr to file "filename."
rm dir/ 2> filename

# Redirect and append stderr to file "filename."
rm dir/ 2>>filename

# Redirect both stdout and stderr to file "filename."      
who &> filename

# Redirects stderr to stdout.
# Error messages get sent to same place as standard output.
rm dir/ 2>&1
```

## Variable Assignment

```bash
NODE_ENV=production npm install
FILES=$(ls)
CURRENT_DATE=`date`
```

## With dollar sign (execute as normal user)

Some technical documentation use the dollar sign to indicate that the command should be executed as a non-root user

```bash
$ ls
$ rm
$ tar
$ git
```

## Declaration commands

```
# With declare
export PATH=$PATH:/another/path
```

## Subshell

```
(ls && rm)
```
# Cool websites

- https://tldr.sh - A very popular cheatsheets repos
- https://cheat.sh/curl, https://cheat.sh/ssh, etc
- https://git-scm.com/book/en/v2/Getting-Started-Installing-Git - Installation Instructions for git
- https://docs.docker.com/install/linux/docker-ce/ubuntu/ - Good examples of package maners and docker commands
- https://devhints.io/ - More Cheatsheets
