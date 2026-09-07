## Hi, I'm David

I build Home Assistant integrations for hardware that shipped without one —
devices that work perfectly well, but that the manufacturer only ever exposed
through a phone app.

The pattern is always the same. Something on your wall speaks a private protocol
to a vendor cloud, and nobody wrote down what it says. So you capture the
traffic, work out what the bytes mean, and hand the result back to Home
Assistant as ordinary entities.

**Everything here is free, MIT-licensed, and runs entirely on your own network.**
No accounts, no vendor cloud, nothing leaving the house.

### 2.4 GHz — Bluetooth Low Energy

- **[daikin_madoka](https://github.com/dasimon135/daikin_madoka)** — Daikin BRC1H
  "Madoka" wall thermostats. Temperature, mode, fan speed and filter alerts, with
  no Daikin account and no phone app. Originally
  [mduran80's work](https://github.com/mduran80/daikin_madoka); this fork has
  carried it since.
- **[ha-bluetooth-mesh](https://github.com/dasimon135/ha-bluetooth-mesh)** —
  Bluetooth SIG Mesh lighting (Häfele Connect Mesh, ThingOS) through the ESPHome
  proxies you already have. A pure-Python mesh stack, provisioning included, so
  the discontinued vendor gateway isn't needed.
- **[ha-bluesight](https://github.com/dasimon135/ha-bluesight)** — Read-only.
  Shows which Bluetooth proxy holds which connection slot, and names the
  deadlocks, ghost slots and pairing storms when they happen.

### 433.92 MHz — ISM band

- **[ha-rf-fan](https://github.com/dasimon135/ha-rf-fan)** — Ceiling fans that
  only ever came with a handset. It never decodes the protocol: it captures what
  your remote sends and sends it back, which is why it works with fans I have
  never seen.
- **[ha-dooya](https://github.com/dasimon135/ha-dooya)** — Dooya roller blinds
  and shutters, with position. The motor reports nothing back, so it is timed
  from travel and recalibrated at the end stops.

### Where things happen

Support lives in each repository's issues — an issue stays readable, searchable
and linkable long after the conversation ends, which a forum thread does not.
Say what hardware you have and bring the logs.

Bug reports from people with hardware I don't own are worth more than they look.
Several of these projects support devices I have never touched, because someone
was patient enough to run a test build and say what happened.

**[dasimon135.github.io](https://dasimon135.github.io)** ·
[buy me a coffee](https://buymeacoffee.com/dasimon135)
