# Metodologia, fonti e conservazione dello storico

**Aggiornato il 23 novembre 2026.** Per i dati consulta la [guida principale](RIVISTE_TOP10_TOP25.md) e il [registro delle verifiche](AUDIT_2026-11-23.md).

## Tre classificazioni differenti

1. **Calibrazione locale UniCA / INF/01 (INFO-01/A):** l'elenco storico [`fascia-A.md`](fascia-A.md) si riferisce al **2023**, con calibrazione **24/06/2024**, e presenta la fascia A come top 10% secondo la procedura dipartimentale. **Non** è una classe A ANVUR nazionale per le aree bibliometriche. Il PDF ufficiale originale non è archiviato né è stato reperito pubblicamente.
2. **JCR / Clarivate:** la pubblicazione **2026** usa i dati **2025**. `Q1` è il primo quartile nella specifica categoria/anno. Clarivate descrive il calcolo dei quartili e dei decili tramite `rango / numero di riviste`. Un rango da una fonte secondaria va etichettato come tale.
3. **SCImago / Scopus:** quartili e SJR variano per categoria e anno. Le quote di posizione calcolate da `rango / totale` **non sono percentili ufficiali**. Non derivare un quartile quando è già mostrato esplicitamente (vedi discrepanza per *Applied Intelligence*).

**Per i concorsi italiani**, seguire il bando e le regole dell'ente valutatore: non esiste una sola lista di riviste top 10% valida ovunque.

## Dati e tracciabilità

| Percorso | Ruolo | Modificabile? |
|---|---|---|
| [`../data/journals.csv`](../data/journals.csv) | CSV storico preesistente (183 riviste) | **No**: conservare i dati originali |
| [`../data/archive/unica_inf01_2023_repository_snapshot.csv`](../data/archive/unica_inf01_2023_repository_snapshot.csv) | Copia immutata dello stesso CSV storico | **No** |
| [`fascia-A.md`](fascia-A.md) | Elenco storico trascritto, più ampio del CSV | Solo note editoriali, non sostituire i dati storici |
| [`../data/verified_2025.csv`](../data/verified_2025.csv) | Record 2025 per fonte/categoria, con data di verifica | Sì, solo con fonte documentata |
| [`AUDIT_2026-11-23.md`](AUDIT_2026-11-23.md) | Registro delle verifiche e dei limiti | Conservare come snapshot datato |

Il CSV storico **non è esaustivo**: contiene 183 righe di riviste, mentre `fascia-A.md` riporta anche altri titoli (ad es. SIMPAT, ESWA). I valori `A,B,C,D,E` del CSV storico **non sono quartili JCR** e non vanno ricalcolati senza la documentazione originaria.

## Schema del CSV 2025

Ogni riga rappresenta **una rivista, una fonte, un anno e una categoria**. Campi principali: `journal`, `issn`, `source`, `metric_year`, `category_area`, `category`, `quartile`, `rank`, `category_total`, `sjr`, `source_type`, `source_url`, `verified_on`, `notes`.

- `source_type=primary`: pagina ufficiale del fornitore (SCImago).
- `source_type=secondary`: riproduzione esterna di dati JCR; **non sostituisce** l'accesso a Clarivate.
- Campi vuoti: **dato non verificato**, non zero.
- `verified_on`: data della consultazione, distinta da `metric_year`.

## Procedura per futuri aggiornamenti

1. Cercare **titolo e ISSN**, annotando eventuali denominazioni storiche.
2. Verificare **anno**, **fonte**, **categoria disciplinare esatta**, **quartile** e, quando disponibile, **rango e totale**.
3. Per le graduatorie Computer Science, non usare ranghi di Mathematics, Energy o altre aree.
4. Per JCR top 10% derivare il decile dal rango ufficiale Clarivate; per SCImago mostrare sempre la **quota di posizione calcolata** separata dal quartile ufficiale.
5. Annotare URL, data e qualità della fonte; evitare di inventare ranghi mancanti.
6. Archiviare nuove calibrazioni istituzionali UniCA **in nuove cartelle per anno**, mantenendo l'originale 2023.
7. Evitare graduatorie globali basate su mix di h-index, JIF e SJR senza una metodologia esplicita.

### Fonti di metodo

- [Clarivate: edizione JCR 2026 e aggiornamenti](https://journalcitationreports.zendesk.com/hc/en-gb/articles/47808147130129-2026)
- [Clarivate: definizione di quartili e decili](https://supportcenter.clarivate.com/s/article/Journal-Citation-Reports-Quartile-rankings-and-other-metrics?language=en_US)
- [SCImago](https://www.scimagojr.com/)
- [Criteri ufficiali UniCA INFO-01/A, 2 marzo 2026](https://personale.unica.it/docric/public/fileadmin/user_upload/2025/associati/criteri/criteri_assr_17D_1125_01INFO-01.pdf) — non una lista di riviste.
