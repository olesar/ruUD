# Lithuanian treebank

Annotated manually using the Morphological Annotator by CCL, Vytautas Magnus University (http://tekstynas.vdu.lt/).
A pilot version which includes news and an essay by Tomas Venclova is available here.


### Grammatical features
|Lithuanian term|KLC tag|UD FEAT|RNC tag|English term|
|---|---|---|---|---|
|<td colspan=4>Kalbos dalis / Part of speech</td>|
|daiktavardis|dkt.|NOUN|S|noun|
|būdvardis|bdv.|ADJ|A|adjective|
|skaitvardis|sktv.|NUM\|ADJ|NUM\|ANUM|numeral|
|įvardis|įv.|PRON|SPRO\|APRO|pronoun|
|veiksmažodis|vksm.|VERB|V|verb|
|prieveiksmis|prv.|ADV|ADV\|ADVPRO\|PARENTH|adverb|
||||PRAEDIC\|PRAEDICPRO||
|jaustukas|jst.|INTJ|INTJ|interjection|
|ištiktukas|išt.|INTJ|INTJ|onomatopoeic interjection|
|dalelytė|dll.|VERB,VerbForm=Part|V,partcp|particle|
|prielinsknis|prl.|ADP|PR|prielinsknis|
|jungtukas|jng.|CONJ|CONJ|switch|
|akronimas|akronim.|Abbr=Yes|abbr|acronym|
|sutrumpinimas|sutr.|Abbr=Yes|abbr|shorthand|
|<td colspan=4>Daiktavardžių rūšys / Noun subcategories
|tikrinis|tikr.|PROPN|S,propn|proper noun|
|bendrinis| |||common noun|
|<td colspan=4>Veiksmažodis ir jo formos / Verb forms</td>
|bendratis|bendr.|VerbForm=Inf|inf|infinitive|
|dalyvis|dlv.|VerbForm=Part|partcp|participant|
|padalyvis|pad.|VerbForm=ConvSSubj|partcp,ger,ssubj|the half|
|pusdalyvis|pusd.|VerbForm=ConvDSubj|partcp,ger,dsubj|participle|
|būdinys|būdn.|VerbForm=ConvManner|partcp,ger,manner|manner of action participle|
|<td colspan=4>Mood</td>
|tiesioginė nuosaka|tiesiog. n.|Mood=Ind|indic|indicative mood|
|liepiamoji nuosaka|liep. n.|Mood=Imp|imper|imperative mood|
|tariamoji nuosaka|tar. n.|Mood=Cnd|cond|conditional mood|
|<td colspan=4>Skaitvardžiai / Numeral subcategories</td>
|kiekinis|kiek.|NumType=Card|NUM,card|cardinal|
|kelintinis|kelint.|NumType=Ord|ANUM,ord|ordinal|
|dauginis|daugin.|NumType=Mult|NUM,mult|multiple|
|kuopinis|kuopin.|NumType=Coll|NUM,collect|collective|
|<td colspan=4>Apibrėžtumas / Adjective forms</td>
|įvardžiuotinis|įvardž.|Definite=Def|def|pronominal (definite)|
|neįvardžiuotinis|neįvardž.|Definite=Ind|indef|indefinite|
|<td colspan=4>Sangrąžiškumas / Reflexivity</td>
|sangrąžinis|sngr.|Reflex=Yes|refl|reflexive|
|nesangrąžinis|nesngr.|Reflex=No||non-reflexive|
|<td colspan=4>Rūšis / Voice</td>
|veikiamoji rūšis|veik. r.|Voice=Act|act|active voice voice|
|neveikiamoji rūšis|neveik. r.|Voice=Pass|pass|passive voice|
|neveikiamoji rūšis|neveik. r.|Voice=Mid|med|middle voice|
|reikiamybės|reik.|Voice=Deb|debit|debitive (necessity)|
|<td colspan=4>Laikas / Tense</td>
|esamasis laikas|es. l.|Tense=Pres|praes|present tense|
|būtasis laikas|būt. l.|Tense=Past|praet|past tense|
|būtasis kartinis laikas|būt. k. l.|Tense=PastSimp|praet|past simple tense|
|būtasis dažninis laikas|būt. d. l.|Tense=PastIter|past,hab|past iterative (frequentative, habitual) tense|
|būsimasis laikas|būs. l.|Tense=Fut|fut|future tense|
|||Tense=PresHab|praes,hab|present tense|
|<td colspan=4>Laipsnis / Degree</td>
|nelyginamasis laipsnis|nelygin. l.|Degree=Pos||positive degree|
|aukštesnysis laipsnis|aukšt. l.|Degree=Cmp|comp|comparative degree|
|aukščiausiasis laipsnis|aukšč. l.|Degree=Sup|super|superlative degree|
|<td colspan=4>Giminė / Gender</td>
|moteriškoji giminė|mot. g.|Gender=Fem|f|feminine gender|
|vyriškoji giminė|vyr. g.|Gender=Masc|m|masculine gender|
|bevardė giminė|bev. g.|Gender=Neut|n|neuter gender|
|bendroji giminė|bendr. g.|Gender=Com|mf|common gender (rare form)|
|<td colspan=4>Skaičius / Number</td>
|vienaskaita|vns.|Number=Sing|sg|singular number|
|daugiskaita|dgs.|Number=Plur|pl|plural number|
|dviskaita|dvisk.|Number=Dual|du|dual number|
|<td colspan=4>Linksnis / Case</td>
|vardininkas|V.|Case=Nom|nom|nominative|
|kilmininkas|K.|Case=Gen|gen|genitive|
|naudininkas|N.|Case=Dat|dat|dative|
|galininkas|G.|Case=Acc|acc|accusative|
|įnagininkas|Įn.|Case=Ins|ins|instrumental|
|vietininkas|Vt.|Case=Loc|loc|locative|
|šauksmininkas|Š.|Case=Voc|voc|vocative|
|iliatyvas|Il.|Case=Il|ill|illative|
|<td colspan=4>Asmuo / Person</td>
|pirmasis asmuo|1 asm.|Person=1|1p|first person|
|antrasis asmuo|2 asm.|Person=2|2p|second person|
|trečiasis asmuo|3 asm.|Person=3|3p|third person|
|<td colspan=4>Teigiamumas / Polarity</td>
|teigiamas|teig.|Polarity=Pos||positive polarity (no negation)|
|neigiamas|neig.|Polarity=Neg|neg|negative polarity|
|<td colspan=4>Romėniški skaičiai / Numeral Form</td>
||rom. sk.|NumForm=Digit|ciph|roman numerals|
|<td colspan=4>Stabiliosios frazės / Phrase types</td>
||idprl.|\*fixed_ADP\*|PR,fixed||
||idjngt.|\*fixed_CONJ\*|CONJ,fixed||
||idPS|\*fixed_PS\*|PS,fixed||

<br/> === Machine-readable metadata ====<br/>
Documentation status: stub <br/>
Data source: automatic <br/>
Data available since: UD v2.1 <br/>
License: CC BY-SA 4.0 <br/>
Genre: nonfiction news <br/>
Contributors: Lyashevskaya, Olga; Sichinava, Dmitry <br/>
Contact: olesar@yandex.ru <br/>
 ========================================
