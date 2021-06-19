# Mriežka na pozadí dokumentu k meraniu sadzby v rôznych jednotkách

Semestrálna práca na předmět BI-TEX, Adam Barla, LS 2020/2021

Táto práca je určená ako pomôcka pri umiestňovaní sadzby. Ide o makro makro pre `OpTeX` určené ne hľadanie príčin nesprávneho umiestnenia sadzby, prípadne zisťovania presnej pozície textu v dokumente.
Makro vytvorí mriežku na pozadí každej stránky vašeho dokumentu. Pritom nemení doterajšie rozloženie textu. Prípadného pozadia definovaného v `\pgbackground` sa ale prepíše. Veľkosť políčok aj veľkosť samotnej mriežky si môžte definovať sami.

>## Dokumentácia

Podrobný popis použitia a tvorby makra je v súbore `documentation.pdf`, ktorý nájdete v priečinku `\doc`. Môžeteho vygenerovať príkazom:

`optex documentation.tex`

V rovnakom priečinku nájdete aj tri ukážky použita makra. Bližšie sú popísané v dokumentácii.

>## Stručné použitie

Definíciu makra nájdete v súbore `mriezka.tex` v priečinku `makro`. Tento súbor musíte priložiť k svojmu dokumentu pomocou `\include mriezka.tex`. Potom ho môžte použiť s defaultnými nastaveniami príkazom:

`\grid ,(,,,)`

alebo môžte definovať parametre mriežky:

`\grid <horizontal spacing>,<vertical spacing>(<left margin>,<top margin>, <horizontal size>,<vertical size>)`

Pri definícii parametrov môžte nechať niektoré z nich aj prázdne a tým bude ich hodnota nastavená na implicitnú. Parametre udávajte s jednotkami definovanými v `TeX`u (pt, in, mm, cm, atď.).

Ďalej sa v priečinku `makro` nachádza testovací text, na ktorom sú predvedené ukážky v dokumentácii.
