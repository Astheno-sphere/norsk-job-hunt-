# Alisa Ramsli free files (extracted Nov 2026)

Source: https://alisanorgeland.github.io/site/#free. Originals saved to Tiger's Downloads via Chrome: `CV mal norsk .docx` and `ATS-keywords-Norway-Alisa-Ramsli.pdf`. Not committed here (her files).

## 1. Her Norwegian CV template: structure, top to bottom
1. Header: photo slot, name, born (date), address, phone, email.
2. **Nøkkelkvalifikasjoner**: the most relevant qualifications for this specific job, hard and soft skills, a few sentences.
3. **Erfaring**: MM.YYYY to MM.YYYY, then company, place, title; responsibilities first, then results.
4. **Utdanning**: years, degree, subject, institution, place.
5. **Kurs og annen opplæring**: courses, including Norwegian course level passed.
6. **Språk**: each language with level, oral and written.
7. **Førerkort**.
8. **Hobby**: interests relevant to the job.
9. **Referanser**: oppgis ved forespørsel.

### Gap check against `03-cvs/trainee-no.md`
| Her structure | Our trainee CV | Action |
|---|---|---|
| Nøkkelkvalifikasjoner at top | "Kort om meg" (profile prose) | Rename/reshape into a tailored Nøkkelkvalifikasjoner block per job. Ellis says the same. |
| Språk section with levels | Norwegian line only in profile | Add Språk: Engelsk flytende; Norsk tidlig samtalenivå, mål B1 2026; [mother tongue, ASK TIGER]. Settles C1 honestly. |
| Hobby section | none | Add one active hobby (her interview advice too). [ASK TIGER] |
| MM.YYYY dates | years or placeholder | Use month precision. STARZZ months [local file]. |
| Kurs section | certificates block | Rename to "Kurs og sertifiseringer"; Norwegian course goes here when there is one. |
| Born date and photo | none | Optional. Traditional Norwegian firms expect birth date more often; international firms strip it (Duong). Variable `company_style`. Tiger's call. |
| Referanser oppgis ved forespørsel | named referees, contacts on request | Keep names: stronger trust signal. Both acceptable. |

## 2. ATS keywords: 30 personal qualities Norwegian employers look for
Her rule: never paste as a list. Build them into phrases and examples, choose only those that fit the ad, adapt per job.

| # | Norsk | English | Tiger proof available |
|---|---|---|---|
| 1 | Samarbeidsorientert | team player | START Molde partnerships team |
| 2 | Selvstendig | works independently | self-built research models |
| 3 | Ansvarsbevisst | responsible | LO Økonomiansvarlig (budget) |
| 4 | Initiativrik | shows initiative | "study from the outside" models |
| 5 | Løsningsorientert | solution-oriented | BEM KEK MRPeasy, +25% OTD |
| 6 | Strukturert | structured | compliance documentation flow, Astorvia |
| 7 | Resultatorientert | results-oriented | +25% OTD; 30% audit-cycle cut |
| 8 | Pålitelig | reliable | STARZZ fixed-date deliveries |
| 9 | Fleksibel | flexible | |
| 10 | Effektiv | efficient | audit cycles three days to eight hours |
| 11 | Kommunikasjonssterk | strong communicator | NORS 2025 presentation |
| 12 | Serviceinnstilt | service-minded | |
| 13 | Engasjert | engaged | START Molde, LO board |
| 14 | Kundeorientert | customer-oriented | |
| 15 | Motivert | motivated | |
| 16 | Endringsvillig | open to change | |
| 17 | Målrettet | goal-oriented | |
| 18 | Tålmodig | patient | |
| 19 | Proaktiv | proactive | warm outreach, built models unasked |
| 20 | Lærevillig | eager to learn | Norwegian study; S/4HANA MM and PS |
| 21 | Innovativ | innovative | TRF thesis |
| 22 | Presis | precise and punctual | spec compliance (STARZZ Mode 2) |
| 23 | Handlekraftig | gets things done | |
| 24 | Empatisk | empathetic | |
| 25 | Tillitsvekkende | inspires trust | compliance / KYC work |
| 26 | Relasjonsbygger | relationship builder | fylkeskommune seminar |
| 27 | Beslutningsdyktig | decisive | |
| 28 | Høy arbeidskapasitet | high work capacity | |
| 29 | Kvalitetsbevisst | quality-conscious | supplier qualification |
| 30 | Analytisk | analytical | R, AMPL, VRP models |

Blank proof = no verified example yet; do not use the word without one.

## 3. Keyword extraction step (our version of her prompt)
She suggests asking an AI to analyse the ad and list the 30 most relevant keywords for Norwegian ATS systems (she names Webcruiter, ReachMee/Talentech, Jobbnorge, EasyCruit, Teamtailor, Workday, SuccessFactors, Jobylon, RecMan and others), focusing on skills, tools, certifications and industry terms.
In our flow this is Stage A: extract the ad's keywords into `templates/job-intake.md` "task words", then the red team's filter 10 checks coverage. Only keywords Tiger can back with a proof line get used.
