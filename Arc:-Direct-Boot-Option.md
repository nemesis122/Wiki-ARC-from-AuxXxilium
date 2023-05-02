Please set Arc - Advanced - Direct Boot - "true"

 - If you have problems to start the DSM
 - If your Hardware will not be found while boot to DSM
 - If you have other problems while booting (especially on HP Clients)

---

Make sure you have rebuilded the Loader after setting Direct Boot to true.

---

**The "Direct Boot" Mode is persistent with Arc Loader. There is a special way after install DSM and Update DSM.**

-> You have to boot once with "Boot DSM" instead of "Boot DSM directly". (If you don't do this, you will stuck in a loop with DSM install page).
-> After the Loader is rebooted, it will always load "Direct Boot" and don't need to reboot everytime like old integrations.