## terminal-tricks

```
##### Automatic Web Server VPN Hackthebox:
ZSH -> printf "alias php-hackthebox=\"ip a | grep 'tun0' | grep 'inet' |sed 's/\/.*//' | sed -e 's/^.*t//' | xargs -I@ php -S @:8082\"" >> ~/.zshrc 
BASH -> printf "alias php-hackthebox=\"ip a | grep 'tun0' | grep 'inet' |sed 's/\/.*//' | sed -e 's/^.*t//' | xargs -I@ php -S @:8082\"" >> ~/.bashrc
```

```
##### Git show all logs:
git log | grep commit | awk '{print $2}' | xargs git show
```
