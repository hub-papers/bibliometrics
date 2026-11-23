# Riviste top 10% e top 25% in Informatica

**Aggiornamento bibliometrico:** 2026-11-23 · **Anno delle metriche:** 2025 (rilasciate nel 2026) · **Copertura:** selezione verificata, **non censimento esaustivo**.

Questa è la **pagina principale** del repository. Per la tabella consultabile/esportabile usa [`data/verified_2025.csv`](../data/verified_2025.csv).

## 1. Quale top 10% o top 25%?

| Classificazione | Che cosa significa | Fonte |
|---|---|---|
| **Fascia A UniCA (INF/01)** | Fascia superiore nella calibrazione locale riferita al **2023**, datata **24/06/2024** | [Elenco storico trascritto](fascia-A.md); [archivio del CSV originario](../data/archive/README.md) |
| **JCR Q1 in Computer Science** | Primo quartile (top 25%) di una specifica categoria **Computer Science** nel JCR dell'anno indicato | [Clarivate](https://supportcenter.clarivate.com/s/article/Journal-Citation-Reports-Quartile-rankings-and-other-metrics?language=en_US) |
| **JCR top 10% in Computer Science** | Decile derivato dal rango JCR della specifica categoria: `rank / totale ≤ 0.10` | [Regola Clarivate per i decili](https://supportcenter.clarivate.com/s/article/Journal-Citation-Reports-Quartile-rankings-and-other-metrics?language=en_US) |
| **SCImago Q1 / top 10% in Computer Science** | Quartile SJR e posizione in una specifica categoria dell'area **Computer Science**; top 10% solo con rango/percentile verificato | [SCImago](https://www.scimagojr.com/) |

**Non sono classificazioni intercambiabili.** Non esiste una fascia A nazionale ANVUR unica per tutte le riviste delle aree bibliometriche. Il criterio da applicare in un concorso dipende dal bando e dalla procedura di valutazione.

## 2. Tabella rapida: Computer Science, dati 2025

La colonna **quota posizione** è `rango / totale × 100`, una **misura derivata e approssimativa**, non il percentile ufficiale SCImago. I ranghi si riferiscono **esclusivamente alle categorie Computer Science indicate**, non a categorie Mathematics o Energy.

| Rivista | Categoria SCImago 2025 (Computer Science) | Q | Rango | Quota posizione | Top 10% dal rango? | UniCA 2023 (elenco storico) |
|---|---|:---:|---:|---:|:---:|---|
| [Applied Soft Computing](https://www.scimagojr.com/journalsearch.php?q=18136&tip=sid) | Software | Q1 | 50/527 | **9,5%** | **Sì** | Presente |
| [Future Generation Computer Systems](https://www.scimagojr.com/journalsearch.php?q=12264&tip=sid) | Hardware and Architecture | Q1 | 18/256 | **7,0%** | **Sì** | Presente |
| [Intelligent Systems with Applications](https://www.scimagojr.com/journalsearch.php?q=21101051831&tip=sid) | Signal Processing | Q1 | 22/196 | 11,2% | No | Non presente |
| [Sustainable Computing: Informatics and Systems](https://www.scimagojr.com/journalsearch.php?q=19700201455&tip=sid) | Computer Science (miscellaneous) | Q1 | 57/403 | 14,1% | No | Presente |
| [Journal of Systems and Software](https://www.scimagojr.com/journalsearch.php?q=19309&tip=sid) | Hardware and Architecture | Q1 | 43/256 | 16,8% | No | Presente |
| [Expert Systems with Applications](https://www.scimagojr.com/journalsearch.php?q=24201&tip=sid) | Computer Science Applications | Q1 | Da verificare | — | Non determinabile | Presente |
| [Applied Intelligence](https://www.scimagojr.com/journalsearch.php?q=23674&tip=sid) | Artificial Intelligence | **Q2** | 124/549 | 22,6%* | No | Presente |

* **Attenzione a Applied Intelligence:** SCImago mostra esplicitamente **Q2** nonostante il rapporto aritmetico 124/549 sia circa 22,6%. Non convertire automaticamente il rapporto in un quartile ufficiale; in caso di discordanza prevale il dato di quartile mostrato dalla fonte, da verificare nel contesto della categoria.

Per **Energy and AI, Ecological Informatics, Information Sciences, Simulation Modelling Practice and Theory ed Environmental Modelling & Software** ho verificato dati SJR 2025 e categorie disciplinari, ma **non** un rango/denominatore 2025 sufficiente per attribuire loro il top 10% *in Computer Science*. Non le classifico quindi arbitrariamente come top 10% CS.

## 3. JCR 2025: esempio con due categorie

| Rivista | Categoria JCR Computer Science | Quartile | Rango | Quota posizione |
|---|---|:---:|---:|---:|
| **Applied Soft Computing** | Artificial Intelligence | Q1 | 35/210 | 16,7% |
| **Applied Soft Computing** | Interdisciplinary Applications | Q1 | 25/185 | 13,5% |

I dati per questa rivista provengono da una [fonte secondaria che riproduce i ranghi JCR](https://akaturk.com/journals/18136?lang=en), **non** da un'esportazione Clarivate autenticata. Per un uso amministrativo occorre verificarli nel JCR istituzionale. In entrambe le categorie risulta **Q1, ma non top 10%** in base ai ranghi riportati.

Il **JCR 2026 contiene metriche 2025**, pubblicate il 17 giugno 2026, con un reload il 14 ottobre 2026: [comunicazione ufficiale Clarivate](https://journalcitationreports.zendesk.com/hc/en-gb/articles/47808147130129-2026).

## 4. Stato della calibrazione UniCA

- Lo storico [`fascia-A.md`](fascia-A.md) dichiara di basarsi sulla valutazione **INF/01, anno 2023, calibrazione 24/06/2024**. La fonte istituzionale originale (PDF) **non è presente nel repository** e non è stata recuperata pubblicamente in questa verifica.
- [`data/journals.csv`](../data/journals.csv) è il **CSV storico preesistente** (183 righe di riviste, più intestazione), mantenuto senza alcuna modifica e duplicato [nell'archivio](../data/archive/README.md). **Non è un elenco completo** di tutte le riviste nominate in `fascia-A.md` (es. SIMPAT ed Expert Systems with Applications compaiono nel Markdown ma non nel CSV).
- È stato trovato un [documento ufficiale UniCA del 2 marzo 2026](https://personale.unica.it/docric/public/fileadmin/user_upload/2025/associati/criteri/criteri_assr_17D_1125_01INFO-01.pdf) con criteri di una selezione INFO-01/A. **Non contiene una nuova lista di riviste né una calibrazione aggiornata**.
- **Non è stata individuata una calibrazione ufficiale successiva al riferimento 2023** nelle fonti pubbliche consultate; ciò non prova che non ne esistano versioni interne.

## 5. Come consultare e aggiornare

1. Verifica **quale fonte richiede il tuo bando**: UniCA, JCR, SCImago o altro.
2. Per le metriche 2025, cerca la rivista nel [CSV verificato](../data/verified_2025.csv). Ogni riga riporta fonte, anno, categoria e **data di verifica**.
3. **Q1 = top 25%**, non necessariamente top 10%. Per il top 10% controlla il rango/denominatore **nella categoria CS**.
4. Se la rivista manca dal CSV, significa **non ancora verificata**, non che sia fuori dal Q1.
5. Se arriva una nuova calibrazione UniCA, archiviala **separatamente** indicando l'anno e conservando il dataset storico 2023.

Vedi [metodologia](methodology.md) e [registro di verifica del 23 novembre 2026](AUDIT_2026-11-23.md).
