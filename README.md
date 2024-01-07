# Automatische-voedingsbak-voor-dieren


## 1. Probleem in het dagelijks leven

Een veelvoorkomend probleem bij huisdierhouders is dat ze af en toe wel eens kunnen vergeten hun huisdier eten te geven of juist meerdere keren per dag ook al is dit niet de bedoeling. Dit kan leiden tot ongezonde eetpatronen en het niet juist opvolgen van hun dieet. Dit komt vaak voor als hun baasje een drukke periode heeft of er meerdere mensen in het gebouw wonen en niet goed communiceren over dat het huisdier al dan niet eten heeft gekregen.

Door middel van onze automatische voederbak kun je dit tegen gaan. Je kunt deze instellen dat uw huisdier de volledige tijd voldoende eten heeft of dat deze gevoed wordt op 1 of meerdere momenten doorheen de dag. Dit kan helpen bij het opbouwen van een gezond eetpatroon en helpt bij het opvolgen bij diëten.

## 2. Project Canvas

![Alt text](<Foto's/Project canvas.jpg>)

## 3. SWOT analyse

#### Sterktes

- Het is een handige tool om ervoor te zorgen dat je huisdier nooit meer zonder eten kan zitten.
- Als het eetpatroon van je huisdier zou veranderen kun je dit opvolgen. Hierdoor kun je vroegtijdig ziekte opsporen.
- Onze automatische voederbak is instaat om via WIFI gegevens door te sturen naar de gebruiker. De gebruiker kan daardoor overal ter wereld realtime gegevens zien over het eetgedrag van hun huisdier, wanneer heeft deze voor het laatst gegeten, hoeveel heeft deze gegeten, is er een verandering in het eetpatroon, …
- De batterij indien de gebruiker wenst te gebruiken zijn oplaadbaar via USB-C

#### Zwaktes

- Als de gewichtssensoren niet nauwkeurig zijn of gevoelig zijn voor externe factoren zoals trillingen, kan dit de betrouwbaarheid van het systeem beïnvloeden. Onnauwkeurige metingen kunnen leiden tot onjuiste meldingen over het voerniveau en mogelijk tot overmatige of onvoldoende voedselafgifte.
- Als je ervoor kiest om geen voedingsspanning te leveren via de kabel maar via de batterijen is er een kans dat er een stroomuitval plaats vindt en je huisdier toch niet automatisch gevoed wordt.
- Batterijen opladen duurt redelijk lang we hebben ervoor gekozen om geen fastcharging te gebruiken aangezien dit hier overbodig zou zijn aangezien de automatische voederbak zowel kan opladen en werken tegelijk.

#### Opportuniteit

- Onze automatische voederbak is in staat om honden, katten, konijnen, … die op dieet zijn aangepaste voeding patronen te geven. Je kunt dit instellen via de app, je kunt de tijdstippen instellen en de hoeveelheid in geven. Aangezien er dieren zijn die maar zouden blijven eten.
- Als u onze automatische voederbak aankoopt kiest u ook niet alleen voor een uitgebreide en modieuze automatische voederbak maar ook voor een milieuvriendelijke voederbak. Ons doel was niet alleen één van de beste of de beste automatische voederbak te ontwerpen maar ook een milieuvriendelijke.

#### Bedreigingen

-	Er is veel concurrentie in de automatische voederbak markt, veel mensen willen ook geen 75-150 euro betalen voor een voederbak.
-	Het is heel gemakkelijk om een sensorstoring te hebben aangezien er steeds eten naar beneden valt en deze steeds een beetje afgeeft. Het zal dus van belang zijn dat de gebruiker regelmatig de sensoren kuist.

## 4. Prototype

Aan de hand van onze prototypes hebben we een realistische en haalbare grootte kunnen kiezen om daarop later onze PCB's en onze motoren te baseren. Hoe groot kan onze PCB zijn? Hoe groot zijn de kleppen die opengaan? Hoe groot wordt de lade om de bak bij te vullen? Hoe groot kunnen de motoren zijn? Waar kunnen we het beste onze microcontroller met Wi-Fi plaatsen? Dit soort prototypes kunnen ervoor zorgen dat je veel informatie verkrijgt. We hebben een prototype uit karton om in levende lijve te kunnen kijken en meten waar alles zou kunnen passen, en een 3D-model dat al een heel stuk dichter bij het eindresultaat komt.

![Alt text](<Foto's/3D project voorkant open.png>)

3D ontwerp voorkant met open kleppen

![Alt text](<Foto's/3D project voorkant gesloten.png>)

3D onwerp voorkant met gesloten kleppen.

![Alt text](<Foto's/3D project zijkant.png>)

3D ontwerp zijkant

![Alt text](<Foto's/3D project achterkant.png>)

3D ontwerpt achterkant

![Alt text](<Foto's/Prototype 1_1.jpg>)

Prototype voorkant

![Alt text](<Foto's/Prototype 1_2.jpg>)

Prototype onderkant

## 5. Testen van het systeem

#### Test 1, kan de sensor gewicht meten?

Als eerste test zou je de code kunnen testen deze zal vaak eerder klaar zijn dan de PCB en zal ook meer tijd en aandacht nodig hebben. Als het stuk code dat instaat om gewicht the meten, kunnen we de gewicht op de sensor leggen en kijken of de gegevens wel aanpassen en juist zijn. Als deze dit juist meet zal er bij een klein gewicht een lampje branden later vervangen door de motoren.
Deze test is geslaagd als het stuk code alleen maar het lampje aanstuurt als de sensor en gewicht meet dat kleiner is dan de ingestelde waarde .

#### Test 2, motoren aansturen

Als test 1 het gewenste resultaat heeft opgeleverd kunnen we nu test 2 uitvoeren. Deze test bestaat uit een nieuw stuk code waar de motoren mee kunnen worden aangestuurd en een stuk code waar het gewicht wordt gemeten, dit is dezelfde code die werd gebruikt in de eerste test enkel is hier een delay van 5 seconden ingesteld tussen het moment dat het blokje hout weg wordt genomen en het moment dat de motoren beginnen te draaien. 
Deze test is geslaagd als we een blokje weg nemen en na een delay van 5 seconden de motoren 90° draaien. De delay kan worden gemeten via een stopwatch of via een oscillator.

#### Test 3, Alles in bouwen

Als test 2 het gewenste resultaat heeft opgeleverd kunnen we nu de laatste test uitvoeren test 3. Deze test bestaat eruit dat alle onderdelen en PCB’s ingebouwd worden en aangesloten.
Deze test is geslaagd als we een blokje wegnemen van de sensor en na een delay van 5 seconden er hondenbrokken naar beneden vallen voor een duur van 3 seconden. Na een delay van 10 seconden om de korrels wat tijd te geven om stil te blijven liggen zal het gewicht nog eens gemeten worden. Als het gewicht de verwachte waarde heeft zullen de motoren niet meer draaien. Als het gewicht minder is dan verwacht zullen de motoren opnieuw 90° draaien voor een duur tijd van 3 seconden en zo weer de cyclus her lopen. 



