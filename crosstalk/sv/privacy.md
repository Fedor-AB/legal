---
title: Crosstalk — Integritetspolicy
lang: sv
version: 0.8.1-draft
effective_date: TBD
status: draft, not in force
---
# Crosstalk — Integritetspolicy

> Utkast för granskning. Gäller inte förrän Fedor AB publicerar det med ett ikraftträdandedatum. Text inom [hakparenteser] väntar på ett beslut av Fedor AB.

Det här är en svensk översättning av den engelska policyn, med samma versionsnummer: [Privacy policy](../privacy).

## 1. Vem som ansvarar

Fedor AB (org.nr 559537-2961) är personuppgiftsansvarig för de personuppgifter som beskrivs här. Kontakt för allt som rör dina uppgifter: <privacy@fedor.nu>. Postadress: Fedor AB, Fabriksvägen 8, 176 69 Järfälla, Sverige.

Crosstalk erbjuds i länder inom Europeiska unionen och Europeiska ekonomiska samarbetsområdet, och den här policyn är skriven för lyssnare där.

## 2. Kort sammanfattning

- Du skapar inget konto hos oss. Vi frågar inte efter ditt namn, din e-postadress eller ditt telefonnummer.
- För att använda Crosstalk behöver du ett Crosstalk-köp i App Store. Apple hanterar betalningen, och vi ser aldrig dina betalningsuppgifter.
- För att skriva det programledarna säger skickar appen uppgifter till vår server om låtarna runt den plats där du är i uppspelningen, din tidszon och ditt språk samt dina önskemål för programledarna.
- Vår server skickar den informationen vidare till en AI-leverantör som skriver manuset, och skickar manuset till en AI-leverantör som gör om det till tal. Appen ber om din tillåtelse innan det sker.
- Vi använder AI-verktyg från andra företag som hjälper oss att driva och reparera tjänsten. När de gör det arbetet kan de läsa det som vår databas innehåller om ditt lyssnande, sparat under en slumpmässig identifierare. De får inte del av de loggar som innehåller din IP-adress.
- Vi sparar en historik över de inslag med programledarna som du har hört. Den är knuten till en slumpmässig identifierare och inte till ditt namn.
- Vi använder inga verktyg för reklam eller spårning, vi använder inga analystjänster från andra företag och vi säljer inga uppgifter. [När kraschrapporter och användningsstatistik finns: vi samlar in dem själva, på vår egen server (avsnitt 3.5). Användningsstatistik samlas bara in om du slår på den.]

## 3. Vad vi behandlar och varför

### 3.1 Skickas varje gång ett inslag begärs

| Uppgift | Detaljer | Varför |
|---|---|---|
| Låtarna runt dig | För låten som just spelades och den som kommer härnäst: titel, artistnamn, album, år och utgivningsdatum, genre, märkning som explicit eller inte, spår- och skivnummer, kompositör och inspelningskod (ISRC). | För att programledarna ska kunna prata om musiken. |
| Vad du spelar från | Typen (spellista, album eller samling), dess titel och upp till 21 låtar runt den plats där du är. Titeln på en spellista är den du själv har gett den. | För att programledarna ska känna till låtens sammanhang. |
| Tid | Tiden då inslaget börjar och din tidszon. | För att programledarna ska veta vilken tid på dygnet och vilken veckodag det är. |
| Språk | Programmets språk, de språk som är inställda på din enhet och det programledarspråk du eventuellt har valt. | För att välja vilket språk programledarna talar. |
| Dina önskemål för programledarna | Det du har ställt in för programledarna i Inställningar, inklusive fritext som du har skrivit till dem. | För att programledarna ska kunna följa dem. |
| Uppgifter om appen | Appens identifierare och version. | För att kontrollera att din version av appen stöds. |

Vi får inte ditt Apple Music-bibliotek, din lyssningshistorik utöver låtarna ovan, ditt Apple-konto, din plats eller dina kontakter.

### 3.2 Identifierare

| Uppgift | Detaljer | Varför |
|---|---|---|
| Lyssnar-id | En slumpmässig identifierare som appen skapar och knyter till ditt köp av Crosstalk i App Store. Den är inte ditt namn eller ditt Apple-konto. [Bekräftas när den här delen av appen är byggd: identifieraren sparas i din iCloud-nyckelring, så att dina enheter delar den och den finns kvar när appen installeras om.] | För att hålla ihop din inslagshistorik och ge programledarna en röd tråd från ett inslag till nästa. |
| Appintegritetsnyckel | Skapas på din enhet av Apples tjänst App Attest, tillsammans med det intyg som Apple utfärdar för den. | För att bekräfta att förfrågningar kommer från en äkta kopia av appen och för att förhindra missbruk. |
| Sessionstoken | En kortlivad token som gäller i högst 15 minuter. | För att godkänna förfrågningar. |
| Köpuppgift | Den signerade transaktionsuppgiften från App Store för ditt Crosstalk-köp. Vår server läser ur den appens identifierare, produkten, utgångsdatumet, om köpet har återbetalats eller återkallats samt lyssnar-id:t. Den innehåller inget namn, inget Apple-konto och inga betalningsuppgifter. Vi kontrollerar uppgiften och sparar den inte. | För att bekräfta att du har rätt att använda tjänsten. |
| Nätverksadress | Din IP-adress, som vid all internetkommunikation. | För att leverera svar och skydda tjänsten. |

### 3.3 Skapas och sparas av oss

| Uppgift | Detaljer | Sparas i |
|---|---|---|
| Inslagshistorik | För varje inslag du har hört: när det sändes, titel, artist och album för låten före inslaget, manuset, programledarnas namn och en kort intern sammanfattning som används för att hålla den röda tråden. | 90 dagar |
| Inslag du inte hörde | Samma uppgifter för ett inslag som skapades men aldrig spelades upp. | 24 timmar |
| Ljudet till ett inslag | Det skapade ljudet, som sparas så att appen kan hämta det igen om anslutningen bryts. | 15 minuter |
| Uppgifter om förfrågningar | Vilka förfrågningar som gjordes, när, och om de lyckades. De innehåller lyssnar-id:t och inga uppgifter om låtar. | 30 dagar |
| Sessioner och bläddringsmarkörer | Den kortlivade sessionstoken (avsnitt 3.2) och de markörer som appen använder för att bläddra i din inslagshistorik. | Tills de går ut |
| Identifierare | Lyssnar-id:t och appintegritetsnyckeln med Apples intyg för den. | Appintegritetsnyckeln: 90 dagar efter att den senast användes. Lyssnar-id:t: tills inget som vi sparar hänvisar till det. |
| Felsökningsunderlag | Hela den text som skickades till AI-leverantören och dess svar, inklusive dina önskemål för programledarna. Avstängt i normal drift; vi slår på det bara för att utreda ett fel. | 30 dagar |
| Server- och nätverksloggar | Tekniska uppgifter om förfrågningar och fel: tid, begärd adress, resultat, din IP-adress, den app- och systemversion som din enhet uppger samt en hänvisning till appintegritetsnyckeln. [Ska bekräftas på produktionsservern: loggarna innehåller inga uppgifter om låtar och ingen text som du har skrivit till programledarna.] | 14 dagar |

[När funktionen ”Build your own show” finns: den beskrivning av stationen och programledarna som du skriver, resultatet av vår automatiska kontroll av den och den godkända världen, som sparas på din enhet.]

### 3.4 Sparas bara på din enhet

Appen sparar följande på din enhet och ingen annanstans:

- dina inställningar: dina önskemål för programledarna, det program- och programledarspråk du har valt och hur ditt bibliotek är sorterat. Dina önskemål för programledarna skickas med varje begäran om ett inslag (avsnitt 3.1) och sparas inte på vår server, utom i ett felsökningsunderlag (avsnitt 3.3);
- en lista över upp till 25 album och spellistor som du nyligen har öppnat, som hänvisningar utan titlar;
- en hänvisning till appintegritetsnyckeln;
- ljudet till ett inslag medan det spelas och, om ett inslag avbröts, det ljudet tillsammans med titel, artist och album för låten som följer efter det, så att inslaget kan fortsätta.

När du raderar appen tas de här uppgifterna bort. [Ska bekräftas: utom lyssnar-id:t, om det sparas i din iCloud-nyckelring.] [När användningsstatistik finns: och utom analysidentifieraren, se avsnitt 3.5.]

### 3.5 Kraschrapporter och användningsstatistik

[Det här avsnittet gäller när de två funktionerna finns. Användningsstatistiken är avstängd tills du slår på den. Kraschrapporter har en egen omkopplare i Inställningar, och Inställningar visar om den är påslagen.]

**Kraschrapporter.** Efter en krasch eller en låsning skickar appen den tekniska rapport som iOS har tagit fram till vår server: vilken del av appens kod som kördes (stackspårningen), appens version och bygge, enhetsmodellen och iOS-versionen. Innan rapporten skickas tar appen bort region, processnummer, minnesadresser, texten i felmeddelanden och den exakta tiden. Vi använder en rapport bara för att hitta och åtgärda felet. Rapporten innehåller ingen identifierare. [Ska bekräftas på produktionsservern: ingen loggrad kopplar en rapport till din IP-adress eller till din appintegritetsnyckel.] Vi sparar en rapport i 90 dagar. Du kan slå av kraschrapporter i Inställningar.

**Användningsstatistik.** Om du slår på den skickar appen en kort lista med händelser till vår server: när uppspelningen startar, hur lång tid det tar innan du hör ljud, när ett inslag börjar och slutar, när du hoppar över, när du slår på eller av programledarna och stegen från att du kommer i gång till köpet. Varje händelse innehåller en analysidentifierare, ett slumpmässigt nummer som appen skapar när du samtycker. [Ska bekräftas: analysidentifieraren är inte kopplad till ditt lyssnar-id eller din inslagshistorik.] Vi använder händelserna för att se hur appen fungerar och för att förbättra den. Vi använder också analysidentifieraren för att ge olika lyssnare olika versioner av en funktion och jämföra resultaten.

Analysidentifieraren sparas i enhetens nyckelring. Den finns kvar där om du raderar appen, och när du har installerat appen igen används den bara om du samtycker på nytt. När du slår av användningsstatistiken tas den bort från din enhet och de händelser som är sparade under den på vår server raderas genast. Ditt köp, din inslagshistorik och dina önskemål för programledarna påverkas inte. Vi sparar händelser i 90 dagar, och vi raderar allt som är sparat under en analysidentifierare efter 90 dagar utan aktivitet.

Vi driver båda på vår egen server. Inget analysföretag utanför oss tar emot de här uppgifterna. [Ska bekräftas: om AI-verktygen i avsnitt 5 kan läsa dem.]

## 4. Rättslig grund

- **Fullgöra vårt avtal med dig** (artikel 6.1 b i dataskyddsförordningen). Att kontrollera ditt köp, skapa inslag, spara din inslagshistorik och ge programledarna en röd tråd är det du ber Crosstalk att göra enligt [användarvillkoren](../terms) (på engelska).
- **Våra berättigade intressen** (artikel 6.1 f). Vi har ett intresse av att hålla tjänsten säker, förhindra missbruk och hålla tjänsten i gång. Det omfattar kontrollen av appens äkthet, gränser för hur ofta inslag kan skapas, loggar, felsökning och användningen av AI-verktyg för att övervaka och reparera tjänsten (avsnitt 5). [Om vi räknar aktiva installationer: det omfattar också att räkna hur många kopior av appen som har varit aktiva de senaste 30 dagarna. Vi räknar de lyssnar-id:n som har setts under den tiden och sparar bara summan.] [När kraschrapporter finns: där omkopplaren är påslagen från början omfattar det också att hitta och åtgärda fel med hjälp av kraschrapporter (avsnitt 3.5).] Du kan invända mot den här behandlingen; se avsnitt 8.
- **Ditt samtycke** (artikel 6.1 a). [När de finns:] användningsstatistik, och kraschrapporter där omkopplaren är avstängd från början och du slår på den (avsnitt 3.5). Du kan när som helst återkalla samtycket genom att slå av dem i Inställningar. Det påverkar inte det som har gjorts dessförinnan.

Före det första inslaget ber appen dig att tillåta delning med AI-tjänster. Skärmen säger kort vad som delas och varför, och den här policyn ger detaljerna: uppgifterna i avsnitt 3.1 och mottagarna i avsnitt 5. Din tillåtelse omfattar de AI-leverantörer som skriver och ger röst åt programledarna och de AI-verktyg som hjälper oss att driva tjänsten. Utan den tillåtelsen kan programledarna inte fungera, och inga av uppgifterna i avsnitt 3.1 skickas till vår server eller till någon AI-leverantör. Du kan när som helst ändra ditt val i Inställningar. När du slår av programledarna skickas inga nya uppgifter. Det som redan är sparat finns kvar under de tider som anges i avsnitt 3.3 och kan fortfarande läsas av AI-verktygen i avsnitt 5; du kan be oss radera det (avsnitt 8).

Appen kontaktar ändå vår server när den startar, för att kontrollera att din version stöds och att appen är äkta. Den kontakten lämnar de tekniska uppgifter som anges under ”Server- och nätverksloggar” i avsnitt 3.3. AI-verktygen i avsnitt 5 får inte del av de loggarna.

## 5. Vem som tar emot dina uppgifter

Vi anlitar andra företag i fyra roller. Vart och ett av dem är vårt personuppgiftsbiträde: det agerar enligt våra instruktioner och får inte använda dina uppgifter för egna ändamål. [Ska bekräftas för varje företag när avtalet med det är undertecknat.]

| Roll | Företag | Vad det tar emot | Ändamål |
|---|---|---|---|
| AI som skriver manus | [Företaget läggs till när avtalet är undertecknat. Vi räknar med att använda någon av Anthropics Claude-modeller, köpt antingen från Anthropic eller via en molnleverantör.] | Den text vi sätter samman för manuset: uppgifterna om låtar och spellista, tiden, dina önskemål för programledarna, programmets beskrivning och manusen till dina senaste inslag. Ingen identifierare för dig ingår. | Att skriva programledarnas manus. |
| AI för tal | Google [avtalsparten läggs till när avtalet är undertecknat] | Det färdiga manuset, de valda rösterna och språket. Ingen identifierare för dig ingår. | Att göra om manuset till tal. |
| Drift av servern | [Molnleverantören läggs till] | Allt som vår server lagrar. | Att driva vår server, i [EU-region]. |
| AI-verktyg som hjälper oss att driva tjänsten | [Företagen namnges här när de är valda.] Leverantörer av AI-modeller och AI-verktyg för programmering, som är amerikanska koncerner. Vi använder dem enligt företagsvillkor som gör dem till våra personuppgiftsbiträden. | Det ett verktyg läser medan det arbetar: databasen bakom tjänsten som den är, utom de tabeller som innehåller appintegritetsnycklar och sessionstoken, som är stängda för verktygen. Det omfattar din inslagshistorik, uppgifterna om förfrågningar och bläddringsmarkörerna (avsnitt 3.3), sparade under ditt lyssnar-id. [Ska bekräftas: om verktygen också kan läsa kraschrapporter och händelser i användningsstatistiken (avsnitt 3.5).] Dina önskemål för programledarna sparas inte i databasen. Ett felsökningsunderlag, när ett sådant är påslaget, innehåller dem, och då kan ett verktyg läsa personliga uppgifter som du har skrivit till programledarna. Vi har inte ditt namn eller ditt Apple-konto, så ett verktyg kan inte se dem. Verktygen får inte del av server- och nätverksloggarna, som innehåller IP-adresser. | Att övervaka tjänsten, hitta och åtgärda fel och underhålla den. |

Våra avtal med AI-leverantörerna tillåter inte att de tränar sina modeller på dina uppgifter. [Ska bekräftas mot varje undertecknat avtal.]

Om vi lägger till eller byter ett företag i den här tabellen publicerar vi först en ny version av den här policyn, och appen informerar dig om ändringen. Du kan när som helst fråga oss vilka företag som har tagit emot dina uppgifter.

Apple deltar som självständig leverantör, inte som vårt personuppgiftsbiträde: Apple levererar appen, säljer köpet till dig och tar emot betalningen, spelar musiken genom din Apple Music-prenumeration och utfärdar intyget om appens äkthet. För det Apple gör gäller Apples integritetspolicy.

Vi lämnar ut uppgifter till myndigheter bara när lagen kräver det.

## 6. Överföringar utanför EU/EES

Vår egen server drivs hos en molnleverantör inom EU: [leverantör och region läggs till].

AI-leverantörerna och leverantörerna av AI-verktyg i avsnitt 5 är amerikanska koncerner. Även när vårt avtal är med en leverantörs europeiska bolag kan det bolaget och dess koncernbolag behandla uppgifter i USA och andra länder. Sådana överföringar omfattas av Europeiska kommissionens standardavtalsklausuler eller, för amerikanska företag som är certifierade enligt det, av dataskyddsramen mellan EU och USA (EU-US Data Privacy Framework). Du kan be oss om en kopia av skyddsåtgärderna.

## 7. Hur länge vi sparar uppgifter

Tiderna anges i avsnitt 3.3. När en tid har gått ut raderar vi uppgifterna. Om du ber oss radera dina uppgifter raderar vi din inslagshistorik, uppgifterna om dina förfrågningar och dina identifierare utan att vänta på att tiderna går ut [och, när användningsstatistik finns, allt som är sparat under din analysidentifierare].

AI-leverantörerna sparar det innehåll vi skickar till dem under en begränsad tid enligt sina egna villkor, för att upptäcka missbruk, och raderar det sedan. [Tiderna ska bekräftas mot de undertecknade avtalen.]

## 8. Dina rättigheter

Du har rätt att:

- få en kopia av de personuppgifter vi har om dig;
- få felaktiga uppgifter rättade;
- få dina uppgifter raderade;
- få vår användning av dina uppgifter begränsad;
- få de uppgifter du har lämnat i ett portabelt format;
- invända mot behandling som vi grundar på våra berättigade intressen;
- när som helst återkalla ett samtycke som du har gett. [När användningsstatistik finns: genom att slå av den i Inställningar.]

Eftersom du inte har något konto hos oss kan vi bara hitta dina uppgifter genom lyssnar-id:t i din app. Skriv till <privacy@fedor.nu>. [Läggs till när det är byggt: hur du raderar dina uppgifter från appens Inställningar och var appen visar din identifierare.] Vi svarar inom en månad.

Du kan också lämna in ett klagomål till Integritetsskyddsmyndigheten (IMY), <https://www.imy.se>, eller till dataskyddsmyndigheten i det land där du bor.

## 9. Barn

Crosstalk är för vuxna. Du måste vara minst 18 år. Appen har åldersgränsen 18+ i App Store, och vi behandlar inte medvetet uppgifter om någon som är yngre.

## 10. Automatiska kontroller

[När funktionen ”Build your own show” finns: en värld som du skapar kontrolleras automatiskt mot våra regler innan den kan användas. Du kan be att en människa tittar på ett avslag genom att skriva till oss.]

Vi fattar inga beslut om dig som har rättsliga följder eller på liknande sätt påverkar dig i betydande grad enbart genom automatiserad behandling.

## 11. Säkerhet

Uppgifter skickas mellan appen och vår server över en krypterad anslutning. Förfrågningar tas bara emot från en äkta kopia av appen. Åtkomsten till servern och uppgifterna på den är begränsad till de personer på Fedor AB som driver tjänsten och till de AI-verktyg de använder för det arbetet, som beskrivs i avsnitt 5.

## 12. Ändringar av den här policyn

Varje version har ett versionsnummer och ett ikraftträdandedatum högst upp. Om vi gör en väsentlig ändring informerar appen dig och ber dig vid behov att godkänna den nya versionen. Tidigare versioner finns kvar på <https://legal.fedor.nu/crosstalk/>.
