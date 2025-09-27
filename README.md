### To remove kaspersky in Linux

```
sudo apt remove kesl-gui kesl klnagent64 -y 
```

### To remove other application
```
sudo apt remove rhythmbox thunderbird
```

### To list top 10 large files

```
sudo find / -type f -exec du -h {} + 2>/dev/null | sort -hr | head -n 10
```

### KV process

#### Ctrl+Alt+T to terminal

```
sudo nano .bashrc
```

### Add anywhere in .bashrc, To exec kv, replace kv with appropriate name, open terminal and issue(exec) kv to open kv
```
kv() {
 sudo java -jar ~/Desktop/kv.jar
}
```
### java installtion

By default, Java 11 is not installed on Linux Mint 22.
To check the Mint version, run

```
cat /etc/os-release
```

If running java --version results in “command not found” or a similar error, Java is not installed.
To install Java 11 (OpenJDK) on Linux Mint 22, you can do:
```
sudo apt update; sudo apt install default-jre
```
After installing, verify with:
```
java --version
```
