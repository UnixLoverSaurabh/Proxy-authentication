In Ubuntu 14.04 or later, in order to use some commands in terminal (like apt-get) trough the college proxy, We need to do the following changes, beyond System Settings > Network > Network proxy > "Apply system wide" 

Copy the four lines in apt.conf file

`$ vi /etc/apt/apt.conf`

Acquire::http::proxy "http://[username]:[password]@[webproxy]:[port]/";
Acquire::https::proxy "https://[username]:[password]@[webproxy]:[port]/";
Acquire::ftp::proxy "ftp://[username]:[password]@[webproxy]:[port]/";
Acquire::socks::proxy "socks://[username]:[password]@[webproxy]:[port]/";



or the same changes in (optional)
`$ vi /etc/apt/apt.conf.d/proxy.conf`


Set up proxy in terminal
Enter the following commands or append these two lines in .bashrc file in home directory:

`$ export http_proxy='http://[username]:[password]@[webproxy]:[port]/'`
`$ export https_proxy='http://[username]:[password]@[webproxy]:[port]/'`

You can check the proxy set by
`$ echo $HTTPS_PROXY`



I think that at least the following command (from here)

`$ sudo http_proxy='http://[username]:[password]@[webproxy]:[port]' apt-get update`

should work, right?

