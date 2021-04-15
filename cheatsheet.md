#### CSS

```css
/* Keyword values */
color: currentcolor;

/* <named-color> values */
color: red;
color: orange;
color: tan;
color: rebeccapurple;

/* <hex-color> values */
color: #090;
color: #009900;
color: #090a;
color: #009900aa;

/* <rgb()> values */
color: rgb(34, 12, 64, 0.6);
color: rgba(34, 12, 64, 0.6);
color: rgb(34 12 64 / 0.6);
color: rgba(34 12 64 / 0.3);
color: rgb(34.0 12 64 / 60%);
color: rgba(34.6 12 64 / 30%);

/* <hsl()> values */
color: hsl(30, 100%, 50%, 0.6);
color: hsla(30, 100%, 50%, 0.6);
color: hsl(30 100% 50% / 0.6);
color: hsla(30 100% 50% / 0.6);
color: hsl(30.0 100% 50% / 60%);
color: hsla(30.2 100% 50% / 60%);

/* Global values */
color: inherit;
color: initial;
color: unset;

```
#### HTML

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>My test page</title>
  </head>
  <body>
    <p>This is my page</p>
  </body>
</html>
```



# CSS

### Example 0

```css
.class {
  display: inline-flex !important;
  list-style: none;
  padding: 0;
  position: relative;
  right: 0;
  text-align: right;
  top: 0;
  color: SandyBrown;
  z-index: 99999999;
}
```

### Example 1
```css
body {
  font-family: Arial;
  color: magenta;
}
```

### Example 2
```css
color: white;
text-decoration: underline;
background-color: blue;
position: relative;
```


### Example 3
```css
/*
 Shared styles
*/

footer p {
	font: 100% Rockwell, Arvo, serif;
}
```

# HTML

### Exmaple 0

```html
<div>text</div>
```

### Example 1
```html
<!-- comment -->
<ul>
  <li>item</li>
  <li>item</li>
  <li>item</li>
</ul>
```

### Example 2
```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>My test page</title>
  </head>
  <body>
    <p class="c">This is my page</p>
  </body>
</html>
```



# Bash

```bash
ls -al
ls -alh
git commit -m "Initial Commit"
npm install -g kmdr

# Program grep

grep -RI "ERROR" .
grep -i "info" .

# Program rm 

rm --recursive --force
rm -f -r /
rm -rf node_modules/

# Program tar

tar -xvzf file.tgz -C directory/
tar -x -v -z -f file.tgz
tar --extract --verbose --gzip --file file.tgz

# Program git

git commit --all --message "Message"
git commit -am "Message"
git reset --hard
git clone git@github.com:facebook/react.git
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

# Program echo
echo 		 hello
echo "			hello"

# Iptables
iptables -t nat -A Clash -d 192.168.0.0/16 -j RETURN

# Rsync

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

```bash
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

history | awk '{print $2}' | sort | uniq -c | sort -nr | head -5
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

```sh
# With declare
export PATH=$PATH:/another/path
```

## Subshell

```sh
(ls && rm)
```
# Cool websites

- https://tldr.sh - A very popular cheatsheets repos
- https://cheat.sh/curl, https://cheat.sh/ssh, etc
- https://git-scm.com/book/en/v2/Getting-Started-Installing-Git - Installation Instructions for git
- https://docs.docker.com/install/linux/docker-ce/ubuntu/ - Good examples of package maners and docker commands
- https://devhints.io/ - More Cheatsheets
