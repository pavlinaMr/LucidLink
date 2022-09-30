# /etc/systemd/system/lucid.service
[Unit]
Description=Start Daemon Service
After=network.target

[Service]
Type=simple
ExecStart=lucid daemon --fs test1.lucid --user testuser --password "DnN795#W8%33"
Restart=always
RestartSec=1
User=testuser

[Install]
WantedBy=multi-user.target
