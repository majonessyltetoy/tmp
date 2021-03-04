
[Inferring gender of Reddit users](https://kola.opus.hbz-nrw.de/opus45-kola/frontdoor/deliver/index/docId/1619/file/Master_thesis_Vasilev.pdf)
2018
Samme som jeg skal prøve, annen metode.
dataset: labeled users from r/relationships, r/AskMen, r/relationship_advice, r/AskWomen, r/tall
features: GLoVE embeddings
model: LogReg, XGBoost, LSTM, charCNN

Dataset med bruker kjønn på github https://github.com/SomeSnm/master_thesis

---

[She’s Reddit: A source of statistically significant gendered interest information?](https://arxiv.org/pdf/1810.08091.pdf)
2019
Kvantifiserer kjønnsdeltagelse over subreddits. Kjønnsklasifisering er basert på brukernavn-kjønn antagelse.
De hevder at å delta på Reddit er en form for konkuranse(karma) og dermed iboende mans dominert....

---

[Privacy on Reddit? Towards Large-scale User Classification](https://aisel.aisnet.org/cgi/viewcontent.cgi?article=1042&context=ecis2015_cr)
2015
Forutsi kjønn og statsborgerskap.
Model: SVM
Features: LDA
resultat: 87% AUC for kjønn

De fant kjønn med å søke etter possesive "my" etterfulgt av "husband", "girlfriend", etc

---

[Age and Gender in Reddit Commenting and Success](https://repository.kisti.re.kr/bitstream/10580/8657/1/E1JSCH_2014_v2n3_18.pdf)
2014
Ser etter sammenheng mellom godt likte kommentarer og kjønn/alder.
De har bare 734 deltagere i studie!
Eldre brukere skriver lengre kommentarer og får dermed mer poeng
MEN menn skriver i gjennomsnitt kortere kommentarer og får i gjennomsnitt mer poeng en kvinner.

Altså er det ikke statistisk significant?

---

[Exploration of Gender Differences in COVID-19 Discourse on Reddit](https://arxiv.org/pdf/2008.05713.pdf)
2020
De måler Valence-Arousal-Dominance(VAD) for reddit kommentarer mellom kjønn. Dataset er hentet fra r/AskMen og r/AskWomen
model: beta regression
features:  valence, arousal, and dominance / BERT

De har dataset med F/M reddit brukerer https://github.com/ellarabi/covid19-demography

---

[Detecting anxiety on Reddit](https://www.aclweb.org/anthology/W17-3107.pdf)
2017
Anslå om en bruker har angst utifra innlegget(ikke kommentaren) dems.
model: LR/SVM/NN
features: word embeddings/LDA/LIWC/N-grams
Resultat: 91% accuracy med embeddings/N-grams. 98% hvis de kombinerer det med LIWC

Interresant lexical features med LIWC/LDA

---

[Discriminating Gender on Twitter](https://apps.dtic.mil/sti/citations/AD1108485)
2011
Anslå kjønn på twitter brukere.
Fire felt: description, alle tweets, screen name, full name
model: Winnow
features: N-grams

Bare tweets ga 75%