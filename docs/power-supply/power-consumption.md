# Theoretical power consumption per component
*Onderstaande data is afkomstig uit de datasheets van de betreffende componenten*

# ATSAMD21 microcontroller
**standby:**

TYP: 4,06µA-55,2µA (3,3V)
MAX: 100µA

**idle:**

1,07mA-2,33mA (3,3V)

**regular:**

6,5mA-7mA (3,3V)

*Dit is het hoogst vermelde stroomverbruik in ACTIVE status, tijdens een CoreMark algoritme bij 85°C. vermeld in datasheet table 36-8, pg 942.*

**verloop meting:**

De microcontroller komt uit slaapmodus om metingen uit te voeren en vervolgens data via LoRa uit te wisselen. Hoe lang de microcontroller uit slaapmodus is, is afhankelijk van de tijdsduur van de metingen en van de LoRa communicatie.

Hiernaast is het tijdsinterval tussen wake-ups instelbaar via LoRa. Dit kan worden aangepast in correspondentie met de effectieve energieconsumptie tijdens het gebruik.

# RN2483 Lora module
**sleep modus:** 

1,6µA-2,6µA (3,3V-3,6V)

**idle/standby:**

2,8mA-3,1mA (3,3V-3,6V)

**regular:**

868MHz: *hoogste stand*: 38,9mA (3,3V)
433MHz: *hoogste stand* 32.9mA (3,3V)

**receive:**

14,22mA-14,69mA (3,3-3,6V)

**verloop meting:**

*Zie werking LoRa*
(Dit is nog niet uitgewerkt)

# SCD41 CO2 sensor

**sleep modus:** 



**idle/standby:**

*Hiervoor is geen data in de datasheet aanwezig, maar volgens een artikel op eMariete:*
*(https://emariete.com/en/sensor-co2-sensirion-scd40-scd41-2/#:~:text=According%20to%20my%20own%20measurements,period%20has%20been%201.20mA.)*

171µA tijdens idle bij 1 single shot per minuut

**regular:**

15mA-18mA (3,3V)
11mA-13mA (5V)

**low power periodic:**

3,2mA-3,5mA (3,3V)
2,8mA-3mA (5V)

**periodic single shot:**

0,45mA-0,5mA (3,3V)
0,36mA-0,4mA (5V)

**verloop meting:**

Bij opstarten: vanaf 2,25V start de component op. Na 1000ms staat de component in idle mode. Vanuit idle mode kunnen er metingen worden uitgevoerd. Bij periodic single shot duurt het 5 seconden om de gemeten data terug te krijgen.

# SGP41 VOC&NOx sensor
**idle/standby:**

34µA-105µA (3,3V)

**conditioning mode:**

4,2mA-4,6mA (3,3V)

**regular:**

3,0mA-3,4mA (3,3V)

**verloop meting:**

Power-up time van 0,6ms, waarna de component in idle mode komt. Vanuit idle mode kan de component in conditioning mode geplaatst worden. Hier wordt 10 seconden als standaard en als maximum gebruikt. Daarna kan het commando gegeven worden om de ruwe data op te meten, wat 1s duurt. Hierna kan het commando worden gegeven om terug naar idle mode te gaan.

# SPS30 particulate matter sensor
**sleep modus:** 

38µA-50µA (5V)

**idle/standby:**

330µA-360µA (5V)

**regular:**

55-65mA (5V)

**startup-measurement**

80mA (5V)

**verloop meting:**

Bij opstarten gaat de sensor in idle mode. Wanneer een measurement commando wordt gegeven, duurt het 20ms om het commando door te geven. Daarna duurt het 200ms om de meting op te starten en 1s om een meting uit te voeren. Vervolgens kan een stop measurement commando gegeven worden, wat 20ms duurt en ten slotte een sleep commando wat 5ms duurt.

Hiernaast is er een standaard routine die 1x per week (elke 604800s) de ventilator in het component laat draaien om het stof uit de component te blazen. Dit duurt 10s. Het tijdsinterval in seconden is aan te passen om het interval te vergroten.

# BME280 humidity & pressure sensor
**sleep modus:** 



**idle/standby:**



**regular:**



**receive:**



**verloop meting:**



# GY-NEO6M GPS module
**sleep modus:** 



**idle/standby:**



**regular:**



**receive:**



**verloop meting:**

