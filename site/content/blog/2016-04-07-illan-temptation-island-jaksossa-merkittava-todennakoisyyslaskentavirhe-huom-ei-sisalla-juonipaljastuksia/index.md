---
title: "Illan Temptation Island -jaksossa merkittävä todennäköisyyslaskentavirhe - HUOM: Ei sisällä juonipaljastuksia"
date: "2016-04-07"
author: "Aapeli Nevala"
---

Temptation Islandin kakkoskauden jaksossa kuusi nähdään keskeinen todennäköisyyslaskentavirhe. Jakso näytetään Nelosella tänään illalla, mutta se on ollut katsottavissa Ruutu+-palvelussa eilisestä asti.

Sarjassa neljä pariskuntaa lähetetään Thaimaahan kahdelle "leirille". Toisessa leirissä 10 sinkkumiestä yrittää iskeä varattuja naisia, toisessa 10 sinkkunaista varattuja miehiä. Nelonen näyttää sarjaa joka viikko kaksi jaksoa, joista toisessa nähdään jaksoparin huipennus "iltanuotio".

Iltanuotiolla pariskunnat katsovat leireihin asennettujen kameroiden kuvaamaa videomateriaalia oman puolisonsa humalaisesta sekoilusta intohimoisten, runsaasti tatuoitujen sinkkujen keskellä. Ensimmäisenä nuotiolle saapuva sukupuoli saakin päättää, näkeekö parin toinen puoli ollenkaan videota.

Kutosjaksossa ensimmäisenä iltanuotiolle saapuvat miehet. Siis jos mies haluaa katsoa videon, myös nainen iltanuotiolla näkee videon. Jos mies päättää, ettei videota katsota, nainenkaan ei näe videota.

Todennäköisyyslaskentavirhe liittyy nimenomaan iltanuotioon.

<!-- \[caption id="" align="alignnone" width="346"\]![](http://www.nelonenmedia.fi/wp-content/uploads/2015/01/Temptation_Island_Suomi_Kausi_1_Promo_Sami_Kuronen_01_Kuvaaja_Toni_Tuominen.jpg) Sami Kuronen. Kuva: Toni Tuominen\[/caption\] -->

Ohjelman juontaja **Sami Kuronen** sanoo naisille: "osa katsoo tänään videon, ja osa ei". Tämä tarkoittaa, että "ainakin yksi näkee" ja "ainakin yksi ei näe".

Neljästä naisesta kaksi ensimmäistä saavat katsoa videon. Virhe tulee, kun Kuronen toteaa nuotiolla kolmantena istuvalle **Iidalle**, että "Iida, sulla on 50-50 mahdollisuus".

Tämä ei pidä paikkaansa.

Merkitään N="näkee" ja E="ei näe". Nyt mahdollisia "näkemiskombinaatioita" on $2^4 = 16$: {NNNN, NNNE, NNEN, NENN, ENNN, NNEE, NENE, ENNE, ENEN, EENN, NEEN, EEEN, EENE, ENEE, NEEE ja EEEE}.

Merkitään A = "Kolmantena vuorossa oleva Iida näkee" ja B="kaksi on jo nähnyt". Tällöin saadaan ehdollinen todennäköisyys $P(A|B)$. Koska voimme rajoittua vaihtoehtoihin, joissa kaksi ensimmäistä ovat nähneet videon, jää jäljelle joukko {NNNN, NNNE, NNEN, NNEE}. Lisäksi tapahtuma NNNN voidaan sulkea pois, sillä tiedetään, että osa ei näe videota.

Jäljelle jää siis vain {NNNE, NNEN, NNEE}. Näistä sarjoista vain yhdessä Iida näkee videon, siis todellisuudessa mahdollisuus ei ole "50-50", vaan pikemminkin "33-67", eli $P(A|B) = \frac{1}{3}$.

Juonipaljastusten minimoimiseksi Tyyppiarvon viihdetoimitus ei kerro, saiko Iida lopulta katsoa videon.

50-50-mahdollisuus onkin kuin suoraan klassisesta vitsistä: "Missiltä kysyttiin, millä todennäköisyydellä voittaa lotossa. Hän vastasi: "50%, joko voittaa tai ei voita!"
