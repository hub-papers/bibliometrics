# Metodologia e provenienza dei dati

**Ultima revisione documentale:** 23 novembre 2026.

## Classificazioni distinte

1. **UniCA / INF/01:** [`fascia-A.md`](fascia-A.md) è l'elenco storico attribuito alla *Valutazione bibliometrica preliminare articoli su rivista — Categoria INF/01 — Anno 2023*, calibrazione **24/06/2024**. Nel documento riportato nel repository la **fascia A** corrisponde al **top 10%** della calibrazione. Non è una “classe A ANVUR” nazionale per le aree bibliometriche. Il documento istituzionale originale non è incluso: per usi amministrativi occorre reperire e verificare la fonte ufficiale.
2. **JCR / Clarivate:** `Q1` indica il primo quartile di una **categoria e di un anno specifici**. Per Informatica usare una categoria `Computer Science, ...`. **Q1 non implica automaticamente top 10%.**
3. **SCImago / Scopus-SJR:** registrare categoria, anno, rango, totale e quartile. **Q1 è top 25%, non necessariamente top 10%.**

La classificazione valida in un concorso dipende dal **regolamento dell'ente**; non esiste una classifica unica valida per tutti i dipartimenti italiani.

## Significato dei file

- [`../data/journals.csv`](../data/journals.csv): trascrizione **storica** con colonne `Rivista,A,B,C,D,E`. I valori numerici delle colonne **non sono quartili JCR né percentili SCImago aggiornati**. Senza la fonte originaria non vanno reinterpretati come flag o percentili. **Non sovrascrivere questo file con metriche 2025.**
- [`fascia-A.md`](fascia-A.md): elenco storico UniCA, riferimento 2023.
- [`2026-Top-Computer-Science-Journals.md`](2026-Top-Computer-Science-Journals.md): watchlist, **non** classifica JCR 2026 certificata.
- [`TOP_JOURNALS.md`](TOP_JOURNALS.md): graduatoria preesistente che mescola h-index, SJR e Impact Factor senza metodologia e annualità sufficientemente verificabili: **archivio**.
- [`../data/verified_2025.csv`](../data/verified_2025.csv): selezione **non esaustiva** di dati 2025 con fonte e data del controllo.
- [`RIVISTE_TOP10_TOP25.md`](RIVISTE_TOP10_TOP25.md): guida principale per la consultazione.

## Procedura per aggiornare le metriche

1. Identificare la rivista tramite **titolo e ISSN**, incluse varianti storiche.
2. Registrare **fonte**, **anno**, **categoria esatta**, **quartile**, **rango** e **totale** quando disponibili.
3. Registrare **URL, data del controllo e tipo di fonte** (ufficiale o secondaria).
4. Non trasferire una classificazione tra sistemi: fascia A UniCA, JCR Q1 e SCImago Q1 sono distinti.
5. Se si calcola `100 × rango / totale`, chiamarlo **quota approssimativa della posizione dall'alto**, non percentile ufficiale.
6. Non presentare la watchlist come elenco completo o certificato senza una verifica sistematica.
7. Per aggiornare la fascia A UniCA, acquisire **una nuova calibrazione ufficiale**, mantenendo intatto l'archivio 2023.

## Esempio documentato: Applied Soft Computing

- **UniCA:** fascia A nello storico 2023.
- **JCR 2025:** Q1, *Computer Science, Artificial Intelligence*, rango **35/210** da [fonte secondaria](https://akaturk.com/journals/18136?lang=en); verificare sul JCR ufficiale per usi amministrativi.
- **SCImago 2025:** Q1, *Software*, rango **50/527**, [scheda SCImago](https://www.scimagojr.com/journalsearch.php?q=18136&tip=sid).

Le altre riviste non sono state ricontrollate sistematicamente in questa revisione.
