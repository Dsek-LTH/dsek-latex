# DSek  ![LaTeX](https://upload.wikimedia.org/wikipedia/commons/thumb/9/92/LaTeX_logo.svg/320px-LaTeX_logo.svg.png "LaTeX")
Här hittar du D-sektionens latexmallar! Det finns några olika varianter på hemsidan, delvis [här](https://www.dsek.se/aktiva/grafiskprofil/latexhemma.php) och [här](https://www.dsek.se/aktiva/motion/). Detta repo skall uppdateras och underhållas för att garantera att DSek latexmallar aldrig blir utdaterade igen!

## Overleaf
**Absolut enklast sätt att skriva snygga Dsek-dokument är att utgå från Overleaf templaten.**

Det finns en fungerande DSek Overleaf-template, som ni kan hitta och klona [här!](https://www.overleaf.com/read/ckwqrthmfwhv). Du klonar genom **Menu -> Copy Project**. Den innehåller minst alla symboler och alla klasser/stilfiler som detta repo innehåller. 

## Installation
1. Klona detta repo, antingen ladda ned som en zip uppe i högra hörnet, eller i terminalen med följande 

`git clone https://github.com/Dsek-LTH/dsek-latex.git`

2. Kompilera .dtx-filerna till .cls/.sty etc med hjälp av 

`latex dsekXXXX.ins --> dsekXXXX.sty`

3. Konfigurera ditt LaTeX-workspace att använda detta repo som en TEXMF-directory. Du kan behöva möblera om lite så att mappstrukturen följer tex/latex/dsek-latex

4. Efter det kan du behöva uppdatera din filnamnsdatabas, men det beror lite på vilken dist du kör.


## Dokumentation
Alla filer här har dokumentation inkluderad i .dtx-filerna! För att generera dokumentationen kör du enbart 

`latex dsekXXXX.dtx --> dsekXXXX.pdf`, där pdfen kommer innehålla massa go fakta.


## LTH-symboler! How to????
LTH-symbolerna finns inte med i detta repo, men finns att hämta [här](https://www.dsek.se/aktiva/grafiskprofil/latexhemma.php). Det är ganska bökigt att få det att fungera klokt, men du behöver placera rätt mapp på rätt ställe, dvs fonts i din LaTeX-installation fonts-mapp etc... Enklast är att göra detta via Overleaf.

## Releases
Det finns en GitHub action som bygger alla nödvändiga klasser och stildokument. De hittar ni under Release. 
