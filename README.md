Web Pirátů
==========

Fáze marketingových úvah
------------------------

Základními dokumenty pro tvorbu webu jsou:
* [Pirátská identita](http://www.pirati.cz/rp/pid/start)
* [Grafický manuál](http://www.pirati.cz/rp/pid/gman/start) (může být upraven)
* [Pirátský klíč](http://www.pirati.cz/rp/pid/klic)

Jaké sociální skupiny web navštěvují, co na něm hledají a jaký chceme, aby si odnesly dojem?

1. **noví návštěvníci** chtějí zjistit, co to jsou ti Piráti, o kterých slyšeli;

   chceme, aby opustili mýty o Pirátské straně, brali nás jako otevřenou a poctivou stranu, která přináší nový vítr do politiky, zastupuje jejich zájmy a dělá ji zábavnější

   konverzní kritéria:
     - počet zobrazených stránek a doba strávená na webu,
     - like na facebooku a počet sdílení článků na facebooku,
     - přihlášení se k odběru newsletteru,
     - registrace příznivcem či podání přihlášky o členství

   skupina návštěvníků je primární skupinou mimo období voleb, dokud nebudou
   Piráti dostatečně známou politickou stranou

2. **příznivci** (a členové) hledají odpovědi na zajímavé otázky, na které narazili
   při diskusi se svými přáteli, hledají možnost jak se zapojit, podpořit naši činnost a stát se členy, příznivci také sledují stanoviska na webu k aktuálním otázkám, vidí zde kalendář celostátních akcí s pozvánkami;

   konverzní kritéria:
     - počet přihlášených dobrovolníků,
     - výše obdržených darů přes platební bránu,
     - navštívené akce,
     - přihláška na kandidátní listinu

   skupina příznivců bude primární skupinou mimo období voleb, jakmile budou
   Piráti dostatečně známou politickou stranou

3. **voliči** hledají informace pro srovnání s ostatními politickými stranami,
   zejména program pro dané volby, stručnou charakteristiku strany, vůči které
   by se mohli srovnávat, kandidáty, činnost a jiné důvody, proč
   Piráty volit či nevolit; skupina voličů se dále segmentuje na jednotlivé persony

   chceme, aby snadno našli pro ně nejdůležitější témata, aby se na základě
   prezentace rozhodli Piráty volit a viděli všechny prospěšné věci,
   které pro ně Piráti dělají (veřejně prospěšné projekty),
   zejména aby nás vnímali po právu jako úplně jinou stranu než ostatní
   politické strany;

   konverzní kritéria:
     - volební preference v průzkumech a ve volební kalkulačce,
     - počet hlasů ve volbách

   skupina voličů je primární skupinou v předvolební době

4. **novináři** a odborná veřejnost hledají oficiální stanoviska k zásadním politickým
   tématům a událostem a podkladové materiály, a dále objektivní údaje
   využitelné při politických srovnáních, případně informace o představiteli strany;

   chceme, aby odcházeli z našeho webu s dojmem přehlednosti, modernosti,
   aktuálnosti a profesionality a měli k Pirátům náklonnost, a dále aby
   informace předávali dále autentické a sympatizovali s Pirátským hnutím,
   které má nezávislost médií jako jeden ze svých cílů.

   konverzní kritéria:
     - počet pozitivních článků o Pirátech (včetně projektů),
     - žádosti médií o vyjádření,
     - ohlas na naše výstupy (témata)

4. **političtí oponenti** hledají možnosti, jak zkopírovat části Pirátského
   webu a využít je k vlastnímu prospěchu;

   chceme schopné lidi z jiných politických stran konvertovat nebo je aspoň
   přimět prosazovat naše principy v jejich stranách,

   konverzní kritéria:
     - počet citací Pirátského programu ostatními politiky
     - počet nových zájemců o členství z ostatních politických stran

Technické řešení
----------------

Z výše uvedených očekávání vyplývá následující vymezení webu:

Jednoduché a jasné internetové stránky, které
1. obsahují autoritativní (reprezentativní) informace, které veřejnost hledá,
2. jsou nepřetržitě rychle dostupná a
3. jsou hlavním kanálem pro oslovení širokých mas voličů.

Komentář: Web je tedy vymezen jako komunikační kanál navenek, neměl by obsahovat zbytečně podrobné informace jako jsou zápisy ze schůzí, které jsou ukládány jinde (např. na redmine nebo wiki). Web by měl mít jednoduchou strukturu. Cílem webu není poskytovat služby členům (uvnitř strany), ale naopak šířit

#### Jak zapadá web do ekosystému elektronických služeb?

Web není stavěn na to, aby plnil složité požadavky (sledování úkolů, projektové
řízení, sbírka předpisů, fórum). Tyto služby jsou vyvedeny do samostatných aplikací.
Celý seznam služeb je obsažen v [off-canvas liště](https://jsfiddle.net/hSu4c/305/).

### Principy fungování

1. Web je v celém svém fungování příkladem uplatňování politiky strany
   (citování autorů, github,     odpovědnost).
2. Web je časově neomezeně a rychle dostupný (statický web pomocí generátoru,
   jednoduché styly a skripty, minifikace) a zobrazování na všech zařízeních
   (responsive design).
3. Web není používán jako náhražka jiných webových aplikací strany.
4. Web je klonovatelný pomocí github a v případě likvidace serveru znovu nahoditelný.
5. Na web přispívají autorizované osoby, v každém kraji je vyškolen aspoň jeden správce.
6. Web dodržuje rozšířené konvence a standardy webdesignu.
7. Web je grafickým základem pro všechny ostatní webové aplikace strany
   (např. off-canvas lišta).
8. Každý informace je snadno dohledatelná do 3 kliků.

### Základní technické řešení

Web funguje na program jekyll a je zveřejněn pomocí github-pages. Upravovat
web může jakýkoliv uživatel githubu, slouží k tomu technologie prose.io.  


#### Jednotné služby

**Potřeby**:

* jednotná kategorizace v rámci hlavního webu a krajských webů (sitemap)
* vnitřní agregace článků podle tématu (např. zobraz články ze všech sdružení
  k dopravě, aby byly u programu s dopravou)
* decentralizované upravování webu,
* koncentrovaná správa více assets (např. layoutů, includes včetně jednotné
  grafiky)

**Řešení**:

Řešit integrací:

* [git submodules](https://help.github.com/articles/using-submodules-with-pages/)
* které jekyll [podporuje](http://git-scm.com/book/cs/v1/N%C3%A1stroje-syst%C3%A9mu-Git-Submoduly)

#### Typy obsahu

**Potřeby**:

* generovat seznamy článků podle tagů (např. články zastupitelského klubu),
* generovat kandidátní listiny,
* generovat články z médií o Pirátech k danému tématu,
* generovat seznamy funkcionářů,
* zobrazit kalendář a generovat seznamy akcí v dané lokalitě.

**Řešení**:

Obsah lze řešit pomocí různých typů pages, resp. collections a posts.
Tj. budeme mít např. následující typy:

* `person` (collection) - stránka nahrazující prezentace na wiki v oblasti /lide/, na které
  budou metadata jména, příjmení, jméno s tituly, datum narození, místo narození,
  souřadnice bydliště, fotografie standardizovaných rozměrů, telefon apod.,
  viz např. [zdroj](https://raw.githubusercontent.com/pirati-cz/webpraha/gh-pages/_posts/2014-09-25-mikulas-ferjencik.md)
  a [výstup](http://praha.pirati.cz/mikulas-ferjencik.html) (patička dole).

  **vazby**: seznam osob s určitou funkcí, kandidátní listiny

* `article` (posts) - stránka s článkem (např. tiskovou zprávou, stanoviskem nebo
  blogem), s tagy, titulkem, perexem, obrázkem a autorem, významností zprávy,
  viz na webu pražských Pirátů [zdroj](https://raw.githubusercontent.com/pirati-cz/webpraha/gh-pages/_posts/blog/2014-11-27-prvni-zasedani.md) a [výstup](http://praha.pirati.cz/prvni-zasedani.html),
  nebo táborských [zdroj](https://raw.githubusercontent.com/pirati-web/tabor.pirati.cz/gh-pages/_posts/2015-02-25-mistni-web.md)
  a [výstup](http://tabor.pirati.cz/clanky/2015/02/25/mistni-web/)

  **vazby**: seznam článků podle tagů, feed na titulní stránce nebo portálu

* `unit` (page) - podstránka organizační složky, zejména místního sdružení (portál),
  která obsahuje název sdružení, název
  nadřízeného sdružení, předsednictvo sdružení (členy orgánu), odkaz na fórum sdružení,
  variabilní symbol sdružení, odkaz na facebook sdružení, odkaz na fórum
  zájemců o členství apod., menu (může obsahovat např. položku volební program,
  zastupitelský klub nebo kandidátní listina), odkaz na redmine a další vazby
  na ostatní systémy strany

  **vazby**: mapa krajských a místních sdružení, domény krajských a místních
  sdružení třetího řádu

* `link` (post) - odkaz na článek o Pirátech, obsahuje odkaz samotný, jeho titulek,
  médium, perex, tagy, významnost zprávy

  **vazby**: feed na titulní stránce, na stránce zastupitelského klubu apod.

* `event` (collection) - událost související s Piráty (schůze sdružení, zasedání zastupitelstva,
  happening, vystoupení v médiích, setkání s občany (míting), demonstrace apod.),
  odkaz na potvrzení účastni na facebooku,

  **vazby**: feed na titulní stránce a na portálu, export do ical formátu
  s možností sledovat vybraný kalendář

Všechny stránky mohou obsahovat: menu (např. na portálech sdružení), odkaz na
facebook, obrázek, tagy apod., nicméně ty mohou být u různých typů obsahu
zobrazeny jinak.

Fáze testování
--------------

Schopnost plnit vytyčené úkoly je třeba od počátku testovat na normálních
lidech všech věkových a sociálních skupin, zejména zástupců person (viz výše).
