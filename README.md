# Solothurn (city): law history in git

The municipal law of the city of Solothurn (Stadt Solothurn, canton of Solothurn, Switzerland) as a git history: one file per article, one commit per amending act on the day it took effect, and the amending act as the commit's author. `git blame` names the act behind every paragraph; `git log` lists every change to an article; checking out a date gives the text in force that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law). The law of the canton of Solothurn is in [lexifina/switzerland-solothurn-law](https://github.com/lexifina/switzerland-solothurn-law); federal law is in [lexifina/switzerland-law](https://github.com/lexifina/switzerland-law).

The text is in German, exactly as the city publishes it.

## What this repository holds

96 acts with 101 versions so far: the Gemeindeordnung (the city's charter) first, then the city's other enactments in force (ordinances, regulations, tariffs and decisions), in the order of the systematic collection, added in parts of about 50. Agreements, concessions, directives and repealed acts are not included.

| Folder | Act | Versions | History |
| --- | --- | ---: | --- |
| `1-1-1/` | Gemeindeordnung der Einwohnergemeinde der Stadt Solothurn (SRS 1.1-1) | 1 | as enacted, 1 January 2026 |
| `1-2-1-vod/` | Vollzugsreglement zum Öffentlichkeitsprinzip und Datenschutz (SRS 1.2-1) | 1 | as enacted, 1 January 2003 |
| `1-2-2/` | Bearbeitungsreglement visuelle Überwachung Museum Blumenstein (SRS 1.2-2) | 1 | as enacted, 1 January 2014 |
| `1-2-3-archivreglement/` | Reglement über das Archivwesen (SRS 1.2-3) | 1 | as enacted, 22 March 2012 |
| `1-2-4/` | Betriebsreglement über die visuelle Überwachung in der Stadt Solothurn (SRS 1.2-4) | 1 | as enacted, 1 July 2026 |
| `1-2-4-1/` | Weisung zur visuellen Überwachung Schrankenanlage Cityplatz (SRS 1.2-4.1) | 1 | as enacted, 1 July 2026 |
| `1-2-4-3/` | Weisung zur visuellen Überwachung Schulhaus Schützenmatt (SRS 1.2-4.3) | 1 | as enacted, 1 July 2026 |
| `1-5-1-gogr/` | Geschäftsordnung des Gemeinderats (SRS 1.5-1) | 1 | as enacted, 1 November 2021 |
| `1-5-1-1/` | Pflichtenheft Wahlbüro (SRS 1.5.1-1) | 1 | as enacted, 1 January 2026 |
| `1-5-1-2/` | Pflichtenheft Baukommission (SRS 1.5.1-2) | 1 | as enacted, 1 January 2026 |
| `1-5-1-3/` | Pflichtenheft Altstadt- und Denkmalkommission (SRS 1.5.1-3) | 1 | as enacted, 1 January 2026 |
| `1-5-1-4/` | Pflichtenheft Planungs- und Umweltkommission (SRS 1.5.1-4) | 1 | as enacted, 1 January 2026 |
| `1-5-1-5/` | Pflichtenheft Sportkommission (SRS 1.5.1-5) | 1 | as enacted, 1 January 2026 |
| `1-5-1-6/` | Pflichtenheft Kulturkommission (SRS 1.5.1-6) | 1 | as enacted, 1 January 2026 |
| `1-5-1-7/` | Pflichtenheft Gesellschaftskommission (SRS 1.5.1-7) | 1 | as enacted, 1 January 2026 |
| `1-5-1-8/` | Pflichtenheft Beschwerdekommission (SRS 1.5.1-8) | 1 | as enacted, 1 January 2026 |
| `1-5-1-9/` | Pflichtenheft Dienst- und Gehaltskommission (SRS 1.5.1-9) | 1 | as enacted, 1 January 2026 |
| `1-5-1-10/` | Pflichtenheft Ständige Arbeitsgruppe Historisches Museum Blumenstein (SRS 1.5.1-10) | 1 | as enacted, 1 January 2026 |
| `1-5-1-11/` | Pflichtenheft Ständige Arbeitsgruppe Kunstmuseum (SRS 1.5.1-11) | 1 | as enacted, 1 January 2026 |
| `1-5-1-12/` | Pflichtenheft Ständige Arbeitsgruppe Naturmuseum (SRS 1.5.1-12) | 1 | as enacted, 1 January 2026 |
| `1-5-1-13/` | Pflichtenheft Ständige Arbeitsgruppe Fuss- und Veloverkehr (SRS 1.5.1-13) | 1 | as enacted, 1 January 2026 |
| `1-5-1-14/` | Pflichtenheft Ständige Arbeitsgruppe Umwelt (SRS 1.5.1-14) | 1 | as enacted, 1 January 2026 |
| `1-5-1-15/` | Pflichtenheft Rechnungsprüfungskommission (SRS 1.5.1-15) | 1 | as enacted, 1 January 2026 |
| `1-7-1-dgo/` | Dienst- und Gehaltsordnung für das Personal der Einwohnergemeinde der Stadt Solothurn (SRS 1.7-1) | 2 | oldest version available, then each consolidated version: 9 December 2024 to 1 January 2026 |
| `1-7-1-4-uniformreglement/` | Reglement für die Bekleidung, Ausrüstung und Bewaffnung der Stadtpolizei (SRS 1.7-1.4) | 1 | one version (the oldest available), 1 January 2003 |
| `1-7-1-6/` | Reglement über den Bezug der Treueprämien in Form von bezahltem Urlaub (SRS 1.7-1.6) | 1 | as enacted, 1 August 1994 |
| `1-7-1-7/` | Pikettdienstreglement (SRS 1.7-1.7) | 1 | one version (the oldest available), 14 January 2021 |
| `1-7-1-9/` | Richtlinien über die Arbeitszeitregelung und Entschädigung des städtischen Personals bei Vertretungen in privaten oder öffentlichen Institutionen sowie für die Ausübung öffentlicher Ämter und Nebenbeschäftigungen (SRS 1.7-1.9) | 1 | one version (the oldest available), 12 March 2015 |
| `1-7-1-10/` | Arbeitszeitreglement der Stadt Solothurn (SRS 1.7-1.10) | 1 | as enacted, 1 January 2026 |
| `1-7-1-11/` | Spesenreglement der Stadt Solothurn (SRS 1.7-1.11) | 1 | as enacted, 1 January 2026 |
| `1-7-1-12/` | Reglement für Leistungen bei unverschuldetem Verlust der Anstellung bei der Stadt Solothurn (SRS 1.7-1.12) | 1 | as enacted, 1 January 2007 |
| `4-1-1/` | Reglement über die Tagesstrukturen (SRS 4.1-1) | 1 | one version (the oldest available), 9 December 2024 |
| `4-1-1-1/` | Ausführungsbestimmungen gemäss Reglement über die Tagesstrukturen (SRS 4.1-1.1) | 1 | as enacted, 1 August 2024 |
| `4-1-2/` | Reglement über die Subventionierung der familienergänzenden Kinderbetreuung der Stadt Solothurn (Subjektfinanzierung) (SRS 4.1-2) | 1 | as enacted, 1 August 2022 |
| `4-1-2-1/` | Verordnung zum Reglement über die Subventionierung der familienergänzenden Kinderbetreuung (Subjektfinanzierung) (SRS 4.1-2.1) | 1 | as enacted, 1 August 2022 |
| `4-2-1/` | Reglement über den schulärztlichen Dienst (SRS 4.2-1) | 1 | one version (the oldest available), 13 August 2025 |
| `4-2-2/` | Reglement über die Schulzahnpflege (SRS 4.2-2) | 1 | one version (the oldest available), 13 August 2025 |
| `4-2-2-1/` | Beiträge der Erziehungsberechtigten an die Schulzahnpflege (SRS 4.2-2.1) | 1 | as enacted, 13 August 2025 |
| `4-2-3/` | Sozialtarif der Schulen (SRS 4.2-3) | 1 | as enacted, 1 August 1996 |
| `4-3-1/` | Reglement über die Musikschule (SRS 4.3-1) | 1 | one version (the oldest available), 9 December 2024 |
| `4-5-1/` | Badeordnung für das Schwimmbad Solothurn (SRS 4.5-1) | 1 | one version (the oldest available), 25 June 1996 |
| `4-5-2/` | Reglement über die Jugendsportförderung (SRS 4.5-2) | 1 | as enacted, 1 January 2018 |
| `4-7-2/` | Statuten der Stiftung der Zentralbibliothek Solothurn (SRS 4.7-2) | 1 | one version (the oldest available), 27 September 2011 |
| `4-7-2-1/` | Stiftungsreglement der Zentralbibliothek Solothurn (SRS 4.7-2.1) | 1 | as enacted, 3 May 1996 |
| `4-7-3/` | Reglement zur Förderung der Jugendkultur (SRS 4.7-3) | 1 | as enacted, 1 January 2002 |
| `4-7-4/` | Reglement über die Jugendmusikförderung (SRS 4.7-4) | 1 | as enacted, 1 July 2021 |
| `5-1-1/` | Polizeiordnung (SRS 5.1-1) | 1 | one version (the oldest available), 1 September 2024 |
| `5-1-2/` | Reglement über die Vergütung von inkonvenienten Diensten bei der Stadtpolizei Solothurn (SRS 5.1-2) | 1 | one version (the oldest available), 5 May 2020 |
| `5-1-3/` | Dienstreglement für die Stadtpolizei (SRS 5.1-3) | 1 | one version (the oldest available), 14 December 2021 |
| `5-3-1/` | Reglement über die Katastrophenvorsorge (SRS 5.3-1) | 1 | one version (the oldest available), 25 June 1996 |
| `5-3-2/` | Vertrag über den gemeinsamen regionalen Bevölkerungsschutz und den Zivilschutz (SRS 5.3-2) | 1 | as enacted, 1 January 2005 |
| `5-3-3/` | Vertrag über eine gemeinsame Zivilschutzorganisation (SRS 5.3-3) | 1 | one version (the oldest available), 23 May 2006 |
| `5-5-1/` | Feuerwehrreglement (SRS 5.5-1) | 1 | one version (the oldest available), 1 July 2007 |
| `6-1-1/` | Reglement über die Führung eines Fonds für Werterhalt bei den Liegenschaften des Finanzvermögens (SRS 6.1-1) | 1 | one version (the oldest available), 1 January 2016 |
| `6-1-2/` | Reglement über die Führung dreier Fonds für Projekte, Ausstellungen, Öffentlichkeitsarbeit und Objekterwerb der Museen (SRS 6.1-2) | 1 | as enacted, 1 January 2013 |
| `6-1-3/` | Reglement über die Führung dreier Fonds für die Ankäufe und den Unterhalt der Sammlungen der Museen (SRS 6.1-3) | 1 | as enacted, 1 January 2013 |
| `6-1-5/` | IKS Verwaltungsreglement (SRS 6.1-5) | 1 | as enacted, 1 January 2024 |
| `6-3-1/` | Steuerreglement (SRS 6.3-1) | 1 | one version (the oldest available), 1 January 2017 |
| `6-4-1/` | Gebührentarif (SRS 6.4-1) | 1 | one version (the oldest available), 19 December 2017 |
| `6-4-1-1/` | Anhang 1: Selbstkosten für die Verrechnung nach Aufwand gemäss § 5 Gebührentarif, SRS 6.4-1 (SRS 6.4-1.1) | 1 | as enacted, 1 January 2026 |
| `6-4-1-2/` | Anhang 2: Gebühren für die Benützung der städtischen Liegenschaften gemäss § 60 Gebührentarif, SRS 6.4-1 (SRS 6.4-1.2) | 1 | as enacted, 1 January 2021 |
| `6-4-1-3/` | Anhang 3: Gebühren für die Benützung von Schul- und Sportanlagen gemäss § 62 Gebührentarif, SRS 6.4-1 (SRS 6.4-1.3) | 1 | one version (the oldest available), 8 December 2025 |
| `6-4-1-4/` | Anhang 4: Eintrittspreise und Gebühren Schwimmbad und Hallenbad Pädagogische Fachhochschule gemäss § 61 Gebührentarif, SRS 6.4-1 (SRS 6.4-1.4) | 2 | oldest version available, then each consolidated version: 8 December 2025 to 1 April 2026 |
| `6-4-1-5/` | Anhang 5: Mietgebühren für Fahrzeuge, Material und Einrichtungen und die damit zusammenhängenden Dienstleistungen (§ 62 Gebührentarif, SRS 6.4-1) (SRS 6.4-1.5) | 1 | one version (the oldest available), 1 October 2025 |
| `6-4-1-6/` | Anhang 6: Gebühren nach § 82 Bestattungs- und Friedhofreglement (SRS 8.2-1) (SRS 6.4-1.6) | 1 | one version (the oldest available), 1 November 2025 |
| `6-4-1-7/` | Anhang 7: Gebühren für Fotokopien und EDV-Ausdrucke gemäss § 17 lit. d Gebührentarif (SRS 6.4-1) (SRS 6.4-1.7) | 1 | as enacted, 1 January 2014 |
| `6-6-1/` | Weisungen über die Benützung von Schulräumen und ‑anlagen (SRS 6.6-1) | 1 | one version (the oldest available), 1 January 2021 |
| `6-7-1/` | Gemeindebeschluss über die Beteiligung an der REGIOBANK SOLOTHURN (SRS 6.7-1) | 1 | as enacted, 12 December 2000 |
| `6-7-1-1/` | Vereinbarung betreffend Beteiligung der EGS an der REGIOBANK (SRS 6.7-1.1) | 1 | as enacted, 27 June 2017 |
| `6-8-1-submissionsreglement/` | Reglement über die Vergabe öffentlicher Aufträge der Stadt Solothurn (SRS 6.8-1) | 1 | as enacted, 1 January 2012 |
| `7-1-1/` | Bau- und Zonenreglement (SRS 7.1-1) | 1 | one version (the oldest available), 23 April 2013 |
| `7-1-2/` | Baureglement (SRS 7.1-2) | 1 | as enacted, 2 May 2023 |
| `7-1-3/` | Reglement zum Planungsausgleich (SRS 7.1-3) | 1 | as enacted, 25 June 2019 |
| `7-1-4/` | Grundeigentümerbeitragsreglement (SRS 7.1-4) | 1 | one version (the oldest available), 1 January 2019 |
| `7-1-5/` | Reglement über Parkplätze für Motorfahrzeuge (SRS 7.1-5) | 1 | one version (the oldest available), 20 December 2022 |
| `7-1-6/` | Richtlinien der Kommission für Altstadt- und Denkmalfragen (SRS 7.1-6) | 1 | as enacted, 22 November 2006 |
| `7-1-7/` | Interne Richtlinien für Beitragsleistungen an Altstadt- und Denkmalschutzobjekte sowie an Objekte in Ortsbildschutzgebieten (SRS 7.1-7) | 1 | as enacted, 19 December 1995 |
| `7-4-1-1/` | Reglement über die Versorgung von Energie und Wasser durch die Regio Energie Solothurn (SRS 7.4.1-1) | 2 | oldest version available, then each consolidated version: 9 December 2008 to 1 January 2026 |
| `7-4-1-1-1/` | Statuten der Regio Energie Solothurn (SRS 7.4.1-1.1) | 2 | oldest version available, then each consolidated version: 31 October 2017 to 1 January 2026 |
| `7-4-1-1-2/` | Konzessionsvertrag zwischen der Einwohnergemeinde der Stadt Solothurn (EGS) und der Regio Energie Solothurn (RES) (SRS 7.4.1-1.2) | 1 | as enacted, 1 January 2024 |
| `7-4-1-1-3/` | Eignerstrategie für die Regio Energie Solothurn (SRS 7.4.1-1.3) | 2 | as enacted, then each consolidated version: 23 August 2022 to 18 August 2026 |
| `7-4-2-1/` | Richtlinien für den Anschluss von Endverbrauchern und Arealnetzbetreibern an das Elektrizitätsnetz der Regio Energie Solothurn (SRS 7.4.2-1) | 1 | as enacted, 27 March 2008 |
| `7-4-2-2/` | Konzessionsvertrag über die Versorgung der Einwohnergemeinde der Stadt Solothurn mit Fernwärme (SRS 7.4.2-2) | 1 | as enacted, 20 November 2009 |
| `7-4-4-1/` | Reglement über die Abfallbewirtschaftung (SRS 7.4.4-1) | 1 | one version (the oldest available), 25 June 1996 |
| `7-4-4-1-1/` | Grundgebühren für die Abfallbeseitigung (SRS 7.4.4-1.1) | 1 | one version (the oldest available), 1 January 2022 |
| `7-7-1/` | Reglement über die Benützung der öffentlichen Parkplätze (SRS 7.7-1) | 1 | one version (the oldest available), 24 June 2003 |
| `7-7-2/` | Ausführungsbestimmungen über das unbeschränkte Parkieren in der Blauen Zone (Anwohnerprivilegierung) (SRS 7.7-2) | 1 | one version (the oldest available), 24 October 2024 |
| `8-2-1/` | Bestattungs- und Friedhofreglement (SRS 8.2-1) | 1 | one version (the oldest available), 1 January 2015 |
| `8-2-2/` | Besondere Vorschriften über den Betrieb des Friedhains (SRS 8.2-2) | 1 | as enacted, 18 November 2021 |
| `8-2-3/` | Reglement über die Gestaltung und den Betrieb der Kindergrabstätte (SRS 8.2-3) | 1 | as enacted, 28 August 2012 |
| `8-2-4/` | Besondere Vorschriften über den Betrieb der Urnengemeinschaftsanlage (SRS 8.2-4) | 1 | as enacted, 22 March 2012 |
| `9-2-1/` | Flurreglement (SRS 9.2-1) | 1 | as enacted, 24 June 2014 |
| `9-4-1/` | Reglement über die Erhebung einer Kurtaxe (SRS 9.4-1) | 1 | one version (the oldest available), 23 June 2009 |
| `9-5-1-marktreglement/` | Reglement über die Nutzung des öffentlichen Raumes für Märkte und marktähnliche Nutzungen (SRS 9.5-1) | 1 | one version (the oldest available), 23 June 2009 |
| `9-5-1-1/` | Vollzugsvorschriften zum Reglement über die Nutzung des öffentlichen Raumes für Märkte und marktähnliche Nutzungen (SRS 9.5-1.1) | 1 | one version (the oldest available), 22 August 2024 |
| `9-5-2/` | Reglement über das Taxiwesen (SRS 9.5-2) | 1 | one version (the oldest available), 1 July 2024 |

## Source

The SRS (systematic collection) of the city, published by the city at <https://reglemente.stadt-solothurn.ch/>. For each act it gives every consolidated version it holds, with the day each version took effect, and a change table listing each amendment: its decision date, the day it took effect, the provision it touched and its entry in the chronological collection (CRS). Annexes the collection publishes only as separate PDF files are not included.

## Dates

- Each commit is dated at **noon, Europe/Zurich, on the day the version took effect**, as the collection gives it ("in Kraft seit / von"). The decision date of each amending act is the `Enacted:` trailer.
- An act's first commit is its oldest version in the collection. It is credited to the act as enacted only when the change table shows no amendment in force before it; otherwise it is the "oldest version available", naming the earlier amendments.
- Versions that take effect after the retrieval day are on the `zukunft` branch, never merged into `main`.
- `--before="YYYY-MM-DD"` alone uses your clock's time of day; use `T23:59:59Z` or `tools/on.py`.

## Files

`<act>/art-005.md` is Art. 5 (or § 5), `art-005a.md` Art. 5a; `ingress.md` holds the title, date and preamble; `gliederung.md` the section headings; `schluss.md` the closing formula and signatures. One paragraph or list item per line. Amendment markers (`*`), footnote numbers and the "Stand" date are left out.

## How it is checked

- Every version of every act is read back from git on the day it took effect and on the day before (`tools/check_repo.py`); both must match `corpus.json`.
- The letters and digits of every version equal those of the city's own text of that version, and every article's text appears in it in order.
- Health checks: no merge commits, commit dates never go backwards, nothing dated in the future, and every commit's trailers parse.

## What "author" means

The author of a commit is the amending act, named by its entry in the chronological collection (CRS), with an e-mail address that cannot exist (`<act key>@reglemente.stadt-solothurn.ch.invalid`). Where one version holds changes by several amending acts and the change table does not say which provision each one touched, the commit names them all. The committer is always Lexifina.

## Limits

This is not an official publication. The binding text is the one the city publishes as binding. The history starts with the oldest consolidated version the collection holds for each act, which for many acts is later than the act's enactment. Only the acts listed above are included.
