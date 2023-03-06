# Theoretical power consumption per component
*Onderstaande data is afkomstig uit de datasheets van de betreffende componenten*

# ATSAMD21 microcontroller
**sleep modus:**

**regular:**

**verloop meting:**
De microcontroller komt uit slaapmodus om metingen uit te voeren en vervolgens data via LoRa uit te wisselen. Hoe lang de microcontroller uit standby is, is afhankelijk van de tijdsduur van de metingen en van de LoRa communicatie.

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
34µA-105µA (3,3V-3,6V)

**conditioning mode:**
4,2mA-4,6mA (3,3V)

**regular:**
3,0mA-3,4mA (3,3V)

**verloop meting:**
Power-up time van 0,6ms, waarna de component in idle mode komt. Vanuit idle mode kan de component in conditioning mode geplaatst worden. Hier wordt aangeraden 10 seconden 

# SPS30 particulate matter sensor
**sleep modus:** 


**idle/standby:**


**regular:**

**verloop meting:**


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
