---
layout: post
title:  "Tehtävään vastaaminen GitHubissa"
---

Tehtävät julkaistaan GitHub Classroom -ympäristössä ja niihin vastaaminen tapahtuu perinteisen GitHub-työkulun mukaisesti. 
Vastaaminen koostuu seuraavista vaiheista:
 * käyttöoikeuden myöntäminen GitHubille
 * tehtävän vastaanottaminen
 * tehtävän kopioiminen omalle koneelle (clone)
 * tehtävän avaaminen Visual Studio Codessa
 * muutosten tekeminen ja tallentaminen 
 * ohjelman suorittaminen
 * testaaminen testausskriptillä
 * muutosten vieminen paikalliseen repoon (commit)
 * tehtävän palautus GitHubiin (push)

## Käyttöoikeuden myöntäminen GitHubille

Ensimmäiseksi tehtävä täytyy vastaanottaa. Tämä tapahtuu klikkaamalla moodlen sivuilla olevaa tehtävälinkkiä. Linkki vie sinut 
tehtävän sivuille GitHub Classroomiin, jossa vastaanotat tehtävän.

Jos olet tekemässä tätä ensimmäistä kertaa, GitHub haluaa varmistaa, että haluat antaa GitHub Classroom -sovellukselle oikeuden
käyttää omaa GitHub-tiliäsi. Kirjaudu sisälle GitHub-tunnuksillasi, anna oikeudet painamalla *Authorize GitHub*-nappia ja 
klikkaa tämän jälkeen listasta omaa nimeäsi. Sivusto varmistaa vielä, että klikkasit varmasti omaa nimeäsi. Hyväksy valinta klikkaamalla OK.

![Käyttöoikeuden antaminen GitHubille](/images/tehtavaan-vastaaminen-authorize.gif)

## Tehtävän vastaanottaminen

Hyväksy tehtävä klikkaamalla *Accept this assignment* -nappia ja odota, että palvelu saa kopioitua tehtävän tiedot sinulle luotuun uuteen repoon. Klikkaa luonnin jälkeen repositoryn linkkiä, niin pääset tehtävän projektisivulle.

![Tehtävän hyväksyminen](/images/tehtavaan-vastaaminen-accept.gif)

## Tehtävän kopioiminen omalle koneelle

Ennen tehtävän suorittamista se kopioidaan omalle koneelle. Tämä tapahtuu klikkaamalla projektisivulla vihreää Code-nappia ja klikkaamalla avautuvasta ikkunasta osoitteen kopioiminen työpöydälle-kuvaketta.

Valitse tämän jälkeen GitHub Desktop -sovelluksessa Clone a repository from the Internet -kohta, avaa URL-välilehti ja liitä kopioimasi osoite Repository URL -kenttään. Varmista, että Local path -kentässä on oikea kansio valittuna. 

Klikkaa Clone-nappia, jolloin tehtävän tiedot kopioidaan omalle koneellesi.

![Tehtävän kloonaaminen](/images/tehtavaan-vastaaminen-clone.gif)

## Tehtävän avaaminen Visual Studio Codessa

Seuraavaksi tehtäväkansio avataan Visual Studio Codessa valitsemalla File &gt; Open Folder... Avautuvaan ikkunaan valitaan se kansio, jonne tehtävämateriaalit edellisessä vaiheessa kopioitiin. Valittu kansio hyväksytään klikkaamalla Select Folder -nappia.

Tämän jälkeen vasemmassa reunassa olevasta tiedostonäkymästä avataan tehtava-kansiosta löytyvä tehtava.html -tiedosto.

![Tehtävän avaaminen](/images/tehtavaan-vastaaminen-open-folder.gif)

## Muutosten tekeminen ja tallentaminen

Lue tehtävätiedostossa olevat ohjeet ja kirjoita tämän jälkeen ohjetekstin alapuolelle teksti *Hei Koodaajaguru, nyt aloitetaan koodaaminen!*. 

Tallenna tekemäsi muutokset valitsemalla File &gt; Save. Voit tallentaa muutokset myös pikanäppäimellä Ctrl + S.

![Muutosten tekeminen ja tallennus](/images/tehtavaan-vastaaminen-edit-and-save.gif)

## Ohjelman suorittaminen

Koodin tehdyt muutokset kannattaa testata tasaisin väliajoin. Harvemmin virheellinen koodi korjaantuu myöhemmissä vaiheissa taianomaisesti, vaan virheen syy kannattaa selvittää välittömästi.

HTML-sivulla olevan koodin pystyy testaamaan avaamalla sivun webbiselaimessa. Helpoiten tämä onnistuu tuplaklikkaamalla tiedostokuvakkeen päällä, jolloin tiedosto avautuu selaimeen.

![Koodin suorittaminen](/images/tehtavaan-vastaaminen-execute.gif)

## Testaaminen testausskriptillä

Tehtäviin on sisällytetty myös testausskripti, jolla vastauksen oikeellisuuden pystyy varmistamaan.

Testausskripti suoritetaan valitsemalla Terminal &gt; New Terminal ja antamalla avautuvaan terminaali-ikkunaan komento *npm test*.

Jos ruudulle tulostuu vihreä passed-teksti, niin silloin tekemäsi muutokset läpäisivät testin. Tällöin voit palauttaa tehtäväsi vastauksen.

Jos ruudulle tulostui punainen failed -teksti, niin silloin koodissasi on jokin virhe ja se täytyy korjata.

![Koodin testaaminen](/images/tehtavaan-vastaaminen-test.gif)

## Muutosten vieminen paikalliseen repoon

Tehtävään tekemäsi muutokset täytyy viedä ensin paikallisessa projektikansiossa olevaan repoon ennen, kuin voit palauttaa tehtävän. Tätä toimipidettä kutsutaan commitiksi.

Aktivoi ensin versiohallintanäkymä Visual Studio Coden vasemman reunan palkista. Valitse tehtava.html -tiedoston oikealla puolella olevaa +-kuvaketta. Tämä merkitsee ko. tiedoston valituksi seuraavaan hyväksyntään (commitiin). Kirjoita tiedostoalueen yläpuolella olevaan tekstikenttään teksti *tehtävä suoritettu* ja klikkaa lopuksi commit-ikonia.

Tämän seurauksena tehtava.html-tiedostoon tekemäsi muutokset tallennettiin paikalliseen git-repoon niin sanottuna committina. Nyt tekemäsi muutokset ovat valmiina palautukseen.

![Muutosten vieminen](/images/tehtavaan-vastaaminen-commit.gif)

## Tehtävän palautus GitHubiin

Viimeisenä vaiheena on paikallisten muutosten vieminen GitHubissa olevaan repoon, jolloin vastaus näkyy myös opettajalle. Tämä tapahtuu valitsemalla ... &gt; pull, push &gt; push.

Voit tarkistaa palautuksen onnistumisen GitHubin projektisivulta. Sivulle pitäisi päivittyä commitissa antamasi tiedot sekä automaattitarkistuksen tulos. 

Commit-riville tulostuu vihreä väkänen, jos palauttamasi koodi on hyväksytty. Keltainen pallo merkitsee, että testiä ollaan vielä suorittamassa. Punainen ruksi puolestaan ilmoittaa, että koodi ei läpäissyt testiä.

![Tehtävän palautus](/images/tehtavaan-vastaaminen-push.gif)