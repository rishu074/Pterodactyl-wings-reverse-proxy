<h3 align="center">Reverse Proxy of Pterodactyl Wings on Port 8080</h3>

<div align="center">

[![Status](https://img.shields.io/badge/status-active-success.svg)]()
[![GitHub Issues](https://img.shields.io/github/issues/kylelobo/The-Documentation-Compendium.svg)](https://github.com/kylelobo/The-Documentation-Compendium/issues)
[![GitHub Pull Requests](https://img.shields.io/github/issues-pr/kylelobo/The-Documentation-Compendium.svg)](https://github.com/kylelobo/The-Documentation-Compendium/pulls)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](/LICENSE)

</div>

---

<p align="center"> Reverse proxy of SFTP of pterodactyl Wings.
    <br> 
</p>

## 🏁 Installing

OPEN ``` nano /etc/nginx/nginx.conf```


AFTER
```

        include /etc/nginx/conf.d/*.conf;
        include /etc/nginx/sites-enabled/*;

}
```
PASTE 
```
stream {
        include /etc/nginx/sshProxy/*;
}
```

THEN
DO ```cd /etc/nginx && mkdir sshProxy && touch sftpProxy.conf```
