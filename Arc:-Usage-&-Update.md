### Use Display Output

* You can use a connected Display to setup the Loader. Loader will be shown automatically.

### Use Webterminal

* You can use Webterminal: `http://IP:7681` to setup the Loader. Loader will be shown automatically.

### Use SSH

* You can use SSH: User: `root` Password: `arc` to setup the Loader. Loader can be launched with `arc.sh`.

### Reboot to Arc from DSM

* Reboot to Loader from DSM `loader-reboot.sh config` or `/usr/sbin/loader-reboot.sh config`.

### Arc Update

* Best option is to replace the Bootmedia with the new Arc Version
* Or you can select "Upgrade Loader" in Arc Update Section
* All Subversions have to be lower or equal to Arc Release. ( Arc 23.11.1 and Addons 23.10.28 -> working / Arc 23.11.1 and Addons 23.11.4 -> not working)
* Use restore Option only if you reinstall same version of Arc Loader

### DSM Update

* You can Update to every new Version of DSM until the Buildnumber will not change, without Loader Update.

Note: All build later than 23.10.1b will have livepatching - If a new DSM Version is found and your Loader doesn’t support this, the Loader will try to get latest source from Github. If there is no Update at this time, you only have to wait for the new files and boot again. 