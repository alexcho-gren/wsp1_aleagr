Vecka 4

12/11/2026

Läste genom kapitel 4.
Gjorde Genomgång och Gör det själv
Kapitel 4, sida 73-75. Genomgång + Gör det själv:
Konfiguerade två switchar med tre VLAN till vardera port med en trunk mellan dem, båda switchar fick en PC inkopplad i samma VLAN. Det gick att pinga mellan båda PCs.
Tog bort vlan 30 från trunkens allowed-lista på Switch-1. Pingade, fick 'request timed out (100% packet loss)'
Skrev show interfaces trunk på båda switchars terminal.
Utdatan är den samma på båda förutom att vlan 30 saknas på Switch-1's utdata. 
Ändrade tillbaka vlan 30 på Switch-1. Ändrade sedan Switch-2's native vlan till vlan 1.

Fick utdatan: 

    %CDP-4-NATIVE_VLAN_MISMATCH: Native VLAN mismatch discovered on GigabitEthernet0/1 (1), with Switch-1 GigabitEthernet0/1 (999).

13/11/2026

Skrev basen till veckans Python-skript. Fick utdatan:

    vlan 10
    name KONTOR
    vlan 20
    name EKONOMI
    vlan 30
    name GAST
    vlan 99
    name DRIFT

Repeterade kapitel 4. Svarade på frågorna i återblicken.

Återblick:

4.20:

IP-adressen är 192.168.1.128. Prefixet för nätmasken är /26. /26 har blocksteget 64. 0, 64, 128, 192. 
128 ligger mellan 128 och 192. Nätadressen är då 192.168.1.128. Nästa nät börjar på 192.
Broadcastadressen är nätet efter nätadressen minus 1. Då är broadcastadressen 192.168.1.191.
Den första enheten får IP-adressen 192.168.1.129. Den sista enheten får IP-adressen 192.168.1.1.190.
Mellan dem finns det 60 lediga adresser. Totalt blir det 62 adresser. Adressintervallen är då 192.168.1.129 - 192.168.1.190.
      
      Kort svar:
      Nätadress: 192.168.1.128
      Broadcastadress: 192.168.1.191
      Adressintervall: 192.168.1.129 192.168.1.190

4.21: 

Adressen FF:FF:FF:FF:FF:FF betyder: på alla enheter, från alla tillverkare: till alla på det här nätet.
Om switchen får broadcastadressen som mottagare för en ram så skickar den ramen genom alla portar utom
den port ramen kom in på. Alla enheter på alla andra portar tar emot ramen och avgör om det angår dem.

4.22: 

Kolumnen 'Vlan'. Om två portar har olika VLAN ska dem inte kunna skicka data mellan varandra.
Om en enhet på en port med ett VLAN ska skicka en ram till en enhet på en annan port i samma 
switch, så måste mottagarens port ha samma VLAN som anvsändarens port. Om det är mellan två
portar på två olika switchar så måste det finnas en trunk mellan de två switcharna, som också
måste vara exakt likadant konfigurerad i båda ändar.


14/11/2026

Gjorde veckans koan. Kopierade test_koans.py ut ur repot och gjorde den utanför repot till att börja med.
Skrev ett commit-meddelande till varje grupp + återblick i ett text-dokument, också utanför repot.

15/11/2026

Skrev in svaren på veckans koan i repot. Commitade alla grupper m. meddelande. Pushade till branch week-04/alexander-agren.
Skrev om veckans Python-skript efter instruktion i 'Veckans Python'.
Satt och sysslade med genomgångar i tidigare kapitel i Packet Tracer.

16/11/2026

Läste kapitel 5.
Gjorde veckans checkpoint. Ska lägga till allt i en ny mapp i /uppgifter på repot.
Pushar sen till en ny branch som heter uppgifter/alexander-agren efter jag skrivit färdigt i dagbok.md.
Efter det ska jag läsa genom kapitel 5 igen.

