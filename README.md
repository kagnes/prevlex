# PrevLex – igekötős igék táblázata

A _PrevLex_ a magyar igekötős igék jelenleg legbővebb, manuálisan ellenőrzött táblázata. A [Magyar Nemzeti Szövegtár 2.0.4](http://clara.nytud.hu/mnsz2-dev/) ([Oravecz et al. 2014](http://www.lrec-conf.org/proceedings/lrec2014/pdf/681_Paper.pdf)) felhasználásával készült. Az igekötős finit igéken túl szerepelnek benne a korpuszban UNKNOWN-nak címkézett szavak és a hapaxok (egyszer előforduló szavak) is.

A _PrevLex_ részletes ismertetéséhez ld. [Kalivoda (2019)](http://real.mtak.hu/101690/1/XV.MagyarSzamitogepesNyelveszetiKonferencia.pdf).

# Az erőforrás szerkezete

A _PrevLex.txt_ egy TSV formátumú fájl, amely a következő oszlopokból áll:

1. oszlop: igekötős igelemma, az igekötő és az ige + jellel elválasztva (ahol az igelemma bizonytalan, ott a két lehetséges igelemma | jellel elválasztva)
2. oszlop: az igekötős ige tokengyakorisága az MNSZ 2.0.4-ben
3. oszlop: kétféle érték állhat itt, attól függően, hogy az ige kapott-e megfelelő annotációt az MNSZ 2.0.4-ben (FIN, ha igen és UNKNOWN, ha nem)
4. oszlop: azt jelzi, hogy az ige hány dokumentumban fordult elő
5. oszlop: a normalizált alak, amely csak a neologizmusoknál térhet el az első oszlop tartalmától (pl. agyon+hypeol ⟶ agyon+hájpol)
<!-- 6. oszlop és attól fölfelé: a konkrét igealak (az igekötő itt csak a könnyebb átláthatóság végett nincs feltüntetve) és szóközzel elválasztva a gyakorisága; az igealakok gyakoriság szerint csökkenő sorrendben állnak -->

# Licensz

Felhasználható oktatási, kutatási és magáncélra. Felhasználása esetén az alábbi cikk hivatkozandó:

Kalivoda Ágnes (2019). _Véges erőforrás végtelen sok igekötős igére._ In: Berend Gábor, Gosztolya Gábor, Vincze Veronika (szerk.): XV. Magyar Számítógépes Nyelvészeti Konferencia (MSZNY 2019). Szeged: Szegedi Tudományegyetem, TTIK, Informatikai Intézet. p. 331-344.

    @inproceedings{kalivoda2019,
        title = {V{\'e}ges er\H{o}forr{\'a}s v{\'e}gtelen sok igek\"{o}t\H{o}s ig{\'e}re},
        booktitle = {XV. Magyar Sz{\'a}m{\'i}t{\'o}g{\'e}pes Nyelv{\'e}szeti Konferencia (MSZNY 2019)},
        year = {2019},
        pages = {331--344},
        publisher = {Szegedi Tudom{\'a}nyegyetem, TTIK, Informatikai Int{\'e}zet},
        organization = {Szegedi Tudom{\'a}nyegyetem, TTIK, Informatikai Int{\'e}zet},
        address = {Szeged},
        author = {Kalivoda, {\'A}gnes},
        editor = {Berend, G{\'a}bor and Gosztolya, G{\'a}bor and Vincze, Veronika}
    }
    
