<h1 align="center"> HOMO-MEX <img src="assets/xx-pride-lgbt.png" width="40" height="40"></h1>
<p align="center">
    <a href="LICENSE">
        <img alt="License" src="https://img.shields.io/badge/License-CC_BY_NC_ND_4.0-red">
    </a>
    <a href="CODE_OF_CONDUCT.md">
        <img alt="Contributor Covenant" src="https://img.shields.io/badge/Contributor%20Covenant-v2.0-orange">
    </a>
    <!-- <img alt="LLMs" src="https://img.shields.io/badge/LLMs-GPT4%2CGPT3.5%2CCommand%2CJurassic%2CLLaMa2%2CMixtral-yellow"> -->
    <!-- <img alt="Domains" src="https://img.shields.io/badge/Domains-Chat,Literary,News,Reviews,WikiHow,Wikipedia-yellow"> -->
    <img alt="Languages" src="https://img.shields.io/badge/Languages-esMx-green">
    <img alt="Subtasks" src="https://img.shields.io/badge/Subtasks-SocialMedia%2CSongLyrics-blue">
    <img alt="Organizers" src="https://img.shields.io/badge/Organizers-UNAM%2CIPN-violet">
</p>

<h2 align="center"> About </h2>
<p>
The HOMO-MEX: Hate speech detection towards the Mexican Spanish speaking LGBT+ population shared task will take place as part of IberLEF 2024, the 6th Workshop on Iberian Languages Evaluation Forum at the SEPLN 2024 Conference, which will be held in Valladolid, Spain on the 26th of September, 2024.
</p>

<h2 align="center"> Sub Tasks </h2>

<p>
This year Homo-Mex is including tasks for the Tweet data annotated for LGBT+phobia and identification of specific types of LGBT+phobia as well as an additional task classifing songs!
</p>

<h3 align="center"> Track 1: Hate Speech detection track (multi-class) </h3>

<p>
The objective of this task is to predict the label of each individual tweet. The three possible labels a tweet can have are LGBT+phobic (P), not LGBT+phobic (NP) , and not LGBT+related (NR). We define each one of these labels next: <br> <br>

<ul>
<li> <b>LGBT+phobic (P)</b> tweets contain hate speech directed against any person whose sexual orientation and/or gender identity differs from cis-heterosexuality. </li>

<li> <b>Not LGBT+phobic (NP)</b> tweets are those that do not include any hate speech against the LGBT+ population but do mention this community. </li>

<li> <b>Not LGBT+related (NR)</b> tweets are those that are not related in any way to the LGBT+ community. </li>
</ul> <br>
In this first track, participants will be able to assign one label to each tweet, e.g. Tweet X can be assigned the label "P", and Tweet Y can be assigned with label "NR". <br> <br>

Given that each tweet can have one of these tree labels, the output submission must have two columns, first column corresponds to the ID of the tweet and the second column corresponds to your prediction value for each tweet indicating "P", "NP" or "NR". E. g. <br> <br>

ID_Track1, "P" - this tweet defined as LGBT+phobic. <br> <br>

ID_Track1, "NR" - this tweet defined as not LGBT+phobic related.
</p>

<h3 align="center"> Track 2: Fine-grained hate speech detection track (multi-labeled) </h3>

<p>
The objective of this task is to predict one or more label(s) of each individual tweet that contains LGBT+phobic hate speech. <br> <br>

The labels in this sub-track are related to various phobias related to LGBT+phobia. Each one of these phobias is described next: <br> <br>

<ul>
<li> <b>Lesbophobia</b> is homophobia explicitly directed at homosexual people who identify as female. </li>

<li> <b>Gayphobia</b> is homophobia explicitly directed at homosexuals who identify as male. </li>

<li> <b>Biphobia</b> refers to hate speech directed against people who are attracted to more than one gender. </li>

<li> <b>Transphobia</b> refers to hate speech directed against non-cis-gendered people. </li>

<li> <b>Other LGBT+phobia</b> is hate speech against other sexual and gender minorities not included in any of the categories described above (e.g "aphobia" which describes the hatred received by people who do not feel sexual attraction). </li>

<li> <b>Not LGBT+related (NR)</b>. Tweets are those that are not related in any way to the LGBT+ community. </li>
</ul>

In this second track, participants will be able to assign one or more labels to each tweet, e.g. Tweet X can be assigned the labels "L", "G", "B", and Tweet Y can be assigned only the label "O". <br> <br>

Given that each tweet can have one to five labels, the output submission must follow this strict order: "L", "G", "B", "T", "O", "NR". <br> <br>

The tweets assigned less than five labels must include the string "0" in place of the label(s) that were not predicted for such tweets, e.g. <br> <br>

ID_Track2, "1", "1", "1", "0", "1", "0" - this tweet would be assigned the labels "L", "G", "B" and "O". The zeros indicate that "B" and "NR" were not predicted for this instance. <br> <br>

ID_Track2, "0", "0", "1", "0, "0", "0" - this tweet would be assigned only the label "B". The zeros indicate that "L", "G", "T", "O" and "NR" were not predicted for this instance. <br> <br>
</p>
<h3 align="center"> Track 3: Homophobic lyrics detection track (binary) </h3>

<p>
The objective of this task is to predict if a phrase of a lyrics song contains LGBT+phobic hate speech. This is a binary task (LGBT+phobic (P), not LGBT+phobic (NP)). We define each one of these labels next: <br> <br>

<ul>
<li> LGBT+phobic (P). Lyrics contain hate speech directed against any person whose sexual orientation and/or gender identity differs from cis-heterosexuality. </li>

<li> Not LGBT+phobic (NP). Lyrics are those that do not include any hate speech against the LGBT+ population but do mention this community. </li>
</ul>

In this last track, participants will be able to assign one of the two labels to each tweet, e.g. Tweet X can be assigned the label "P", and Tweet Y can be assigned with label "NP". <br> <br>

Given that each tweet can have one of these tree labels, the output submission must have two columns, first column corresponds to the ID of the tweet and the second column corresponds to your prediction value for each tweet indicating "P" or "NP". E. g. <br> <br>

ID_Track3, "P" - this tweet defined as LGBT+phobic. <br> <br>

ID_Track3, "NP" - this tweet defined as not LGBT+phobic related. <br> <br>
</p>

<h2 align="center"> Site </h2>

Check out the task site <a href="_blank" target="https://sites.google.com/view/homomex/home?authuser=0">here</a>.

<h2 align="center"> Organizers </h2>

<b>Gemma Bel Enguix</b> (II-UNAM, Mexico, gbele@iingen.unam.mx) is a researcher at the Instituto de Ingeniería, UNAM. Ph.D. in linguistics from the Rovira i Virgili University (Tarragona, Catalunya).
<br> <br>

<b>Helena Gómez Adorno</b> (IIMAS-UNAM, Mexico, helena.gomez@iimas.unam.mx) is an associate researcher at Instituto de Investigaciones en Matemáticas Aplicadas y en Sistemas, UNAM. Ph. D. in Computer Science from the Computer Research Center (IPN).
<br> <br>

<b>Juan Vásquez</b> (Boulder Language and Social Technologies Group, University of Colorado Boulder, EEUU, juan.vasquez-1@colorado.edu) is a first-year PhD student.
<br> <br>

<b>Scott Thomas Andersen</b> (Posgrado en Ciencia e Ingeniería de la Computación, Mexico, sthomasen7@gmail.com) is currently pursuing a master's degree in computer science at Instituto de Investigaciones en Matemáticas Aplicadas y en Sistemas, UNAM in Computer Science.
<br> <br>

<b>Sergio Luís Ojeda-Trueba</b> (II-UNAM, Mexico, sojedat@iingen.unam.mx) is a graduate student at Instituto de Ingeniería at the UNAM.
<br> <br>

<b>Hiram Calvo</b> (Centro de Investigación en Computación, Instituto Politécnico Nacional, México, hcalvo@cic.ipn.mx) is a researcher at the Centro de Investigación en Computación, Instituto Politécnico Nacional, México (CIC-IPN) in Mexico.
<br> <br>

<b>Tania Alcántara</b> (Centro de Investigación en Computación, Instituto Politécnico Nacional, Mexico, talcantaram2020@cic.ipn.mx) is currently pursuing a Ph.D. in Computer Science at the Centro de Investigación en Computación, Instituto Politécnico Nacional, México (CIC-IPN) in Mexico.
<br> <br>

<b>Miguel Soto</b> (Centro de Investigación en Computación, Instituto Politécnico Nacional, Mexico, msotoh2021@cic.ipn.mx) is currently pursuing a Ph.D. in Computer Science at Centro de Investigación en Computación, Instituto Politécnico Nacional, México (CIC-IPN) in Mexico.
<br> <br>

<b>Cesar Macias</b> (Centro de Investigación en Computación, Instituto Politécnico Nacional, Mexico, cmaciass2021@cic.ipn.mx) is currently pursuing a Ph.D. in Computer Science at Centro de Investigación en Computación, Instituto Politécnico Nacional, México (CIC-IPN) in Mexico.
<br> <br>

<h2 align="center"> Citing this work </h2>

Citing the HOMO-MEX 2025 shared task.
<pre>
@article{HomoMex24,
  author = {Helena G{'o}mez-Adorno and Gemma Bel-Enguix and Hiran Calvo and Juan V{'a}squez and Scott Thomas Andersen and Sergio Ojeda-Trueba and Tania Alc{'a}ntara and Miguel Soto and Cesar Macias},
  title = {Overview of HOMO-MEX at Iberlef 2024: Hate Speech Detection Towards the Mexican Spanish Speaking LGBT+ Population},
  journal = {Natural Language Processing},
  volume = {73},
  year = {2024},
  issn={1989-7553}
}
</pre>

Citing the HOMO-MEX Twitter dataset
<pre>
@inproceedings{vasquez-etal-2023-homo,
    title = "{HOMO}-{MEX}: A {M}exican {S}panish Annotated Corpus for {LGBT}+phobia Detection on {T}witter",
    author = "V{\'a}squez, Juan  and
      Andersen, Scott Thomas  and
      Bel-enguix, Gemma  and
      G{\'o}mez-adorno, Helena  and
      Ojeda-trueba, Sergio-luis",
    editor = {Chung, Yi-ling  and
      R{{\textbackslash}"ottger}, Paul  and
      Nozza, Debora  and
      Talat, Zeerak  and
      Mostafazadeh Davani, Aida},
    booktitle = "The 7th Workshop on Online Abuse and Harms (WOAH)",
    month = jul,
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.woah-1.20",
    doi = "10.18653/v1/2023.woah-1.20",
    pages = "202--214",
}
</pre>
