# Laden van een LiPo batterij
Lithium-gebaseerde batterijen zijn zeer veelzijdig, door hun hoge snelheid en vermogen. 

Hierbij komt wel kijken dat deze batterijen op een juiste manier worden behandeld, aangezien het mishandelen van een LiPo-batterij kan leiden tot smelten of zelfs ontvlammen of ontploffen van de batterij.

Een gewoonlijke laadcyclus van een LiPo batterij is onderverdeeld in 3 laadfasen, gescheiden volgens batterijspanning.

1. Trickle
2. Constant Current
3. Constant Voltage

![power-supply](LiPo-battery/optimalLiPoCharging.png 'Figuur 1: Realistisch laadverloop 3.7V Li-Po batterij')

# Trickle charge
Bij een lage batterijspanning, wordt de interne weerstand zeer hoog. Om schade aan de batterij te vermijden, moet de stroomsterkte tijdens het opladen bij lage batterijspanningen dus ook laag blijven. 

# Constant Current charge
Vanaf de batterijspanning hoog genoeg is, dan kan de batterij opgeladen worden aan een constante stroomsterkte. Doorgaans wordt aangeraden om de batterij op te laden aan maximaal 1C en liefst zelfs aan 0,5C. C is hierbij de laad-/ontlaadcapaciteit, die uitgedrukt worden in mAh of Ah.

# Constant Voltage charge
Wanneer de batterijspanning zijn maximum nadert, dan wordt overgeschakeld naar Constant Voltage charge, waar de spanning gelijk blijft zodat de batterij de maximale spanning bereikt en blijft aanhouden. Tijdens deze laadfase daalt de stroomsterkte geleidelijk aan naar 0 toe tot de batterij zijn capaciteit bereikt.