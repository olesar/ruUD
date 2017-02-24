# Lithuanian treebank

Annotated manually using the Morphological Annotator by CCL, Vytautas Magnus University (http://tekstynas.vdu.lt/).
A pilot version which includes news and an essay by Tomas Venclova is available here.

### Grammatical features
|Category|Lithuanian term|KLC tag|UD FEAT|RNC tag|English term|
|---|---|---|---|---|---|
|Kalbos dalis|daiktavardis|dkt.|NOUN|S|noun|
||būdvardis|bdv.|ADJ|A|adjective|
||skaitvardis|sktv.|NUM|ANUM|NUM|numeral|
||įvardis|įv.|PRON|S-PRO|A-PRO|pronoun|
||veiksmažodis|vksm.|VERB|V.|verb|
||prieveiksmis|prv.|ADV|ADV|adverb|
||jaustukas|jst.|INTJ|INTJ|interjection|
||ištiktukas|išt.|INTJ|INTJ|onomatopoeic interjection|
||dalelytė|dll.|PART|V,partcp|particle|
||prielinsknis|prl.|ADP|PR|prielinsknis|
||jungtukas|jng.|CONJ|CONJ|switch|
||akronimas|akronim.|Abbr=Yes|abbr|acronym|
||sutrumpinimas|sutr.|Abbr=Yes|abbr|shorthand|
|Daiktavardžių rūšys|tikrinis|tikr.|PROPN|S,propn|proper noun|
||bendrinis| |||common noun|
|Veiksmažodis ir jo formos|bendratis|bendr.|VerbForm=Inf|inf|infinitive|
||dalyvis|dlv.|VerbForm=Part|partcp|participant|
||padalyvis|pad.|VerbForm=ConvSSubj|partcp,ger,ssubj|the half|
||pusdalyvis|pusd.|VerbForm=ConvDSubj|partcp,ger,dsubj|participle|
||būdinys|būdn.|VerbForm=ConvManner|partcp,ger,manner|manner of action participle|
||tiesioginė nuosaka|tiesiog. n.|Mood=Ind|indic|indicative mood|
||liepiamoji nuosaka|liep. n.|Mood=Imp|imper|imperative mood|
||tariamoji nuosaka|tar. n.|Mood=Cnd|cond|conditional mood|
|Skaitvardžiai|kiekinis|kiek.|NumType=Card|NUM,card|cardinal|
||kelintinis|kelint.|NumType=Ord|ANUM,ord|ordinal|
||dauginis|daugin.|NumType=Mult|NUM,mult|multiple|
||kuopinis|kuopin.|NumType=Coll|NUM,collect|collective|
|Apibrėžtumas|įvardžiuotinis|įvardž.|Definite=Def|def|pronominal (definite)|
||neįvardžiuotinis|neįvardž.|Definite=Ind|idf|neįvardžiuotinis|
|Sangrąžiškumas|sangrąžinis|sngr.|Reflex=Yes|refl|reflexive|
||nesangrąžinis|nesngr.|Reflex=No||nesangrąžinis|
|Rūšis|veikiamoji rūšis|veik. r.|Voice=Act|act|active voice|
||neveikiamoji rūšis|neveik. r.|Voice=Pass|pass|passive|
||reikiamybės|reik.|Voice=Deb|debit|necessity|
|Laikas|esamasis laikas|es. l.|Tense=Pres|praes|present tense|
||būtasis kartinis laikas|būt. k. l.|Tense=PastSimp|praet|past simple tense|
||būtasis dažninis laikas|būt. d. l.|Tense=PastIter|past,hab|past iterative (frequentative, habitual) tense|
||būsimasis laikas|būs. l.|Tense=Fut|fut|future tense|
||būtasis laikas|būt. l.|Tense=Past|praet|past tense|
|Laipsnis|nelyginamasis laipsnis|nelygin. l.|Degree=Pos||positive degree|
||aukštesnysis laipsnis|aukšt. l.|Degree=Cmp|comp|comparative degree|
||aukščiausiasis laipsnis|aukšč. l.|Degree=Sup|super|superlative degree|
|Giminė|moteriškoji giminė|mot. g.|Gender=Fem|f|feminine gender|
||vyriškoji giminė|vyr. g.|Gender=Masc|m|masculine gender|
||bevardė giminė|bev. g.|Gender=Neut|n|neuter gender|
||bendroji giminė|bendr. g.|Gender=Com|mf|common gender (rare form)|
|Skaičius|vienaskaita|vns.|Number=Sing|sg|singular number|
||daugiskaita|dgs.|Number=Plur|pl|plural number|
||dviskaita|dvisk.|Number=Dual|du|dual number|
|Linksnis|vardininkas|V.|Case=Nom|nom|nominative|
||kilmininkas|K.|Case=Gen|gen|genitive|
||naudininkas|N.|Case=Dat|dat|dative|
||galininkas|G.|Case=Acc|acc|accusative|
||įnagininkas|Įn.|Case=Ins|ins|instrumental|
||vietininkas|Vt.|Case=Loc|loc|locative|
||šauksmininkas|Š.|Case=Voc|voc|vocative|
||iliatyvas|Il.|Case=Il|ill|illative|
|Asmuo|pirmasis asmuo|1 asm.|Person=1|1p|first person|
||antrasis asmuo|2 asm.|Person=2|2p|second person|
||trečiasis asmuo|3 asm.|Person=3|3p|third person|
|Teigiamumas, neigiamumas|teigiamas|teig.|Polarity=Pos||positive polarity (no negation)|
||neigiamas|neig.|Polarity=Neg|neg|negative polarity|
|Romėniški skaičiai| |rom. sk.|NumForm=Digit|ciph|roman numerals|
|Stabiliosios frazės| |idprl.|*fixed_ADP*|PR,fixed||
|||idjngt.|*fixed_CONJ*|CONJ,fixed||
|||idPS|*fixed_PS*|PS,fixed||

=== Machine-readable metadata =================================================
Documentation status: stub
Data source: automatic
Data available since: UD v2.1
License: CC BY-SA 4.0
Genre: nonfiction news
Contributors: Lyashevskaya, Olga; Sichinava, Dmitry
Contact: olesar@yandex.ru
===============================================================================