# GateWay

## Gateway board

We gebruken voor de basis een Raspberry Pi 4 Compute module op een CM4-POE-UPS-BASE, dit bord heeft een ingebouwde UPS in de vorm van 3 18650 Li-ion batterijen. We verder het apparaat van stroom verzien middels POE 802.3af, ook is er ondersteuning voor RTC met een CR2032 batterij.

## BOM

- CM4-POE-UPS-BASE KIT (<https://www.waveshare.com/wiki/CM4-POE-UPS-BASE>)
- 3X 18650 batterij
- Raspberry PI Compute module 4 met 32GB MMC (CM4104032)
- Antennes voor LoRaWAN
- 2x Pigtail SMA-MHF voor LoRaWAN optimaal 8.5cm
- 1x Pigtail SMA-MHF, lengte nog te bepalen
- CR2032 batterij
- USB SDR + antenne
- IC880A LoRaWAN bord
- Adapter bord IC880A (zie onder)
- 12V Fan 4010 met PWM
- Metalen behuizing (zie onder))

### Adapter Board

- PCB design (<https://github.com/OpenIotNetwork/ic880a-adapter-raspberry>)
- 1 pc of 1x20 pinheader
- 1 pc of 2x20 pinheader
- 2 pcs of 1x3 pinheader

### Enclosure voorbeelden

| Hoogte     | Breedte    | Diepte     | Rating   | Prijs (excl.) | Link                                                                                                       |
| ---------- | ---------- | ---------- | -------- | ------------- | ---------------------------------------------------------------------------------------------------------- |
| 500 mm     | 400 mm     | 175 mm     | IP66     | 82,94 €       | [Farnell](https://be.farnell.com/hylec/deds0300/steel-door-enclosure-ip66-ik10/dp/3375484)                 |
| 400 mm     | 300 mm     | 150 mm     | IP65     | 63,16 €       | [Farnell](https://be.farnell.com/europa-components/stb403015/steel-enclosure-400x300x150mm/dp/3371506)     |
| 400 mm     | 400 mm     | 210 mm     | IP66     | 56,75 €       | [RS-Online](https://benl.rs-online.com/web/p/wall-boxes/7755325)                                           |
| 400 mm     | 400 mm     | 300 mm     | IP66     | 56,75 €       | [RS-Online](https://benl.rs-online.com/web/p/wall-boxes/1896590)                                           |
| **400 mm** | **300 mm** | **200 mm** | **IP66** | **83,47 €**   | [RS-Online](https://be.farnell.com/schneider-electric/nsys3d4320p/enclosure-ip66-400x300x200mm/dp/1853682) |

### Behuizing print adapter

WIP
