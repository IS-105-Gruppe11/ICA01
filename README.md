 Deltakere:
 
 Erdvik, Magnus
 Lie, Eva Kristine
 Nguyen, Philip
 Tellefsen, Erlend Frøysnes
 Van Dijk, Richard
 Younas, Osman
 
                                                          ICA01 - Gruppe 11

                                                             Oppgave 1.2.1

(1) 1 =  0001
1 bit  
(2) 2 = 0010
2 bit
(3) 5  = 0101 
3 bits
(4) 8  = 1000
4 bits
(5) 16 = 0001 0000
5 bits
(6) 256 = 0001 0000 0000
9 bits

For å konvertere fra desimaltall til bit-tall:

Metode som ble brukt er å dele desimaltallet på 2 og skrive 1 om det er rest og 0 om det ikke er helt til desimaltallet er lik null. Bittene legges sammen fra bunn til topp som igjen gir oss binærtallet.  (Den metoden som ble vist på tavlen). 

For å finne antall bits:

“A positive integer n has b bits when 2^(b-1) ≤ n ≤ 2^(b) – 1”

Konverter følgende binære tall til desimaltall (mest signifikante bit-en er til venstre): 

(1) 100 = 4
(2) 1001 = 9
(3) 1100110011 = 819

Metoden vi brukte var å først finne desimaltallet til alle bittene i binærtallet som er 1. Desimaltallet finner vi ved å gå fra høyre til venstre, den første bitten har desimaltallet 1, den neste 2, 4, 8, 16, osv. Så om bit = 1, tar vi ut desimaltallet til den biten, om bit = 0 tar vi det ikke ut. Slik gikk vi gjennom hele binærtallet. Deretter plusset vi sammen de desimaltallene vi tok ut som igjen gir oss svaret.



                                                            Oppgave 1.2.2 

Flere personer prøver å gjette et tresifret (3-bit) binært tall. 
(1) Lise har fått vite / lærer at tallet er et oddetall. 
(2) Per har fått vite at tallet er IKKE et multiplum av 3 (dvs. ikke 0, 3, 6). 
(3) Oskar har fått vite at tallet inneholder nøyaktig 2 enere. 
(4) Louise har fått vite alt det Lise, Per og Oskar vet. 
Hvor mye informasjon (i bits) har hver spiller fått? 

Svar:
Største 3 bit tall = 7 
N = 7 (totalt antall mulige valg)
M = antall valg personen får vite om
Formel: log2(1/(M/N)) -> log2(N/M) = informasjonsmengden i bits

Lise: 1, 3, 5, 7 -> M = 4
log2(7/4) = 0.807 = 1 bit
Per: 1, 2, 4, 5, 7 -> M = 5
log2(7/5) = 0.485 = 1 bit
Oskar: 3, 5, 6  (011, 101, 110) -> M = 3
log2(7/3) = 1.222 = 2 bit
Louise: 5 -> M = 1
log2(7/1) = 2.807 = 3 bit





                                                            Oppgave 1.2.3


Brukte Git Bash.
cd C:/
mkdir Work
git init.
git clone https://github.com/jeroenbijl92/Is105-uke4
Dro inn hello.go i notepad og skrev en oppdatering.
git status for å sjekke modifikasjonen.
git add hello.go
git commit -m "en melding til gruppen"
 Logge inn. git config user.name "your name"
git push origin master.
 Måtte også bruke git remote add for å linke til repository
git remote -v for å se om det stemte med riktig url.



                                                            Oppgave 1.2.4
                                                            
                                                            
                                                            
1) Hvilken fordeler og ulemper har en git-flow-modell med en hovedrepository? 

En av fordelene med Git, er at alle får en oversikt over hvor prosjektet er underveis.
Man kan lett klone alt innhold til sin egen pc, og jobbe med koden ,for å så legge til endringer med beskjed til medlemmene om at “dette er forandret”. 
Koden blir markert på en oversiktlig måte, så det gjør det lett for andre brukere og forstå innholdet og forandringene som blir gjort. 

Å lagre et prosjekt mot et felles repository, kan gjøre jobben lettere for en som vil ha innsikt i prosjektet ved å se historikken over endringer som har blitt utført. Denne oversikten gjør det vesentlig lettere for enhver å komme med foreslåtte endringer og løsninger.
Det er også en grei løsning for et felles oppbevaringssted for sine filer og prosjekter, som gir deg tilgang på dem når og hvor som helst.

Ulempene er at det gjerne krever litt tid, for å sette seg inn i modellen og lære seg alle kommandoene man må bruke for å få en fin flyt over arbeidet.
Igjen så virker det litt lite hensiktsmessig å bruke og holde kontroll over alle kommandoene man må gjøre i cmd, i stede for å bruke tradisjonelt GUI for å gjøre jobben og holde oversikt.
Men kan se verdien i modellen ved at det kan bli svært effektivt når man har fått en god forståelse over arbeidsmetoden. (kilde)



                                                            Oppgave 2
// Github mappe; “Hello”

Windows = .exe
OS = .dmg som mountes ved hjelp av .app extension.
Linux = RUN, OUT
BIN = Er en binary executable som Windows, OS og Linux kan kjøre.



De forskjellige operativsystemene opererer med forskjellige fil extensions for at systemene og programmene skal kunne tolke innholdet og hvordan det skal utføres.
Grunnen til at det er forskjellige object filer, er hvordan den binære koden og logaritmen er skrevet, og hvordan det skal bli tolket av datamaskinen.
Plattformene er bygd opp for å tolke de forskjellige logaritmene mest effektivt

                                                            Oppgave 3
// Github mappe; “logbase2”

Alle go programmer er bygd opp av pakker. Det er ingen bruk av klasser i go. Bruken av private og public variabler er også ikke tilstede.

Go kan kompilere direkte inn i en kjørende program fil, som kan bli kjørt av alle platformer av samme OS. Det er heller ikke bruk for en konstruktor.

Java behøver ; semicolon etter metoder og variabler.
For import metode, så er det ikke nødvendig og skrive import for hver eneste pakke som i java. I Go kan man stacke de sammen i et singel import kall.

For å kjøre en metode fra import pakken i Go, så bruker man alltid stor forbokstav.
Hvis man vil bruke 2 parameter typer av int, så trenger man bare spesifisere det en gang, ved å skrive x, y int.

Funksjonen .var oppretter en liste av variabler med typen spesifisert på slutten, omvendt rekkefølge i forhold til Java og uten priv/public.
Go gir deg anledning til å bruke := kommandoen for å referere til en ny variabel.
boolean er kortet ned til bool.

I Go trenger man ikke å oppgi type til variabelen, hvis verdien står bak =. Den blir gjenkjent automatisk. 

Java bruker static final “MAX” f.eks for å deklarere max som en konstant. Go gjør det mer effektivt ved å bruke const max = “verdien”.
Det er også innebygd array, kart og slices i Go.

Du kan bruke deklarasjonen “var” for å definere en rekke variabler av samme type. Eks: “var a, b, 1, 2, 3 boolean”. Du kan også gi variabler verdier ved bruk av “var”. Eks: 1, 2, 3, = true, false, “Ja”. 

I Go har man bare bruk av en for løkke, og man trenger ikke å legge inn parenteser rundt alle utførelsene. I stedet bruker man uttrykker som init, condition og post.

Hovedforskjellen fra Go til Java, er at Go er mer strukturert og krever litt mindre presisjon. Å definerer typer er blitt gjort enklere, og det er en vesentlig forkortning av nødvendig kode skriving for å oppnå det samme som i Java. (kilde)

                                                            Oppgave 4
Når man compiler på Go Lang så compiler slik at det er konfigurert til det plattformen man programmerer på f.eks. Linux / Windows, og når det er compiled så lagrer Go Lang hele standardbiblioteket (de du har brukt f.eks. fmt) slik at du kan kjøre programmet raskere.

Denne oppgaven viser at ved bruk av github/git er det lett å ta i bruk andres kode raskt og effektivt, samt legge ut din kode for andre gruppemedlemmer å bruke. 
Hvis noen av medlemmene ikke får kjørt sin kode, så kan man bruke flere medlemmer til å samarbeide om flere kreative løsninger og finne eventuelle feil i andre koder. Dette gir en mer effektiv ressursbruk av hverandres ideer og tankeganger. 
Etter vi har jobbet sammen på denne oppgaven, så har det gitt oss en bedre forståelse for hvordan man kan kjøre kode/beregninger ved hjelp av commands og en bedre forståelse for golang sin oppbygging.

log.go:


main.go:


Resultat i kommandolinje: (log2 av 8)


                                                            Oppgave 5

5) Er det hensiktsmessig å legge inn denne filen i git repository? Begrunn svaret!
// Github mappe; “logbase2input”
Filen logcli.go i  master branch kjøres ved "go run logcli.go (3 11)" der første parameter er LogBase-3 og andre parameter er LogBase-11. 


                                                            Oppgave 6

6) Hvordan skiller pakken log​, som dere har implementer, seg fra andre pakker i go, som, for eksempel, fmt​? 
// Github mappe; “LogProgram”

Hver pakke har forskjellige metoder som utfører forskjellige funksjoner.







 






