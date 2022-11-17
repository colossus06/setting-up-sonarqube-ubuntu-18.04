# setting-up-sonarqube-ubuntu-18.04

### Conf. the prerequisites

![image](https://user-images.githubusercontent.com/96833570/202447891-32cab4c2-c224-4d6d-9777-772c9d69e826.png)

![image](https://user-images.githubusercontent.com/96833570/202447802-c6ebde63-1265-4564-8679-3290f8521566.png)


`sudo nano /etc/sysctl.conf`

```
vm.max_map_count=524288
fs.file-max=131072
```

`sudo sysctl -p`

```
sudo apt update
sudo apt install docker -y
sudo apt install docker-compose -y
sudo usermod -aG docker $USER
```


### docker compose file

### References

[](https://docs.sonarqube.org/latest/requirements/requirements/)

[](https://unix.stackexchange.com/questions/621023/how-to-display-current-vm-map-max-map-count-value)
