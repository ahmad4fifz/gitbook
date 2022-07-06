# Failed to open "/etc/machine-id": No such file or directory

## Solution

Generate the new machine-id using the following command:

```
sudo systemd-machine-id-setup
```

or

```jsx
sudo dbus-uuidgen --ensure=/etc/machine-id. systemd-machine-id-setup
```

Check if `/etc/machine-id` exists and contain machine UUID.
