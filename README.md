## Hi, I'm David

You bought a thermostat, some blinds, a ceiling fan. They work fine. The only
thing standing between you and controlling them properly is the manufacturer's
app.

I write the Home Assistant integrations that give those devices back to you.
Once one is installed, the device appears in Home Assistant like any other: you
can put it on a dashboard, automate it, or ask your voice assistant for it.

**All of it is free, and all of it runs on your own network.** There is no
account to create and no cloud to depend on — nothing about your home leaves
your home.

### Bluetooth — 2.4 GHz

**[daikin_madoka](https://github.com/dasimon135/daikin_madoka)** — Control your
Daikin heating and cooling from Home Assistant: set the temperature, change the
mode, adjust the fan, see when the filter needs cleaning. It reaches the BRC1H
"Madoka" panel on your wall over Bluetooth, with no Daikin account and no phone
app. Originally [mduran80's work](https://github.com/mduran80/daikin_madoka);
this fork has carried it since.

**[ha-bluetooth-mesh](https://github.com/dasimon135/ha-bluetooth-mesh)** —
Switch and dim your Häfele Connect Mesh lights from Home Assistant, using the
ESPHome Bluetooth proxies already scattered around your house. Häfele
discontinued the gateway these lights needed; this replaces it, so there is no
extra box to buy.

**[ha-bluesight](https://github.com/dasimon135/ha-bluesight)** — When your
Bluetooth devices keep going unavailable, this tells you why. It shows which
proxy is holding which connection and names the fault when it finds one. It only
ever watches — it changes nothing.

### Radio — 433.92 MHz

**[ha-rf-fan](https://github.com/dasimon135/ha-rf-fan)** — Put a ceiling fan
that only came with a remote into Home Assistant. You press each button once
while it listens, and you get back the speeds, the light, the timer and the
direction. It never tries to understand the signal, which is why it works with
fans I have never seen.

**[ha-dooya](https://github.com/dasimon135/ha-dooya)** — Open and close your
Dooya blinds and shutters, and stop them halfway with a slider. The motor never
says where it is, so the position is timed from how long the blind travels and
corrected at each end stop.

### Something not working?

Open an issue in the repository it belongs to. Tell me what hardware you have
and attach the logs — with those two things I can usually answer within the
week.

If you have a device I don't own, your bug report is worth more than you would
think. Several of these projects support hardware I have never touched, because
someone was patient enough to run a test build and tell me what happened.

**[dasimon135.github.io](https://dasimon135.github.io)** ·
[buy me a coffee](https://buymeacoffee.com/dasimon135)
