apt-get install tinyproxy
nano /etc/tinyproxy/tinyproxy.conf
scroll to the bottom and find the "Allow 10.0.0.0/8" line and uncomment it.
Run service tinyproxy start
Within Burp, go to User options → connections
Add the upstream proxy of the host:port where tinyproxy is set up, use * for destination host

![image](https://user-images.githubusercontent.com/66387143/145064589-29063dd0-1a9c-48dc-b7fb-073ac6c5eac6.png)
