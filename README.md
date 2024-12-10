**Dreambox Two Softcam Repository Install**

```
curl -L -o /tmp/gp4-cam-feed-configs.deb https://github.com/mutebessim/dreambox-two/raw/refs/heads/main/debs/gp4-cam-feed-configs_2.0-r4_all.deb && dpkg -i /tmp/gp4-cam-feed-configs.deb
```

**Dreambox Two Oscam Emu Install**

First run the above command
```
apt-get update && apt-get upgrade && apt-get install gp4-cam-oscam-2-emu
```
