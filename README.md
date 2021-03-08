# linux-dframe

A simple linux digital picture frame

## Installation

Create a `.env` file with this content:
```
DFRAME_FOLDER="/path/to/folder"
```

Enable the sytemd service to run the script at boot:
```
cp dframe.service ~/.config/systemd/user/
systemctl --user daemon-reload
systemctl --user enable --now dframe.service
systemctl --user status dframe
```
