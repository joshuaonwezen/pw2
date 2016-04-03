#Bundlin.com

##Improvements to be made

* mobile loadtime
* above the fold css
* scroll performance
* buildtool improvements
* html/css optimalisatie

##Mobile loadtime


##Above the fold css (critical css)
Critical CSS

Aangezien de CSS onderverdeeld is in modules is het vrijwel onmogelijk een critical css file aan te maken voor het builden voor above the fold loading. Hiervoor pakken we dus de compressed CSS die al via grunt aangemaakt wordt en laten we hiervoor een critical css file genereren. In de homepage html files willen we vervolgens de CSS inline zetten en in iedergeval bovenaan in de HTML.

![alt tag](criticalcss.png)

https://github.com/filamentgroup/criticalCSS

##Scroll performance

![alt tag](scroll1.png)


##Buildtool improvements
Bij critical css hebben we al gekeken een extra grunt task. Voor buildtool improvements zou ik aanraden aan lifely om over te stappen op gulp. Tijdens de presentatie hoorde ik al wel dat ze dit voor huidige projecten al wel doen. 

Een paar redenen waarom ik gulp beter vind dan grunt:

* Makkelijker op te zetten
* Grunt checked het hele project elke keer wanneer er ook maar 1 change is, gulp doet dit niet dus veel sneller
* Grunt = config, Gulp = code
* Gulp gebruikt streams dus is een heel stuk sneller.

##HTML/CSS Optimization

Voor dit project is gebruikt gemaakt van angular. Wat betreft HTML optimization verandert dit dus een hoop aangezien zij gebruik maken van inline if statements en animations via angular. Wat deels ontbreekt in de huidige opbouw van de HTML is het semantisch maken hiervan. Er zijn lijkt wel random overal articles en sections geplaatst met daarin een hele hoop div's om de animations goed te laten werken. Maar wat als dit wegvalt? Of als ik dit allemaal helemaal niet wil zien? 

![alt tag](angular.png)
