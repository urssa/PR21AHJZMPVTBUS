# Vmesno poročilo o Prometnih nesrečah v Sloveniji

## Opis problema

Osrednji problem seminarske naloge je analiza dejavnikov oz. okoliščin za nastanek prometnih nesreč ter udeležencev v le-teh.
Za vmesno poročilo smo izvedli analizo za sledeči dve vprašanji:

-	Razmere ob katerih največkrat pride do prometnih nesreč

-	Profil voznika povzročiteljev prometnih nesreč

Na predlog profesorja smo dodali še analize podatkov iz naslednjega leta ( 2020 ) na prej navedeni vprašanji.
Za končno poročilo nam tako ostane še, da odgovorimo na naslednji dve vprašanji:

-	Pogoste pojavitve prometnih nesreč po posameznih krajih in mesecih

-	Relacije med okoliščinami prometne nesreče in stopnjo poškodb udeležencev

## Opis podatkov in vir

Podatke, ki smo jih uporabili za reševanja problema so podatki o prometnih nesrečah od leta 1995 dalje, ki jih lahko najdemo na spletni strani Slovenske policije.

Uporabili smo podatke za leto 2019 in leta 2020 ki se nahajajo na spodnji povezavi:

https://podatki.gov.si/dataset/mnzpprometne-nesrece-od-leta-2009-dalje/resource/77b5484b-ed7e-48de-abf8-6bd2b35a218f

Na navedeni spletni strani smo našli povezavo do spletne strani policije, ki deli statistiko po različnih dolžnosti policije (npr. število zaposlenih, prejeti klici na policijo, prometna varnost, itd.).

Povezava do strani z omenjenimi podatki:

https://www.policija.si/o-slovenski-policiji/statistika/prometna-varnost

Podatki so tabelarične oblike, shranjeni v ločenih csv datotekah, ki se nahajajo v zip arhivih. Vsak zip arhiv je poimenovan oz. označen z letom iz katerega so podatki. Zaradi velike količine podatkov se bomo prvotno smo se osredotočili le na leto 2019 pozneje smo na predlog profesorja dodali še analizo iz leta 2020 ter primerjali njune rezultate. 

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

## Opis in ugotovitve analize ciljev/vprašanj

### Razmere ob katerih največkrat pride do prometnih nesreč
#### Ugotovitve

Za analizo okoliščin smo najprej pregledali katere vrednosti v posameznih atributih imajo največje pojavitve prometnih nesreč. 
Ugotovili smo sledeče:

  -	Stanje ceste na kateri se zgodi največ prometnih nesreč je suhe, nato mokre in na zadnjem mestu so spolzke. Izkaže se tudi, da  so ne splužene ceste večkrat vzrok nesreče kot splužene isto velja tudi za ne posoljene ceste. Rezultati so bili isti za leto 2020.

  -	Največ prometnih nesreč se zgodi v mestih oz. v naseljih z uličnim sistemom, nato v manjših vaseh oz. naseljih brez uličnega sistema ter na avtocestah. Podobne rezultate smo dobili za leto 2020.

  -	Vrsta odseka na kateri se zgodi prometna nesreča je bila navadna cesta, nato je sledilo parkirišče in na tretjem mestu so  križišča.  Leta 2020 so rezultati podobni.

  -	Naša analiza je zajela tudi v katerih letnih časih se zgodi največ prometnih nesreč. Izkazalo se je, da je bilo v letu 2019 največ prometnih nesreč jeseni in poleti, med tem ko leta 2020, je bilo ponovno poleti največ prometnih nesreč, zima in jesen pa sta bile izenačene. Iz tega lahko sklepamo, da je v poletju večja verjetnost, da pride do prometne nesreče.

  -	Zanimalo nas je tudi ob katerih urah se zgodi največ prometnih nesreč. Izkazalo se je, da se je leta 2019 in 2020 zgodilo največ prometnih nesreč med 14 in 15 uro. To je lahko razvidno iz spodnjega grafa.
  
  ![slika](https://user-images.githubusercontent.com/68822429/163239423-a7bc5f07-234d-4ee6-9e66-9d91f9e826b6.png)

  
### Profil voznikov povzročiteljev prometnih nesreč
#### Ugotovitve

- Ugotovili smo, da moški povzročajo več prometnih nesreč kot ženske. Enak rezultat je bil  tudi za leto 2020. Prav tako smo ugotovili tudi, da je večna udeležencev v  prometnih nesrečah moških. To lahko razberemo iz spodnjega grafa.

![slika](https://user-images.githubusercontent.com/68822429/163240224-508e54ff-0a13-481a-9c09-ddb98502dcd5.png)


- Ugotovili smo , da so največkrat povzročitelji stari med 20 in 40 let, podoben rezultat smo dobili tudi za leto 2020.  
Presenetljiv rezultat, ki smo ga opazili je , da večina povzročiteljev prometnih nesreč ni bila pod vplivom alkohola. Ugotovili smo, da je število povzročiteljev prometnih nesreč, ki so pod vplivom alkohola bistveno večje med 15 in 20 uro. Podobne rezultate smo dobili za leto 2020. To je lahko razvidno iz spodnjega grafa.

![slika](https://user-images.githubusercontent.com/68822429/163239869-e8bb5ea1-5891-4209-bd11-29551b812f2b.png)


- Analizirali smo tudi leta in mesece izkušenj, ki jih je imel povzročitelj nesreče. Vendar so bili tu podatki nepopolni oz. podatka nismo imeli za vse voznike. Zato smo pri tistih kjer ni bilo podatka, predvidevali izkušnje glede na starost.  Rezultati, ki smo jih pridobili so da največ prometnih nesreč povzročijo vozniki, ki imajo od 0 do 10 let izkušenj. Izkazalo se je tudi, da več kot ima nekdo izkušenj manjša je verjetnost, da bo tak voznik povzročil prometno nesrečo. Enako je bilo za 2020.

- Izvedli smo tudi pregled ali so povzročitelji prometnih nesreč večinoma Slovenci ali  tujci. Kot je bilo pričakovano se je izkazalo, da največ prometnih nesreč povzročijo Slovenci. Tudi v letu 2020 je bilo enako.

Iz zgornjih ugotovitev lahko sklepamo, da največ prometnih nesreč povzročijo v povprečju moški vozniki, ki so stari med 20 in 40 let, so Slovenci in imajo samo nekaj letne izkušnje. Tako smo dobili odgovor na naše vprašanje kakšen profil imajo povzročitelji prometnih nesreč.
