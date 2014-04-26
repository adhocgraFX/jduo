jduo
====

## Super lightweight off-canvas sketch for rwd templates.

Jduo ist eine kleine Skizze einer möglichst einfach zu implementierenden off-canvas Funktionalität.

inspired by codrops Blueprint: Slide and push Menus / https://github.com/codrops/Blueprint-SlidePushMenus

## How to ..

Notwendig sind folgende 2 Dateien:

* classie.min.js > 560 bytes
* off-canvas.less > off-canvas.css > 1.61kb

Alle weiteren less Dateien beziehen sich auf das Layout der Demo.

In der index.html wird gezeigt, wie den beiden Elementen nav und aside die off-canvas Funktionalität zugewiesen wird.

## Das Grundprinzip

In den üblichen grid-layouts besitzen die container-divs die Eigenschaften float: left und position: relative. Im mobile first Ansatz wird die Breite auf width: 100% gesetzt. Sie wird mittels media queries dann für größere devices differenziert, z.B. in ein 2-Spaltensystem von 66.66% zu 33.33%. Die container-divs, die man für kleinere devices in den off-canvas setzen will, muss man nun für die schmalen Breiten via media queries aus diesem System herausbrechen, indem man ihnen position: absolute zuweist. Das ist im Prinzip alles.

Funktioniert auf allen Browsern, die media queries und javascript verstehen.