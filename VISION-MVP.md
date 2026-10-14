# Viðskiptamarkmið, framtíðarsýn og Minimum Viable Product

**Verkefni 3 — Vision and Scope**

**Heiti kerfis:** Cafeteria Ordering System (COS)

**Teymi og höfundar:** Hópur 0, Ebba Þóra Hvannberg

**Git repository:** https://github.com/Hvannberg/HBV301G-Verkefni3-lausn

Þetta eru drög að sýnislausn fyrir COS í HBV301G 2026 samkvæmt template-i. Efnið byggir á  [verkefni 1](https://github.com/Hvannberg/HBV301G-2026-COS) og [verkefni 2](https://github.com/Hvannberg/HBV301G-Verkefni2-lausn).

Við yfirferð var einnig stuðst við [verkefnislýsingu ársins](Heimildir/Verkefni%203%20Viðskiptamarkmið,%20sýn%20og%20umfang.html), kennsluefni 6.1 og [endurgjöf úr yfirferð verkefnis 3](Heimildir/9.2%20Yfirferð%20á%20verkefni%203.html), sem eru varðveitt í Heimildir.

Tölulegir grunnar eru viðmið í COS-dæminu en ekki nýjar mælingar. Tillögur að mæliaðferðum og afmörkun MVP þarf að staðfesta með hagsmunaaðilum.

**Rekjanleiki:** Uppruni efnis, aðlaganir og viðbætur eru skráð í [REKJANLEIKI.md](REKJANLEIKI.md).

## Efnisyfirlit

1. [Viðskiptamarkmið](#1-viðskiptamarkmið)
2. [Framtíðarsýn](#2-framtíðarsýn)
3. [Prófíll lykilhagsmunaaðila eða mikilvægra notenda](#3-prófíll-lykilhagsmunaaðila-eða-mikilvægra-notenda)
4. [Forgangsröðun verkefnisins](#4-forgangsröðun-verkefnisins)
5. [Umfang fyrstu útgáfu (MVP)](#5-umfang-fyrstu-útgáfu-mvp)

## 1. Viðskiptamarkmið

Í COS-dæminu fara matarbirgðir til spillis og rekstraraðilinn hefur þörf fyrir að lækka kostnað. Símapantanir og handvirkt verklag takmarka yfirsýn starfsfólks mötuneytis yfir vænta eftirspurn. Starfsmenn fyrirtækisins verja jafnframt tíma í að panta, bíða og fara eftir mat. Forpantanir skapa tækifæri til að aðlaga framleiðslu að eftirspurn og afhending getur minnkað ferðir og bið. Þessi vandamál og tækifæri liggja að baki BO-1–BO-3 og byggja á greiningu verkefna 1 og 2.

### BO-1: Lækka hlutfall rýrnunar matarbirgða um 40% innan sex mánaða frá fyrstu útgáfu

| Atriði | Lýsing |
|---|---|
| Mælikvarði (Scale) | Verðmæti matarbirgða sem fara til spillis sem hlutfall af verðmæti innkeyptra matarbirgða á sama tímabili. |
| Mæliaðferð (Meter) | Starfsfólk mötuneytis skráir innkaup og birgðir sem það hendir í birgðakerfið. Fyrir fjórar vikur fyrir innleiðingu og fjórar vikur við lok sjötta mánaðar er hlutfallið reiknað sem 100 × samanlagt verðmæti skráðrar rýrnunar / samanlagt verðmæti innkaupa. Nota sömu verðmatsaðferð og sambærilegt þjónustumagn. Matarleifar á diskum teljast aðeins með ef þær eru skráðar með sama hætti í báðum mælingum. |
| Fyrri staða (Past) | 33% árið 2013 samkvæmt COS-dæminu í verkefni 1. Núverandi staða er ekki þekkt enn; mæla skal hana í fjórar vikur fyrir innleiðingu. |
| Markmið (Goal) | Undir 20% innan sex mánaða, sem jafngildir um 40% hlutfallslegri lækkun miðað við 33% upphafsgildi. Ef grunnmælingin breytist þarf að samræma tölulegt markmið henni. |
| Metnaðarmarkmið (Stretch) | Undir 15% á sama tímabili. |

Byggir á [BREQ-1 úr verkefni 1](https://github.com/Hvannberg/HBV301G-2026-COS/blob/main/SRS/business_requirements.md#breq-1). Forpantanir veita betri upplýsingar um eftirspurn. Í [árekstragreiningu verkefnis 2](https://github.com/Hvannberg/HBV301G-Verkefni2-lausn/blob/main/CONFLICTS.md#markmið-um-minni-matarsóun) kemur fram að árangur krefst einnig breytinga á verklagi og þátttöku neytenda. Kerfið eitt tryggir ekki þessa lækkun.

### BO-2: Lækka mánaðarlegan rekstrarkostnað mötuneytis um 15% innan tólf mánaða frá fyrstu útgáfu

| Atriði | Lýsing |
|---|---|
| Mælikvarði (Scale) | Rekstrarkostnaður í USD á mánuði við sambærilegan fjölda og samsetningu máltíða. Nær til launa, matar, rekstrarvara, viðhalds og húsnæðis, þar með talið rafmagns, vatns og hita. Kaup á varanlegum búnaði eru undanskilin. |
| Mæliaðferð (Meter) | Rekstraraðilinn tekur saman tilgreinda kostnaðarliði úr bókhaldi og fjölda afgreiddra máltíða. Bera saman meðal mánaðarkostnað síðustu þriggja mánaða fyrir innleiðingu og mánaða 10–12 eftir hana. Leiðrétta samanburð fyrir verðlagi, fjölda máltíða og samsetningu þjónustu. Rekstur COS sem fellur á mötuneytið telst með. |
| Fyrri staða (Past) | Til viðmiðunar í dæminu er gert ráð fyrir 10.000 USD á mánuði fyrir morgun- og hádegisverð fyrir 50 manns. Núverandi staða er ekki þekkt enn; afla skal gagna úr bókhaldi fyrir þrjá mánuði fyrir innleiðingu. |
| Markmið (Goal) | 15% lækkun innan tólf mánaða, eða 8.500 USD á mánuði miðað við viðmiðunargrunninn. |
| Metnaðarmarkmið (Stretch) | 20% lækkun, eða 8.000 USD á mánuði miðað við viðmiðunargrunninn. |

Markmiðið styður við þörf rekstraraðilans fyrir hagkvæmari nýtingu birgða og mannafla í verkefni 2. Minni rýrnun samkvæmt BO-1 er ein leið að árangrinum; ekki má tvítelja sama sparnað við mat á heildarávinningi.

### BO-3: Auka meðalraunvinnutíma starfsmanns sem notar mötuneytið um 15 mínútur á dag innan sex mánaða

| Atriði | Lýsing |
|---|---|
| Mælikvarði (Scale) | Meðalraunvinnutími í mínútum á starfsmann á vinnudegi hjá þeim sem nota mötuneytið. Reiknaður sem samtala skráðra vinnumínútna / fjöldi skráðra starfsmannsdaga. Tími við pöntun, bið og ferðir er mældur sérstaklega til að skýra framlag COS. |
| Mæliaðferð (Meter) | Tillaga: sama úrtak starfsmanna skráir tíma við vinnu, pöntun, bið, ferðir og hlé í tíu sambærilega vinnudaga fyrir innleiðingu og tíu daga við lok sjötta mánaðar. Starfsmenn og mannauðsdeild semja um flokkun tímans áður en mælt er. Reikna meðaltal yfir alla skráða starfsmannsdaga og nota samanteknar niðurstöður. Viðvera í Teams er ekki ein og sér mæling á raunvinnutíma. |
| Fyrri staða (Past) | Til viðmiðunar í dæminu er gert ráð fyrir 400 mínútum á dag. Núverandi staða er ekki þekkt enn; staðfesta skal hana með úrtaksmælingu fyrir innleiðingu. |
| Markmið (Goal) | Aukning um 15 mínútur á dag innan sex mánaða, eða 415 mínútur miðað við viðmiðunargrunninn. |
| Metnaðarmarkmið (Stretch) | Aukning um 20 mínútur á dag, eða 420 mínútur miðað við viðmiðunargrunninn. |

Byggir á [BREQ-2 úr verkefni 1](https://github.com/Hvannberg/HBV301G-2026-COS/blob/main/SRS/business_requirements.md#breq-2). Tímasparnaður við að sækja mat er ekki sjálfkrafa aukinn raunvinnutími. Í samræmi við [árekstragreiningu verkefnis 2](https://github.com/Hvannberg/HBV301G-Verkefni2-lausn/blob/main/CONFLICTS.md#afhending-matar-og-félagsleg-tengsl) er afhending valkostur og starfsmenn geta áfram sótt mat og borðað saman. Markmiðið gerir ekki ráð fyrir að stytta matarhlé.

## 2. Framtíðarsýn

Samanburðurinn hér miðast við símapantanir og handvirka afgreiðslu sem lýst er í F-1 úr verkefni 1. Staðfesta þarf núverandi verklag við raunverulega innleiðingu.

Fyrir starfsmenn fyrirtækisins sem vilja fá fjölbreyttar máltíðir með lítilli fyrirhöfn er COS vefkerfi sem gerir þeim kleift að skoða matseðla, panta og greiða fyrir mat og velja að sækja hann eða fá hann afhentan á vinnustaðnum. Starfsfólk mötuneytis fær yfirsýn yfir eftirspurn og pantanir til að skipuleggja framleiðslu og afhendingu betur, draga úr matarsóun og lækka rekstrarkostnað. Í stað símapantana og handvirkrar skráningar fá notendur sameiginlegt pöntunarferli og skýrar upplýsingar um verð og stöðu pöntunar. Til framtíðar getur COS einnig boðið pantanir frá nálægum veitingastöðum, endurteknar pantanir, hóppantanir og ítarlegri upplýsingar um máltíðir. Kerfið eykur þannig valfrelsi og sparar tíma um leið og starfsfólk heldur valinu um hvar það borðar.

## 3. Prófíll lykilhagsmunaaðila eða mikilvægra notenda

Valið byggir á [hagsmunaaðilagreiningu verkefnis 2](https://github.com/Hvannberg/HBV301G-Verkefni2-lausn/blob/main/STAKEHOLDERS.md). Hér eru dregin fram þau atriði sem ráða mestu um fyrstu útgáfu. Viðhorf og væntingar sem eru sett fram sem forsendur þarf að sannreyna með fulltrúum hópanna.

### Starfsmenn fyrirtækisins

**Val á notendahópi:** Starfsmenn leggja inn pantanirnar sem skapa eftirspurnargögn og tímasparnað. Ef notendum finnst erfitt að nota kerfið eða afhending er óáreiðanleg næst hvorki BO-1 né BO-3.

| Atriði | Lýsing |
|---|---|
| Notendahópur og hlutverk | Starfsmenn sem skoða matseðla, panta máltíðir og greiða fyrir þær. Þar á meðal eru vaktavinnustarfsmenn og persona Guðrún úr verkefni 2. |
| Helsta virði (Major value) | Minni fyrirhöfn við að panta mat, styttri bið eftir afgreiðslu með forpöntun og minni ferðatími þegar matur er afhentur; tengist tímasparnaði að baki BO-3. Aukinn raunvinnutími er ávinningur fyrirtækisins og felur ekki sjálfkrafa í sér ávinning starfsmanns. |
| Áhugi (Interest) | Mikill (++), samkvæmt mati í verkefni 2. Matið er áfram viðeigandi þar sem hópurinn notar pöntunarþjónustuna beint og verður fyrir áhrifum af verði, afgreiðslu og afhendingu. |
| Viðhorf (Attitudes) | Áhugi á þægilegri þjónustu, en félagslegt gildi heimsókna í mötuneytið getur haft áhrif á notkun. |
| Helstu áhugamál (Major interests) | Einföld pöntun, rétt gjaldfærsla, áreiðanleg afhending, viðráðanlegt verð og sýnileg staða pöntunar. |
| Takmarkanir (Constraints) | Þurfa vafra og viðurkennda auðkenningu. Þurfa að geta forpantað utan dagvinnutíma, en afhending er bundin við skilgreinda þjónustutíma. |

### Starfsfólk mötuneytis

**Val á notendahópi:** Þessi hópur birtir framboð og notar pantanir til að útbúa mat. Yfirsýn hans og breytt framleiðsluáætlun eru forsenda þess að BO-1 og BO-2 náist.

| Atriði | Lýsing |
|---|---|
| Notendahópur og hlutverk | Matráðar, kokkar og annað starfsfólk sem útbýr matseðla, undirbýr pantanir og afhendir mat til viðskiptavina eða sendla. |
| Helsta virði (Major value) | Forpantanir bæta áætlun um fjölda skammta og minnka handvirka skráningu og mistök. Styður BO-1 og BO-2, en kostnaðarlækkun felur ekki sjálfkrafa í sér betri starfskjör. |
| Áhugi (Interest) | Mikill (++), samkvæmt mati í verkefni 2. Matið helst þar sem kerfið breytir daglegri vinnu hópsins við matseðla, framleiðsluáætlun og afgreiðslu. |
| Viðhorf (Attitudes) | Sér tækifæri til betri skipulagningar en hefur fyrirvara um raunhæfi sóunarmarkmiðsins. Forsenda til staðfestingar: hópurinn hefur einnig áhyggjur af áhrifum breytinganna á störf. |
| Helstu áhugamál (Major interests) | Skýr pöntunarlisti eftir réttum og afhendingartíma, uppfært framboð og einföld skráning á stöðu pöntunar. |
| Takmarkanir (Constraints) | Framleiðslugeta, birgðir og mönnun takmarka framboð. Gera þarf ráð fyrir þjálfun og viðmóti sem nýtist við álag í afgreiðslu. |

### Fyrirtækið sem rekur mötuneytið

**Val á lykilhagsmunaaðila:** Rekstraraðilinn er viðskiptavinur og eigandi BO-1 og BO-2. Hann þarf að meta hvort breytingar á verklagi og fjárfesting skili ávinningi og tryggja rekstrarforsendur MVP.

| Atriði | Lýsing |
|---|---|
| Notendahópur og hlutverk | Rekstrarstjórn mötuneytisins sem samþykkir innleiðingu og ber ábyrgð á rekstri og framleiðsluáætlun. |
| Helsta virði (Major value) | Minni rýrnun og lægri rekstrarkostnaður samkvæmt BO-1 og BO-2 með betri aðlögun framleiðslu að eftirspurn. |
| Áhugi (Interest) | Mikill (++), samkvæmt mati í verkefni 2. Matið helst þar sem rekstraraðilinn ber ábyrgð á BO-1 og BO-2 og þarf að meta ávinning innleiðingar. |
| Viðhorf (Attitudes) | Í verkefni 2 kemur fram vilji til að minnka sóun. Forsenda til staðfestingar: rekstraraðilinn styður innleiðingu ef mælingar sýna að ávinningur réttlæti þróunar- og rekstrarkostnað. |
| Helstu áhugamál (Major interests) | Áreiðanleg eftirspurnargögn, rekjanleg gjaldfærsla og mælanlegur sparnaður án skerðingar á þjónustu. |
| Takmarkanir (Constraints) | Árangursmat krefst aðgangs að birgða- og bókhaldsgögnum. Rekstur þjónustunnar krefst mönnunar og samráðs við mötuneyti og launadeild. Fjárheimildir hans eru ekki þekktar og þarf að staðfesta áður en kostnaður er samþykktur. |

Sendlar eru einnig nauðsynlegir beinir notendur MVP. Þörf þeirra fyrir lista með viðtakanda, stað og tíma kemur fram í verkefni 2 og er tekin inn í kafla 5. Launadeild þarf að staðfesta gjaldfærsluferlið áður en það er tekið í notkun.

## 4. Forgangsröðun verkefnisins

Flokkunin fylgir COS-dæminu sem kennt er í 6.1: ákveðnir eiginleikar fyrstu útgáfu þurfa allir að virka og tiltækur þróunarmannafli stýrir áætluninni. Hún lýsir þróunarverkefninu. Afhendingartími matar og mönnun mötuneytis eru rekstrarforsendur sem hafa áhrif á kröfur, en eru ekki þessar verkefnisvíddir.

| Vídd | Flokkun | Rökstuðningur |
|---|---|---|
| Eiginleikar | Takmörkun (Constraint) | Samþykkt kjarnavirkni í kafla 5.1 þarf öll að virka til að pöntun, afgreiðsla og gjaldfærsla myndi nothæfa heild og styðji BO-1–BO-3. Hún er lágmarksumfang útgáfunnar; viðbótareiginleikar geta beðið. |
| Gæði | Takmörkun (Constraint) | Auðkenning, vernd upplýsinga, rétt gjaldfærsla og skýrt pöntunarferli þurfa að standast lágmarkskröfur. QA-2 úr V1 setur 95% árangur nýrra notenda í fyrstu tilraun. Mistök og óáreiðanlegar pantanir grafa undan viðskiptamarkmiðum. |
| Tímasetningar | Frígráða (Degree of freedom) | Í COS-dæminu er svigrúm í afhendingu hugbúnaðarins. Dagsetning er aðlöguð að tiltækum þróunarmannafla og tíma til sannprófunar. Enginn fastur afhendingardagur hefur verið tilgreindur; tímamörk BO teljast frá fyrstu útgáfu. |
| Kostnaður | Frígráða (Degree of freedom) | Í COS-dæminu er svigrúm í kostnaði. Enginn hámarksfjárhagsrammi hefur verið staðfestur. Semja þarf við kostunaraðila um þróunar- og rekstrarkostnað með hliðsjón af væntum sparnaði í BO-2; frígráða felur ekki í sér ótakmarkað fé. |
| Mannafli | Drifkraftur (Driver) | Tiltækur þróunarmannafli stýrir áætlun COS samkvæmt dæminu í 6.1. Verkaskipting og afhendingaráætlun eru mótuð út frá honum. Fjöldi þróunaraðila og aðgengi að sérfræðiþekkingu þarf að staðfesta; fjöldi sendla rökstyður ekki þessa flokkun. |

Ef tiltækur þróunarmannafli nær ekki að ljúka kjarnavirkninni með lágmarksgæðum á áætluðum tíma er afhendingardagur endurskoðaður og kostnaður ræddur við kostunaraðila. Ekki er sleppt nauðsynlegum hluta pöntunarferlisins eða slakað á lágmarksgæðum til að halda óstaðfestri dagsetningu. Viðbótareiginleikar í kafla 5.3 koma ekki í fyrstu útgáfu.

## 5. Umfang fyrstu útgáfu (MVP)

### 5.1 Umfang fyrstu útgáfu (MVP)

Fyrsta útgáfa þjónar starfsmönnum hjá einu fyrirtæki og pantanir koma úr hádegismatseðli eigin mötuneytis. Starfsmaður getur forpantað eða pantað samdægurs eftir framboði, sótt mat eða valið tiltækan afhendingarglugga á þjónustusvæði fyrirtækisins. Greitt er með frádrætti frá launum. Starfsfólk mötuneytis og sendlar fá þær upplýsingar sem þarf til að ljúka afgreiðslunni.

| Hvað þarf að vera í MVP? | Hvers vegna? | Tengsl við fyrri verkefni, ef við á |
|---|---|---|
| Búa til og birta hádegismatseðil með réttum, verði og framboði. Nauðsynlegar leiðréttingar þurfa að vera mögulegar. | Starfsmenn vita hvað er í boði og mötuneytið ræður við eftirspurnina. BO-1 og BO-2. | F-2 úr V1; lágmarksleiðréttingar eru ný tillaga að umfangi MVP. |
| Velja rétti og magn, sjá heildarverð og staðfesta einstaklingspöntun. | Kemur í stað símtals eða biðar og skapar eftirspurnargögn. BO-1 og BO-3. | F-1, FR-1 og FR-3 úr V1. |
| Velja að sækja mat eða afhendingu á tilteknum stað og í tiltækum 15 mínútna glugga. | Sparar ferðatíma og heldur valinu um að fara í mötuneytið. BO-3. | F-1, FR-2 og BRG-2 úr V1; félagsleg tengsl í verkefni 2. |
| Breyta eða hætta við pöntun áður en hún er útbúin; loka fyrir þær aðgerðir eftir það. | Heldur eftirspurnargögnum réttum og minnkar ósamræmi í afgreiðslu. BO-1. | FR-4–FR-6 úr V1. |
| Skoða eigin pöntun og stöðu hennar; starfsfólk mötuneytis skráir framvindu afgreiðslu. | Notandi veit hvort pöntun hefur borist og starfsfólk hefur sameiginlega yfirsýn. BO-3. | Þörf starfsmanna úr verkefni 2; stöður nefndar í FR-6 úr V1. Útfærsla þarf nánari kröfur. |
| Pöntunarlisti fyrir mötuneyti eftir réttum og afhendingartíma; sendlar sjá viðtakanda, stað og tíma á sínu svæði og skrá afhendingu. | Forpantanir nýtast í framleiðslu og afhending verður framkvæmanleg. BO-1–BO-3. | Þarfir starfsfólks mötuneytis og sendla úr verkefni 2; bæta þarf við virknikröfum. |
| Reikna verð og senda kostnaðarfærslur til launakerfis með rekjanlegri leiðréttingu þegar við á. | Full þjónusta þarf rétta greiðslu og leið til að leysa úr röngum færslum. | F-1 og BRG-1 úr V1; þarfir launadeildar úr verkefni 2. Staðfesta þarf snið og tímasetningu færslna. |
| Vefaðgangur af innra neti og Interneti; hægt að leggja inn pantanir allan sólarhringinn fyrir skilgreinda þjónustutíma. | Vaktavinnustarfsmenn geta forpantað. BO-3. | F-3 úr V1; úrlausn um aðgengi utan afhendingartíma úr verkefni 2. |
| Auðkenning fyrir pöntun, aðgangur eftir hlutverki og dulkóðaðar netsendingar með fjárhags- og persónuupplýsingum samkvæmt QA-1. | Verndar upplýsingar og kemur í veg fyrir að notandi gjaldfæri á annan. | QA-1 úr V1; þarfir öryggisstjóra úr verkefni 2. |
| Að minnsta kosti 95% nýrra notenda geti pantað án villna í fyrstu tilraun í notendaprófun. Staðfest pöntun varðveitist og endurtekin staðfesting valdi ekki tvöfaldri pöntun eða gjaldfærslu. | Einfaldleiki og áreiðanleiki eru forsenda notkunar og tímasparnaðar. BO-3. | QA-2 úr V1; varðveisla og vörn gegn tvískráningu eru nýjar tillögur að lágmarksgæðum. |

### 5.2 Rökstuðningur fyrir vali í fyrstu útgáfu

MVP nær yfir heila þjónustu: starfsmaður pantar, mötuneytið útbýr, matur er sóttur eða afhentur og rétt greiðsla skráist. Matseðill og pöntunarform ein og sér nægja ekki. Pöntunarlistar gera forpantanir að framleiðsluupplýsingum fyrir BO-1 og BO-2; afhending og auðveld notkun styðja BO-3.

Samkvæmt kafla 4 eru samþykkt kjarnavirkni og lágmarksgæði takmarkanir, en tiltækur þróunarmannafli stýrir áætluninni. Umfangið er því afmarkað við hádegismat úr eigin mötuneyti og eina greiðsluleið áður en það er samþykkt. Launadeild þarf að staðfesta færsluferlið áður en opnað er fyrir gjaldfærðar pantanir. Afhending krefst einnig mönnunar og þjónustugetu; listi í kerfinu kemur ekki í stað sendils.

Útgáfan gerir kleift að kanna hvort starfsfólk notar þjónustuna, hvort afgreiðsla gengur frá upphafi til enda og hvort eftirspurnargögn nýtast til að minnka sóun. Grunnmælingar samkvæmt kafla 1 þurfa að fara fram áður en árangur er metinn. Viðbrögð lykilnotenda og niðurstöður mælinga ráða næstu útvíkkun.

### 5.3 Hvað bíður síðari útgáfu?

| Eiginleiki | Ástæða þess að hann getur beðið |
|---|---|
| Pantanir frá nálægum veitingastöðum. | Krefjast samninga og nýrra afhendingar- og greiðsluferla. Eigin mötuneyti nægir til að prófa kjarnavirðið. Styður framtíðarsýnina um aukið úrval. |
| Áskriftir, endurteknar pantanir og hóppantanir. | Einstaklingspantanir nægja í fyrstu. Þessir eiginleikar úr framtíðarsýninni flækja breytingar, afpantanir og gjaldfærslu og geta því beðið. |
| Debet- og kreditkortagreiðslur. | Launafrádráttur veitir eina heila greiðsluleið. Fleiri leiðir kalla á viðbótarsamþættingu. |
| Morgun- og kvöldmatur. | Hádegismatur nægir til fyrstu innleiðingar; lengri þjónustutími krefst mats á mönnun og eftirspurn. |
| Ítarlegar hráefna- og næringarupplýsingar. | Bætir upplýsingar sem notendur geta byggt val sitt á en er ekki forsenda almennrar pöntunarleiðar. Gert er ráð fyrir að núverandi leið til að fá nauðsynlegar upplýsingar um mat haldist aðgengileg. |
| Full matseðlasaga, eyðing og vistun eldri matseðla í safn. | Birting og nauðsynlegar leiðréttingar duga fyrir daglegan rekstur MVP. |
| Sérstök símaforrit og kiosk með sérstakri auðkenningu. | Vefaðgangur nægir í fyrsta áfanga. Kiosk þarf sérstaka lausn fyrir örugga innskráningu og útskráningu samkvæmt verkefni 2. |

### 5.4 Takmarkanir og útilokanir

COS er pöntunar- og afgreiðslukerfi fyrir starfsmenn fyrirtækisins. Almenn sala til fólks utan fyrirtækisins og afhending utan skilgreinds þjónustusvæðis eru ekki hluti af fyrirhugaðri vöru. Þessi afmörkun er tillaga í drögunum og þarf staðfestingu rekstraraðila.

COS kemur ekki í stað birgðakerfis, bókhalds eða launakerfis. Það miðlar gögnum vegna pantana og gjaldfærslu, en launaútreikningur og heildstæð innkaupa- og birgðastýring eru utan vörunnar. Kerfið afhendir ekki mat sjálft. Aðgengi að pöntunum allan sólarhringinn felur ekki í sér afhendingar allan sólarhringinn.
