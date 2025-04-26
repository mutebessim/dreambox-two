**Dreambox Two Softcam Repository Install**

```
curl -L -o /tmp/gp4-cam-feed-configs.deb https://github.com/mutebessim/dreambox-two/raw/refs/heads/main/debs/gp4-cam-feed-configs_2.0-r4_all.deb && dpkg -i /tmp/gp4-cam-feed-configs.deb
```

**Dreambox Two Oscam Emu Install**

First run the above command
```
apt-get update && apt-get upgrade && apt-get install gp4-cam-oscam-2-emu
```

**Example for LCD**
```
    <screen id="100" name="InfoBarSummary" position="0,0" size="240,80">
		<ePixmap pixmap="Zombi-Shadow-FHD/skin_default/back_DE.png" position="0,0" scale="fill" size="240,80" zPosition="-1" />
        <widget blend="on" position="1,0" render="Picon" scale="stretch" size="150,50" source="session.CurrentService" zPosition="1">
            <convert type="ServiceName">Reference</convert>
        </widget>
		<!-- foregroundColor="ltbluette2" -->
		<widget font="Display;38" foregroundColor="ltbluette2" halign="center" position="136,-3" render="Label" size="120,33" source="global.CurrentTime" transparent="1" valign="center">
            <convert type="ClockToText">Format:%H:%M</convert>
        </widget>
		<widget borderWidth="1" pixmap="Zombi-Shadow-FHD/skin_default/progressAB.png" position="161,35" render="Progress" size="70,12" source="session.Event_Now" transparent="1">
            <convert type="EventTime">Progress</convert>
        </widget>
		<!-- EliteRunningText -->
		<widget font="Display;35" halign="left" position="0,40" options="movetype=running,direction=left,startpoint=0,repeat=2,steptime=5,startdelay=2000,noWrap" render="ExtRunningText" size="240,40" source="session.Event_Now" transparent="1" valign="center" zPosition="10">
            <convert type="EventName">Name</convert>
        </widget>
    </screen>
```
