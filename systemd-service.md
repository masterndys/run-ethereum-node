📄 docs/systemd-service.md

md
Copy
Edit
# Run Geth as Systemd Service

```ini
[Unit]
Description=Ethereum Node
After=network.target

[Service]
ExecStart=/usr/bin/geth --http
Restart=always

[Install]
WantedBy=default.target
