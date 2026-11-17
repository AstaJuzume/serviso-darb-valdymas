# Serviso darbų valdymo prototipas

Nuasmenintas, lietuviškas automobilių remonto užsakymų demonstracinis prototipas pagal pateikto komercinio pasiūlymo funkcinę apimtį. Naudojami tik sugalvoti kontaktai ir įrašai.

## Funkcionalumas

- Klientų, automobilių ir remonto užsakymų kortelių kūrimas, redagavimas ir paieška.
- Nauja užklausa nereikalauja iš anksto sukurtos kliento ar automobilio kortelės: kontaktas ir automobilio duomenys įvedami užklausoje, gali būti patikslinami vėliau; taip pat galima pasirinkti esamą klientą. Kortelės susiejamos užklausą paverčiant remonto užsakymu.
- Rankinis pirminių užklausų registravimas, gavimo šaltinis, vadybininkas, kitas veiksmas ir data; pavertimas užsakymu arba uždarymas su priežastimi.
- Draudikas, draudimo rūšis, žalos numeris, atvykimas, terminas ir Audatex nuoroda.
- Užsakymų Kanban lenta ir sąrašas, būsenos, filtrai, vėlavimo ir dėmesio žymos, laukimo priežastys ir subrangovas su komentaru.
- Du PDF dokumentai iš esamų duomenų: kliento užsakymas ir vidinis darbų lapas; lietuviški rašmenys išlaikomi atvaizduojant dokumentą.
- Individualus darbų sąrašas, vykdymo seka, meistras, data ir prioritetas; kito etapo paruošimas baigus ankstesnį.
- Darbuotojo sąsaja telefonui: tik pasirinkto demonstracinio darbuotojo priskirti darbai, priėmimas, užbaigimas, komentarai ir nuotraukos.
- Papildomi darbai su aprašymu ir nuotraukomis, vadybininko patvirtinimas ar atmetimas, derinimo poreikis ir patvirtinto darbo įtraukimas į planą.
- Kokybės patikra užbaigus visus darbus; patvirtinimas arba grąžinimas taisyti; vadybininko automobilio perdavimas klientui ir užsakymo uždarymas.
- Keturios fiksuotos rolių peržiūros; naudotojų kūrimas, redagavimas ir aktyvumo nustatymas.
- Užsakymų kiekiai pagal būseną, vadybininką, darbuotoją ir draudiką, vėluojantys ir laukiantys užsakymai, užklausų šaltiniai ir uždarymo priežastys.

## Demonstracijos ribos

Tai naršyklėje veikiantis demonstracinis prototipas, ne produkcinė .NET / React / SQL / Azure sistema. Duomenys ir sumažintos nuotraukos saugomi tik konkrečios naršyklės localStorage. Vaidmenų perjungimas demonstruoja sąsajos scenarijus; tikrasis Azure AD prisijungimas ir serverio prieigų tikrinimas neįjungti. Dokumentai naudoja du pavyzdinius šablonus. Klientų ir draudikų derinimas vyksta už sistemos ribų. Audatex yra tik vartotojo įvedama nuoroda.

Pagal pasiūlymą nėra išorinių API integracijų, automatinių laiškų, SMS, laiko sekimo ar pauzių, užimtumo kalendoriaus, apkrovų skaičiavimo, sąskaitų, sandėlio, pelningumo, elektroninio pasirašymo ar klientų portalo.

## Paleidimas

Statinis turinys pateiktas pagrindiniame kataloge, papildomo surinkimo nereikia. Atidarykite index.html arba paleiskite statinių failų serverį. PDF eksportas naudoja vietinę pdf-lib kopiją, jos licencija pateikta PDF-LIB-LICENSE.md.

## Patikrinimai

Naršyklėje patikrinti užklausos pavertimas užsakymu, užsakymo kortelė, PDF atsisiuntimas, keturios vaidmenų peržiūros, darbo priėmimas ir užbaigimas, kito darbo parengimas, kokybės patvirtinimas, papildomo darbo patvirtinimas ir įtraukimas į planą. Atskirai patikrinta JavaScript sintaksė ir pagrindinė darbų sekos bei proceso užtvarų logika.
