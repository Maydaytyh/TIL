需要现在本地生成公钥和密钥，使用`ssh-keygen -t rsa`来生成

随后使用`ssh-copy-id -i /root/.ssh/id_rsa.pub remote`，即可实现免密登录