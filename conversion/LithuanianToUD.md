# Lithuanian: DLKT-MulText-East to to UD 2.0 conversion table 

Created: 06 Jan 2019

## Parts of speech (UPOS)

||P|DLKT|UD|description|
|---|---|---|---|---|
|➚|1|N|NOUN|noun|
|➘|1|N|PROPN|proper noun|
|➚|1|Y|PROPN|abbreviation|
|➚|1|V|VERB|verb|
|➘|1|V|AUX|auxiliary verb|
|➚|1|A|ADJ|adjective|
|➘|1|A|DET|determiner|
|+|1|P|PRON|pronoun|
|+|1|R|ADV|adverb|
|+|1|S|ADP|preposition|
|➚|1|C|CCONJ|conjunction|
|➘|1|C|SCONJ|conjunction|
|+|1|M|NUM|numeral|
|+|1|Q|PART|particle|
|➘|1|I|INTJ|interjection|
|➚|1|O|INTJ|onomatopoeia|
|+|1|X|X|residual|
|➚|1|T|PUNCT|punctuation|
|➘|1|T|SYM|symbol|

## Features (FEAT)		

### Noun
Number of codes: 7
Examples: Lietuvai,"Npfsdng"; vasarą,"Ncfsan-"

||P|DLKT|UD|Value|
|---|---|---|---|---|
|:|1|N|NOUN/PROPN|Noun|
|||||Type|
||2|c|NOUN|common|
||2|p|PROPN|proper|
|||||Gender|
||3|c|Gender=Com|common|
||3|f|Gender=Fem|feminine|
||3|m|Gender=Masc|masculine|
|||-||irrelevant|
|||||Number|
||4|p|Number=Plur|plural|
||4|s|Number=Sing|singular|
||4|d|Number=Dual|dual|
||4|-||irrelevant|
|||||Case|
||5|n|Case=Nom|nominative|
||5|g|Case=Gen|genitive|
||5|d|Case=Dat|dative|
||5|a|Case=Acc|accusative|
||5|i|Case=Ins|instrumental|
||5|l|Case=Loc|locative|
||5|v|Case=Voc|vocative|
||5|x|Case=Ill|illative|
||5|-||irrelevant|
|||||Reflexiveness|
||6|y|Reflex=Yes|yes|
||6|n||no|
|||||Name|
|-|7|f||first name|
|-|7|s||surname|
|-|7|g||geographic name|
|-|7|-||irrelevant|

### Verb
Number of codes: 14
Examples: rezervuoju,"Vgmp1s--n--ni-"; paliktu,"Vgps-smpnnin-p"

||P|DLKT|UD|Value|
|---|---|---|---|---|
|:|1|V|VERB|Verb|
|||||Type|
||2|g||general|
|||||VForm|
||3|i|VerbForm=Inf|infinitive|
||3|m|VerbForm=Fin|main (finite)|
||3|p|VerbForm=Part|particle|
||3|a|VerbForm=PartPad|adverbial participle|
||3|h|VerbForm=PartPus|half particle|
|-|3|s|VerbForm=PartPad?|adverbial participle2|
|||||Tense|
||4|p|Tense=Pres|present|
||4|a|Tense=PastSimp|simple past|
||4|s|Tense=Past|past tense|
||4|q|Tense=PastIter|past frequentative|
||4|f|Tense=Fut|future|
|-|||Tense=PresHab|present habilit|
|||||Person|
||5|1|Person=1|first|
||5|2|Person=2|second|
||5|3|Person=3|third|
|||-||irrelevant|
|||||Number|
||6|p|Number=Plur|plural|
||6|s|Number=Sing|singular|
||6|d|Number=Dual|dual|
|||||Gender|
||7|f|Gender=Fem|feminine|
||7|m|Gender=Masc|masculine|
||7|n|Gender=Neut|neuter|
||7|-||irrelevant|
|||||Voice|
||8|a|Voice=Act|active|
||8|p|Voice=Pass|passive|
||8|n|Voice=Necess|necessity|
||8|-||irrelevant|
||||Negative polarity|
||9|y|Polarity=Neg|yes|
||9|n|Polarity=Yes|no|
|||||Defineteness|
||10|y|Definite=Def|yes|
||10|n|Definite=Ind|no|
|||||Case|
||11|n|Case=Nom|nominative|
||11|g|Case=Gen|genitive|
||11|d|Case=Dat|dative|
||11|a|Case=Acc|accusative|
||11|i|Case=Ins|instrumental|
||11|l|Case=Loc|locative|
||11|v|Case=Voc|vocative|
||11|x|Case=Ill|illiative|
||11|-||irrelevant|
|||||Reflexiveness|
||12|y|Reflex=Yes|yes|
|-|12|n||no|
|||||Mood|
||13|i|Mood=Ind|indicative|
||13|s|Mood=Cnd|subjunctive|
||13|m|Mood=Imp|imperative|
||13|-||irrelevant|
|||||Degree|
||14|p|Degree=Pos|positive|
||14|c|Degree=Cmp|comparative|
||14|s|Degree=Sup|superlative|
||14|-||irrelevant|

### Adjective
Number of codes: 7
Examples: svarbu,"Agpn--n"; gražiausius,"Agsmpan"

||P|DLKT|UD|Value|
|---|---|---|---|---|
|:|1|A|ADJ|Adjective|
|||||Type|
|-|2|g||general|
|||||Degree|
||3|p|Degree=Pos|positive|
||3|c|Degree=Cmp|comparative|
||3|s|Degree=Sup|superlative|
|?|3|d|Derivation=Dimin|diminutive|
||3|-||irrelevant
|||||Gender|
||4|f|Gender=Fem|feminine|
||4|m|Gender=Masc|masculine|
||4|n|Gender=Neut|neuter|
||4|-||irrelevant|
|||||Number|
||5|p|Number=Plur|plural|
||5|s|Number=Sing|singular|
||5|d|Number=Dual|dual|
||5|-||irrelevant|
|||||Case|
||6|n|Case=Nom|nominative|
||6|g|Case=Gen|genitive|
||6|d|Case=Dat|dative|
||6|a|Case=Acc|accusative|
||6|i|Case=Ins|instrumental|
||6|l|Case=Loc|locative|
||6|v|Case=Voc|vocative|
||6|x|Case=Ill|illative|
||6|-||irrelevant|
|||||Defineteness|
||7|y|Definite=Def|yes|
||7|n|Definite=Ind|no|

### Pronoun
Number of codes: 6
Examples: visoks,"Pgmpin"; man,"Pg-sdn"

||P|DLKT|UD|Value|
|---|---|---|---|---|
|:|1|P|PRON|Pronoun|
||||Type|
|-|2|g||general|
|||||Gender|
||3|f|Gender=Fem|feminine|
||3|m|Gender=Masc|masculine|
||3|n|Gender=Neut|neuter|
||3|-||irrelevant|
|||||Number|
||4|p|Number=Plur|plural|
||4|s|Number=Sing|singular|
||4|d|Number=Dual|dual|
||4|-||irrelevant|
|||||Case|
||5|n|Case=Nom|nominative|
||5|g|Case=Gen|genitive|
||5|d|Case=Dat|dative|
||5|a|Case=Acc|accusative|
||5|i|Case=Ins|instrumental|
||5|l|Case=Loc|locative|
||5|v|Case=Voc|vocative|
||5|x|Case=Ill|illative|
||5|-||irrelevant|
|||||Defineteness|
||6|y|Definite=Def|yes|
||6|n|Definite=Ind|no|
||6|-||irrelevant|

### Numeral
Number of codes: 7
Examples: penkiom,"Mcf-iln" / "Mcf-dln"; 10,"M----d-"

||P|DLKT|UD|Value|
|---|---|---|---|---|
|:|1|M|NUM|Numeral|
|||||Type|
||2|c|NumType=Card|cardinal|
||2|o|NumType=Ord|ordinal|
||2|l|NumType=Sets|collect|
||2|m|NumType=Mult|multiple|
||2|-||irrelevant|
|||||Gender|
||3|f|Gender=Fem|feminine|
||3|m|Gender=Masc|masculine|
||3|n|Gender=Neut|neuter|
||3|-||irrelevant|
|||||Number|
||4|p|Number=Plur|plural|
||4|s|Number=Sing|singular|
||4|-||irrelevant|
|||||Case|
||5|n|Case=Nom|nominative|
||5|g|Case=Gen|genitive|
||5|d|Case=Dat|dative|
||5|a|Case=Acc|accusative|
||5|i|Case=Ins|instrumental|
||5|l|Case=Loc|locative|
||5|v|Case=Voc|vocative|
||5|x|Case=Ill|illative|
||5|-||irrelevant|
|||||Form|
||6|d|NumForm=Digit|digit|
||6|r|NumForm=Roman|roman|
||6|l|NumForm=Letter|letter|
|?|6|m||m-form|
|||||Defineteness|
||7|y|Definite=Def|yes|
||7|n|Definite=Ind|no|
||7|-||irrelevant|

### Adverb
Number of codes: 3
Examples: apskritai,"Rgp"; gerai,"Rgc"

||P|DLKT|UD|Value|
|---|---|---|---|---|
|:|1|R|ADV|Adverb|
|||||Type|
|-|2|g||general|
|||||Degree|
||3|p|Degree=Pos|positive|
||3|c|Degree=Cmp|comparative|
||3|s|Degree=Sup|superlative|
|?|3|d|Derivation=Dimin|diminutive|
||3|-||irrelevant

### Preposition
Number of codes: 3
Examples: su,"Sgi"; po,"Sgg"

||P|DLKT|UD|Value|
|---|---|---|---|---|
|:|1|S|ADP|Preposition|
|||||Type|
|-|2|g||general|
|||||Case|
||3|g|Case=Gen|genitive|
||3|d|Case=Dat|dative|
||3|a|Case=Acc|accusative|
||3|i|Case=Ins|instrumental|

### Conjunction
Number of codes: 2
Examples: būtent,"Cg"; ir,"Cg"

||P|DLKT|UD|Value|
|---|---|---|---|---|
|:|1|C|CCONJ/SCONJ|Conjunction|
|||||Type|
|-|2|g||general|

### Particle
Number of codes: 2
Examples: pat,"Qg"; gal,"Qg"

||P|DLKT|UD|Value|
|---|---|---|---|---|
|:|1|Q|PART|Particle|
|||||Type|
|-|2|g||general|

### Interjection/Onomatopoeia
Number of codes: 2
Examples: na,"Ig"; va,"Ig" (Interjection); dzin, "Og"; cypt, "Og" (Onomatopoeia)

||P|DLKT|UD|Value|
|---|---|---|---|---|
|:|1|I|INTJ|Interjection/Onomatopoeia|
|||||Type|
|-|2|g||general|

### Abbreviation
Number of codes: 2
Examples: t.t.,"Ys"; TV,"Ya"

||P|DLKT|UD|Value|
|---|---|---|---|---|
|:|0|Y|PROPN|Abbreviation|
|||||Type|
||2|s|Abbr=Cut|shortening|
||2|a|Abbr=Yes|acronym|

### Others
Number of codes: 2
Examples: the, "Df"; http://www.vdu.lt, "De"

||P|DLKT|UD|Value|
|---|---|---|---|---|
|:|1|D|X|Residual|
|||||Type|
||2|f||foreign|
||2|t||typo|
||2|p||segmentation|
||2|h||tag|
||2|l||link|
||2|e||e-mail addresses|

### Punctuation
Number of codes: 2
Examples: ",","Tc"; "?","Tq"

||P|DLKT|UD|Value|
|---|---|---|---|---|
|:|1|T|PUNCT|Punctuation|
|||||Type|
||2|p||full stop/period (.)|
||2|c||comma (,)|
||2|s||semicolon (;)|
||2|n||colon (:)|
||2|q||question mark (?)|
||2|e||exclamation mark (!)|
||2|i||ellipsis (...)|
||2|h||dash, minus (- – —)|
||2|l||opening bracket ([{|
||2|r||closing bracket )]}|
||2|u||quotation mark ("'„“)|
||2|t||slash, stroke|
||2|x||other marks, symbols (\*%^$)|
