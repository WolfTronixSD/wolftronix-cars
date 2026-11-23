# WolfTronix Cars

The phone website for the WolfTronix garage alarm: shows the cars (home / away, batteries, alarms, trips with
the route on a map, event log) and the garage doors, from anywhere.

Live at **https://wolftronixsd.github.io/wolftronix-cars/** (GitHub Pages from `main`).

This page holds no data and no secrets. The garage CYD pushes its data encrypted (AES-256 + HMAC-SHA256)
to a public MQTT broker; the page decrypts it in the browser with the key from your private link
(after the `#`, which browsers never send to any server). Get your link on the CYD at `http://cyd.local/cloud`.

Source and details: `car_site/` in the 2CarGarageAlarm repo. Copy `car_site/index.html` here after changing it.
