# generate ssh

```
ssh-keygen -t ed25519 -C "your_email@example.com"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
cat ~/.ssh/id_ed25519.pub
```

## Keyboard bluetooth

```
bluetoothctl
power on
agent KeyboardOnly
default-agent
pairable on
scan on

pair 01:02:03:04:05:06
trust 01:02:03:04:05:06
connect 01:02:03:04:05:06

quit
```
