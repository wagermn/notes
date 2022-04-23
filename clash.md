# Install clash on Ubuntu

## download
Go to [release](https://github.com/Dreamacro/clash/releases) to download `clash-linux-amd64-vX.X.X.gz`.

## clash as a daemon [copy from here](https://github.com/Dreamacro/clash/wiki/clash-as-a-daemon)

Copy Clash binary to `/usr/local/bin` and configuration files to `/etc/clash`
```bash
sudo cp clash /usr/local/bin
sudo cp config.yaml /etc/clash/
sudo cp Country.mmdb /etc/clash/
```

Create the systemd configuration file at /etc/systemd/system/clash.service:
```bash
[Unit]
Description=Clash daemon, A rule-based proxy in Go.
After=network.target

[Service]
Type=simple
Restart=always
ExecStart=/usr/local/bin/clash -d /etc/clash

[Install]
WantedBy=multi-user.target
```

Launch clashd on system startup with:
```bash
sudo systemctl enable clash
```

Launch clashd immediately with:
```bash
sudo systemctl start clash
```
Check the health and logs of Clash with:
```bash
sudo systemctl status clash
sudo journalctl -xe
```
