---
title: Crosstalk — Integritetspolicy
lang: sv
version: 0.5.1-draft
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
- För att skriva det programledarna säger skickar appen uppgifter till vår server om låtarna runt den plats där du är i uppspelningen, din tidszon och ditt språk samt det meddelande du eventuellt har skrivit till programledarna.
- Vår server skickar den informationen vidare till en AI-leverantör som skriver manuset, och skickar manuset till en AI-leverantör som gör om det till tal. Appen ber om din tillåtelse innan det sker.
- Vi använder AI-verktyg som hjälper oss att driva och reparera tjänsten. När de gör det arbetet kan de läsa det som vår server sparar om ditt lyssnande. De får inte del av de loggar som innehåller din IP-adress eller dina identifierare.
- Vi sparar en historik över de inslag med programledarna som du har hört. Den är knuten till en slumpmässig identifierare och inte till ditt namn.
- Vi använder inga verktyg för reklam, analys eller spårning, och vi säljer inga uppgifter.

## 3. Vad vi behandlar och varför

### 3.1 Skickas varje gång ett inslag begärs

| Uppgift | Detaljer | Varför |
|---|---|---|
| Låtarna runt dig | För låten som just spelades och den som kommer härnäst: titel, artistnamn, album, år och utgivningsdatum, genre, märkning som explicit eller inte, spår- och skivnummer, kompositör och inspelningskod (ISRC). | För att programledarna ska kunna prata om musiken. |
| Vad du spelar från | Typen (spellista, album eller samling), dess titel och upp till 21 låtar runt den plats där du är. Titeln på en spellista är den du själv har gett den. | För att programledarna ska känna till låtens sammanhang. |
| Tid | Tiden då inslaget börjar och din tidszon. | För att programledarna ska veta vilken tid på dygnet och vilken veckodag det är. |
| Språk | Programmets språk, de språk som är inställda på din enhet och det programledarspråk du eventuellt har valt. | För att välja vilket språk programledarna talar. |
| Ditt meddelande | Fritext som du har skrivit till programledarna i Inställningar, om du har gjort det. | För att programledarna ska kunna svara på det. |
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
| Identifierare | Lyssnar-id:t och appintegritetsnyckeln med Apples intyg för den. | [Lagringstiden ska beslutas] |
| Felsökningsunderlag | Hela den text som skickades till AI-leverantören och dess svar. [Ska bekräftas: avstängt i normal drift och påslaget bara under en begränsad tid för att utreda ett fel.] | 30 dagar |
| Server- och nätverksloggar | Tekniska uppgifter om förfrågningar och fel: tid, begärd adress, resultat, din IP-adress, den app- och systemversion som din enhet uppger samt en hänvisning till appintegritetsnyckeln. [Ska bekräftas på produktionsservern: loggarna innehåller inga uppgifter om låtar och ingen text från ditt meddelande.] | 14 dagar |

[När funktionen ”Build your own show” finns: den beskrivning av stationen och programledarna som du skriver, resultatet av vår automatiska kontroll av den och den godkända världen, som sparas på din enhet.]

### 3.4 Sparas bara på din enhet

Appen sparar följande på din enhet och ingen annanstans:

- dina inställningar: ditt meddelande till programledarna, det program- och programledarspråk du har valt och hur ditt bibliotek är sorterat;
- en lista över upp till 25 album och spellistor som du nyligen har öppnat, som hänvisningar utan titlar;
- en hänvisning till appintegritetsnyckeln;
- ljudet till ett inslag medan det spelas och, om ett inslag avbröts, det ljudet tillsammans med titel, artist och album för låten som följer efter det, så att inslaget kan fortsätta.

När du raderar appen tas de här uppgifterna bort. [Ska bekräftas: utom lyssnar-id:t, om det sparas i din iCloud-nyckelring.]

## 4. Rättslig grund

- **Fullgöra vårt avtal med dig** (artikel 6.1 b i dataskyddsförordningen). Att kontrollera ditt köp, skapa inslag, spara din inslagshistorik och ge programledarna en röd tråd är det du ber Crosstalk att göra enligt [användarvillkoren](../terms) (på engelska).
- **Våra berättigade intressen** (artikel 6.1 f). Vi har ett intresse av att hålla tjänsten säker, förhindra missbruk och hålla tjänsten i gång. Det omfattar kontrollen av appens äkthet, gränser för hur ofta inslag kan skapas, loggar, felsökning och användningen av AI-verktyg för att övervaka och reparera tjänsten (avsnitt 5). Du kan invända mot den här behandlingen; se avsnitt 8.

Före det första inslaget ber appen dig att tillåta två saker: att uppgifterna i avsnitt 3.1 skickas till de AI-leverantörer som skriver och ger röst åt programledarna, och att de AI-verktyg som vi använder för att driva tjänsten får läsa det som vår server sparar om ditt lyssnande. Skärmen namnger företagen. Utan den tillåtelsen kan programledarna inte fungera, och inga av de uppgifterna skickas till vår server eller till någon AI-leverantör.

Appen kontaktar ändå vår server när den startar, för att kontrollera att din version stöds och att appen är äkta. Den kontakten lämnar de tekniska uppgifter som anges under ”Server- och nätverksloggar” i avsnitt 3.3. AI-verktygen i avsnitt 5 får inte del av de loggarna.

## 5. Vem som tar emot dina uppgifter

Vi anlitar andra företag i fyra roller. Vart och ett av dem är vårt personuppgiftsbiträde: det agerar enligt våra instruktioner och får inte använda dina uppgifter för egna ändamål. [Ska bekräftas för varje företag när avtalet med det är undertecknat.]

| Roll | Företag | Vad det tar emot | Ändamål |
|---|---|---|---|
| AI som skriver manus | [Företaget läggs till när avtalet är undertecknat. Vi räknar med att använda någon av Anthropics Claude-modeller, köpt antingen från Anthropic eller via en molnleverantör.] | Den text vi sätter samman för manuset: uppgifterna om låtar och spellista, tiden, ditt meddelande, programmets beskrivning och manusen till dina senaste inslag. Ingen identifierare för dig ingår. | Att skriva programledarnas manus. |
| AI för tal | Google [avtalsparten läggs till när avtalet är undertecknat] | Det färdiga manuset, de valda rösterna och språket. Ingen identifierare för dig ingår. | Att göra om manuset till tal. |
| Drift av servern | [Molnleverantören läggs till] | Allt som vår server lagrar. | Att driva vår server, i [EU-region]. |
| AI-verktyg som hjälper oss att driva tjänsten | Anthropic och OpenAI [avtalsparterna läggs till när avtalen är undertecknade] | Det ett verktyg läser medan det arbetar: din inslagshistorik, uppgifterna om förfrågningar och felsökningsunderlaget (avsnitt 3.3). Verktygen får inte del av server- och nätverksloggarna, som innehåller IP-adresser, eller identifierarna i avsnitt 3.2. [Ska bekräftas före publicering: om verktygen kan se det lyssnar-id som din inslagshistorik och uppgifterna om förfrågningar är sparade under.] | Att övervaka tjänsten, hitta och åtgärda fel och underhålla den. |

Våra avtal med AI-leverantörerna tillåter inte att de tränar sina modeller på dina uppgifter. [Ska bekräftas mot varje undertecknat avtal.]

Om vi lägger till eller byter ett företag i den här tabellen publicerar vi först en ny version av den här policyn, och appen informerar dig om ändringen.

Apple deltar som självständig leverantör, inte som vårt personuppgiftsbiträde: Apple levererar appen, säljer köpet till dig och tar emot betalningen, spelar musiken genom din Apple Music-prenumeration och utfärdar intyget om appens äkthet. För det Apple gör gäller Apples integritetspolicy.

Vi lämnar ut uppgifter till myndigheter bara när lagen kräver det.

## 6. Överföringar utanför EU/EES

Vår egen server drivs hos en molnleverantör inom EU: [leverantör och region läggs till].

AI-leverantörerna i avsnitt 5 är amerikanska koncerner. Även när vårt avtal är med en leverantörs europeiska bolag kan det bolaget och dess koncernbolag behandla uppgifter i USA och andra länder. Sådana överföringar omfattas av Europeiska kommissionens standardavtalsklausuler eller, för amerikanska företag som är certifierade enligt det, av dataskyddsramen mellan EU och USA (EU-US Data Privacy Framework). Du kan be oss om en kopia av skyddsåtgärderna.

## 7. Hur länge vi sparar uppgifter

Tiderna anges i avsnitt 3.3. När en tid har gått ut raderar vi uppgifterna. Om du ber oss radera dina uppgifter raderar vi din inslagshistorik, uppgifterna om dina förfrågningar och dina identifierare utan att vänta på att tiderna går ut.

AI-leverantörerna sparar det innehåll vi skickar till dem under en begränsad tid enligt sina egna villkor, för att upptäcka missbruk, och raderar det sedan. [Tiderna ska bekräftas mot de undertecknade avtalen.]

## 8. Dina rättigheter

Du har rätt att:

- få en kopia av de personuppgifter vi har om dig;
- få felaktiga uppgifter rättade;
- få dina uppgifter raderade;
- få vår användning av dina uppgifter begränsad;
- få de uppgifter du har lämnat i ett portabelt format;
- invända mot behandling som vi grundar på våra berättigade intressen.

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
