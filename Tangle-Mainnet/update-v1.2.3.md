

```
sudo systemctl stop tangle
wget -O tangle https://github.com/webb-tools/tangle/releases/download/v1.2.3/tangle-default-linux-amd64 && chmod +x tangle
sudo mv tangle /usr/bin/
tangle --version
```
```
systemctl daemon-reload
systemctl restart tangle && journalctl -u tangle -f -o cat
```
