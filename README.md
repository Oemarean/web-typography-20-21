# Web Typography, 2020/2021
### scroll to onderbouwing bottom part

Als je doof bent, of als je om een andere reden geen geluid kunt horen, dan mis je veel informatie als je een film kijkt. Knisperende voetstappen, langzaam aanzwellende muziek, nerveus getik op een deur, je hoort het natuurlijk allemaal niet. Nu bestaat er zoiets als *closed caption*, wat een type ondertiteling is waarbij ook dingen als omgevingsgeluiden en de muziek beschreven worden. Hierdoor krijgt een kijker die informatie wel binnen.

Alleen wordt die auditieve informatie nogal neutraal beschreven. Het geluid van huilend persoon zou bijvoorbeeld beschreven kunnen worden als *snikgeluid op de achtergrond*. En iemand die lacht zou geschreven kunnen worden als *iemand lacht.* Heel neutraal, bijna zakelijk, en bovendien allebei in precies hetzelfde neutrale lettertype. Terwijl het toch echt over twee heel verschillende emoties gaat. 

Dat kan visueel sterker. 

En dat gaan jullie doen.

## Leerdoelen

- Je kan de kennis over vormgeving die je hebt opgedaan tijdens de minor technisch toepassen met behulp van CSS
- Je kan verborgen nuance uit een audiotrack overtuigend vertalen naar visuele (typografische) beelden
- Je kan je typografische keuzes onderbouwen.
- Je hebt de exclusive design principles gebruikt.

## Oplevering

Je levert een werkende versie op, gemaakt met HTML, CSS en JavaScript. Deze staat op Github. In een duidelijke readme documenteer en onderbouw je je ontwerpkeuzes. Je developmentgeschiedenis is terug te vinden op GitHub.

Je levert ook een *screen recording* met audio op van je fragment. Dit is een video van de definitieve versie, gemaakt van jouw browserscherm.

De beoordeling is mondeling en volgt [de rubric uit het beoordelingsformulier](web-typografie-beoordeling.pdf).

## Typografische restricties

Je *moet* een van deze twee opties kiezen, en je keuze moet je onderbouwen. In je readme staat een uitleg over je overwegingen om de ene of de andere restrictie te kiezen.

### Optie 1: Systeemfont

De eerste optie is dat je gebruik maakt van het zogenaamde *systeemfont* van degene die naar jouw werk kijkt. Dit font verschilt per operating system, en het verschilt soms zelfs per versie van het operating system. Het is ook aan te passen door de gebruiker zelf. 

Je hebt dus geen controle over welk lettertype er precies gebruikt wordt. Het levert dus een onzeker, en beperkt typografisch palet op. Je hebt geen *light* versies, of *extrabold*. En ook geen serif en sans-serif versie van dezelfde familie. In dit geval heb je alleen de beschikking over normal, **bold** en _italic_. Dit heeft natuurlijk ook zijn voordelen!

### Optie 2: Brenner

Je kan er ook voor kiezen om gebruik te maken van de complete Brenner familie. Dit is een zeer uitgebreid en uiterst flexibel font. [Hier kan je je verdiepen in dit font](https://www.typotheque.com/blog/brenner_an_unusual_typeface_family_with_distinct_voices). Als je kiest voor dit font dan heb je de beschikking over een *sans serif*, een *condensed*, een *serif*, een *monotype*, een *slab*, een *display* en een *script* versie. En veel van deze versies hebben varianten van *light* tot *bold*, en allemaal zowel *bold* als *italic*.

Met Brenner zijn er natuurlijk veel en veel meer mogelijkheden dan met systeemfonts. Dat kan zowel een voordeel als een nadeel zijn. 

Voor een overzicht, zie [de brenner.pdf](brenner.pdf).

## Het fragment

Ik heb een fragment voorbereid. Het gaat om twee scenes uit *Blade Runner 2049*. De captions staan in de HTML, en ze verschijnen in sync met de video. [Kijk maar](closed-captions/index.html).

### De captions

De captions staan in de html, in het bestand index.html. Je kan aan elke paragraaf eventueel een of meer classes toevoegen. Bijvoorbeeld `voice1` of `voice2 soft`. Classes voeg je handmatig toe in de html.

Met JavaScript worden er een paar dingen extra gedaan: 

- er wordt aan elke paragraaf een unieke class toegevoegd (`p0`, `p1`, etc)
- Elk woord wordt in een aparte `span` gezet. Hierdoor kan je elk woord apart stylen, en eventueel ook [na elkaar laten verschijnen](https://github.com/cmda-minor-vid/web-typography-18-19/blob/master/closed-captions/css.css#L41).

### Tijdens het afspelen

Tijdens het afspeelen wordt er een class `on` op de caption gezet als hij moet verschijnen, en een class `off` als hij klaar is. *Zowel class `on` als class `off` blijft op de caption staan!*

De timimg van de captions kan je aanpassen in [closed-captions/captions.js](closed-captions/captions.js).

Er verschijnen ook classes op de body op momenten dat er geluiden worden afgespeeld, zoals `sound1` en `sound2`. Je kan geluiden toevoegen in [closed-captions/sounds.js](closed-captions/sounds.js).

*let op,* de geluiden zijn niet compleet, dit zal je zelf moeten aanvullen.

## Een eigen fragment (afgeraden, uitgebreide onderbouwing is nodig)

Je kan er ook voor kiezen om een eigen, *beter* fragment te gebruiken. Dit wordt afgeraden. De tijd die je besteedt aan het zoeken naar dat fragment kan je beter besteden aan het werken aan de opdracht. Bovendien blijkt dat er vaak fragmenten worden gekozen die niet goed voldoen aan de opdracht. Als je een ander fragment kiest dan *moet* je dit goed onderbouwd voorleggen aan je docent. De deadline hiervoor is vrijdagochtend in de eerste week.

### Waar moet je op letten bij het kiezen van een eigen fragment.
Lees de opdracht nog eens goed door. Waar gaat het ook al weer precies om? 

Voor een goede onderbouwing van je keuze voor een ander fragment moet je deze vragen in elk geval beantwoorden:

- Welke informatie zit er in de audio die echt niet zichtbaar is?
- Welke rol speelt de audio in het fragment?
- Werkt de scene nog zonder geluid?
- Waarom is dit fragment beter dan het aangeboden fragment?

Je kan dan de nodige HTML en JavaScript genereren door gebruik te maken van [caption generator](https://cmda-minor-vid.github.io/web-typography-18-19/generator/) (in Google Chrome). 

Als je de closed captions wil bewerken dan kan je een tool zoals [Amber Script](https://www.amberscript.com/en) gebruiken. Daar kan je exporteren als `.srt`, en die kan je weer door de generator halen.

### Feedback.

Week 1. 
Connectie maken met github en voorbereiden voor het gesprek met Darice.

Gesprek Darice:
Tijdens het gesprek werden er vragen gesteld over typografie en achtergrond (gifs) 
Het was al snel duidelijk dat Darice vind dat ik het rustig moet aanpakken met de gifs want
het kan de aandacht van de film weg trekken.

Week 2.

Mij focus ging richting de achtergronden.
Had samen met Karim afgesproken dat hij aan typografie bezig was en dat ik met 
focus met de achtergronden. Hierdoor kunnen we kijken wat Darice goed aan vind
en wat ze slecht aan vind.

Gesprek Darice:
Al snel was het duidelijk dat het overweldigend is en dat sommige gifs niet aansloten
op het video moest me daar meer op focussen. Verder was het duidelijk dat de typografie
in een keer moest komen en niet stapgewijs. Gebruiker vond het niet fijn om daar de tekst te
lezen hierdoor gaat tijd kwijt aan het video.

Gesprek Coach:
Moest meer research doen met de gifs keuzes en typografie was niet goed.
Verder moest ik even contrast checker gaan doen om te kijken of het daadwerkelijk de correcte
keuze was voor de kleur van de typografie.

Week 3.

Gesprek Coach:
Leesbaarheid van tekst was te ver uit elkaar. Vond inderdaad dat de gebruiker steeds op en
neer moest gaan lezen waardoor je snel moe raakt van het lezen. Verder had ik geen oude versie
van mijn oude werk waarbij ik kleuren had gebruikt binnen de typografie.


### Onderbouwing.

Voor de closed captions heb ik gekozen voor een unique ervaring van film kijken.
Omdat het gaat om een gebruiker dat slechthorend is heb ik me gefocused om de film
ervaring te verbeteren.

Doordat de gebruik misschien geen audio kan horen wil ik dat de gebruiker het kan
zien wat voor soort audio er bij komt spelen. Typografisch is het moeilijk op te lossen
met een systeemfont maar had hierdoor meer vrijheid met mijn beperkte keuzes. Doordat ik
voor systeemfont kies wou ik me meer het daarom heen wat ontwerpen.

Kleur gebruik typografie.
De reden waarom ik weinig gebruik maakte met de kleuren in het typografie is omdat het anders
veels te veel word voor de gebruiker om zowel het video als achtergronden als typografie nog 
te volgen. Hierdoor ben ik van de kleur gebruik afgegaan. (zie map 'Examples' Color text) 

Waarom gifs?
De reden waarom ik voor unique backgrounds gebruik is omdat ik geen simpele kleuren wil gebruiken voor
verandering binnen het video. Wil het fris en unique houden door middel van gifs. Hierdoor
voelt het video meer interactief met de verschillende gifs.

Gif keuzes.
Mijn keuzes in gifs waren vooral dat het een verrassende effect gaf op het video.
Doordat ik medeklasgenoten alleen maar met kleur ziet spelen vond ik het video geen
extra nuances geven. (lackluster in mijn opinie) Wou doormiddel van een gif
een extra flaire toevoegen.




