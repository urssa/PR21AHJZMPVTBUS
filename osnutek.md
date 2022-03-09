# Prometne nesreče v Sloveniji

## Opis problema

Osrednji problem seminarske naloge je analiza dejavnikov oz. okoliščin za nastanek prometnih nesreč ter udeležencev v le-teh.

Glavni cilji oz. ugotovitve bodo zajemali:
1. Pogostost pojavitve prometnih nesreč po posameznih krajih in mesecih
2. Relacija med okoliščinami prometne nesreče in stopnjo poškodb udeležencev
3. Razmere ob katerih največkrat pride do prometne nesreče
4. Profil voznikov povzročiteljev prometnih nesreč

## Opis podatkov in vir

Podatke, ki jih bomo uporabili za reševanja problema so podatki o prometnih nesrečah od leta 1995 dalje, ki jih lahko najdemo na spletni strani Slovenske policije.

Uporabili bomo podatke za leto 2019, ki se nahajajo na spodnji povezavi:

https://podatki.gov.si/dataset/mnzpprometne-nesrece-od-leta-2009-dalje/resource/77b5484b-ed7e-48de-abf8-6bd2b35a218f

Na navedeni spletni strani smo našli povezavo do spletne strani policije, ki deli statistiko o različnih dolžnosti policije (npr. število zaposlenih, prejeti klici na policijo, prometna varnost, itd.).

Povezava do strani z omenjenimi podatki:

https://www.policija.si/o-slovenski-policiji/statistika/prometna-varnost

Podatki so tabelarične oblike, shranjeni v ločenih csv datotekah, ki se nahajajo v zip arhivih. Vsak zip arhiv je poimenovan oz. označen z letom iz katerega so podatki. Zaradi velike količine podatkov se bomo prvotno osredotočili le na leto 2019, kasneje pa dodali še primerjave iz prejšnjih let v kolikor bodo te relevantne. 

V vsaki csv datoteki je približno od 20000 do 31000 primerov in 35 atributov, enoličnih primerov nesreč pa je od 12000 do 20000.

Podatki so sestavljeni iz sledečih atributov:

1.	številka za štetje in ločevanje posamezne prometne nesreče
2.	klasifikacija nesreče glede na posledice (Izračuna se avtomatično glede na najhujšo posledico pri udeležencih v prometni nesreči)
3.	upravna enota, na območju katere se je zgodila prometna nesreča
4.	datum nesreče (format: dd.mm.llll) 
5.	ura nesreče (format: hh.mm) 
6.	indikator ali se je nesreča zgodila v naselju (D) ali izven (N)
7.	lokacija nesreče
8.	vrsta ceste ali naselja na kateri je prišlo do nesreče
9.	oznaka ceste ali šifra naselja kjer je prišlo do nesreče
10.	tekst ceste ali naselja, kjer je prišlo do nesreče
11.	oznaka odseka ceste ali šifra ulice, kjer je prišlo do nesreče
12.	tekst odseka ali ulice, kjer je prišlo do nesreče
13.	točna stacionaža ali hišna številka, kjer je prišlo do nesreče
14.	opis prizorišča nesreče
15.	glavni vzrok nesreče
16.	tip nesreče
17.	vremenske okoliščine v času nesreče
18.	stanje prometa v času nesreče
19.	stanje vozišča v času nesreče
20.	stanje površine vozišča v času nesreče
21.	Geo Koordinata X (Gauß-Krüger-jev koordinatni sistem)
22.	Geo Koordinata Y (Gauß-Krüger-jev koordinatni sistem)
23.	številka za štetje in ločevanje oseb, udeleženih v prometnih nesrečah
24.	kot kaj nastopa oseba v prometni nesreči
25.	starost osebe (LL)
26.	spol
27.	upravna enota stalnega prebivališča
28.	državljanstvo osebe
29.	poškodba osebe
30.	vrsta udeleženca v prometu
31.	ali je oseba uporabljala varnostni pas ali čelado (polje se interpretira v odvisnosti od vrste udeleženca) (Da/Ne)
32.	vozniški staž osebe za kategorijo, ki jo potrebuje glede na vrsto udeleženca v prometu (LL)
33.	vozniški staž osebe za kategorijo, ki jo potrebuje glede na vrsto udeleženca v prometu (MM)
34.	vrednost alkotesta za osebo, če je bil opravljen (n.nn v enoti mg alkohola/liter izdihanega zraka (mg/l))
35.	vrednost strokovnega pregleda za osebo, če je bil odrejen in so rezultati že znani (n.nn v enoti g alkohola/kg krvi (g/kg))
