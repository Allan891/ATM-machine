# ATM-machine
ATM machine code in Prolog

Kortfattad om mig.

Civilingenjörsstudent i Informationsteknik vid KTH med bakgrund som elmontör, gruppledare och trafikledare. Då, smalat jag erfarenhet av kundbemötande, ledarskap och teamarbete. Jag är noggrann, ansvarstagande och trivs i sociala och serviceinriktade. Engagerad, analytisk och gillar utmaningar. Språk förmågan, kan jag båda svenska och engelska, både i tal och skrift.

DD1351 Logik för dataloger.

Modellprovning för CTL.

Huvudsyftet är att utforska (modellkontroll) tekniker för computational tree logic (CTL), och implementera ett bevissystem skräddarsytt för CTL-formler. Modellkontroll används för verifiering av CTL-formler och implementeras här rekursivt samtidigt som man tar med de utmaningar som loopar i modellen utgör, vilket är avgörande för att säkerställa avslutning. Jag hade tre steg för att bygga vår modell. Förstå systemet, implementera systemet och validera dess funktionalitet genom olika scenarier. I början testade jag det enklaste möjliga fallet genom att implementera de bokstavliga och kontrollera om en given start noden hade en specifik egenskap eller inte. Steg två var att implementera varje efterföljande regel och testa dem separat i olika scenarier genom att skriva enkla modeller och påståenden. Det sista steget i utvecklingen av modellkontrollen var att testa med mer komplicerade nästed flera regler och körde igenom den medföljande testen. Jag gjorde en kopia av vår modellcheckare som skulle skriva ut varje regel som modellen bedömde vara sant när ett påstående testades och använde det om programmet gav ett felaktigt svar eller frös på en testfil för att isolera problemet. Sedan jag uppdaterade lösningen genom olika liknande scenarier.

Modell

Min modell består av 12 tillstånd. Den representerar en förenklad version av en bankomat. Tillstånden och fastigheterna är namngivna på ett sätt som gör dem ganska självförklarande. Kortfattat visar modellen de olika tillstånden för att komma åt ett konto och antingen visa kontosaldot eller ta ut pengar. Det tar också hänsyn till möjligheten att uttaget nekas samt att det finns en gren för att visa de olika tillstånden och möjliga övergångar i händelse av att en felaktig pinkod skrivs in.
