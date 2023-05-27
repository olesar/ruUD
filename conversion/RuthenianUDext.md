# Ruthenian corpus tagset

### Инвентарь грамматических тегов Корпуса простой мовы

This document presents a brief description of the part of speech and morphological tagset used for grammatical annotation of the Ruthenian corpus. 
A brief description see below the table.

Created: 21 May 2023  Edited: 21 May 2023


## Universal parts of speech (UPOS)

|UDext|UPOS|XPOS|RNC|AUT|MulTEXT|description(EN)|Example|Status|description(RU)|description(BE)
|---|---|---|---|---|---|---|---|---|---|---|
|NOUN|NOUN|NN|S|Nn|Nc|common noun||UD basic|имя существительное|назоўнік|
||NOUN|NNA|S|Nn|Nc|common noun: semantically animate|_бурмистръ_, _игуменья_, _конь_||:семантически одушевленное|:семантычна адушаўлёны|
||NOUN|NNI|S|Nn|Nc|common noun: inanimate|_присяга_, _поветъ_, _выбиранье_||:неодушевленное|:неадушаўлёны|
|PROPN|PROPN||S|Nn|Np|proper noun||UD basic|имя собственное|імя ўласнае|
||PROPN|NPA|S|Nn|Np|proper noun: semantically animate|_Маркъ_, _Данильевичъ_, _Селява_||:семантически одушевленное|:семантычна адушаўлёнае|
||PROPN|NPI|S|Nn|Np|proper noun: inanimate|_Рига_, _Менскъ_, _Немцы_||:неодушевленное|:неадушаўлёнае|
|INIT|PROPN||INIT|Nn|W|initial letter|_В.Н._|UDext|инициал|ініцыял|
|ADJ|ADJ||A|Aj|A|adjective||UD basic|имя прилагательное|прыметнік|
||ADJ|JJL|A|Aj|A|adjective: plain form|_живый_, _добрый_||:полная форма|:поўная форма|
||ADJ|JJH|A|Aj|A|adjective: short form|_годенъ_, _марковъ_||:краткая форма|:кароткая форма|
||ADJ|JJR|A|Aj|A|adjective: comparative|_высший_, _дорожший_||:сравнительная степень|:параўнальная ступень|
||ADJ|JJS|A|Aj|A|adjective: superlative|_лацнейший_, _наяснейший_||:превосходная степень|:найвышэйшая ступень|
||ADJ|JJ|A|Aj|A|adjective: others|||:другое|:iншае|
|NUM|NUM|CD|NUM|Nm|M|numeral|_четыри_, _4_, _колько_|UD basic|имя числительное|лічэбнік|
|ANUM|ADJ|ORD|ANUM|Aj|A|ordinal numeral|_первый_, _1387-е_|UDext|числительное-прилагательное|лічэбнік-прыметнік|
|AUX|AUX||V|Vb|Va|auxiliary|_быти_, _бы_|UD basic|вспомогательный глагол/частица, выполняющие грамматическую функцию|дапаможны дзеяслоў/часціца|
|VERB|VERB||V|Vb|Vm|verb|_ведати_, _держатися_|UD basic|глагол|дзеяслоў|
||VERB|VBC|V|Vb|Vmi/Vmm|verb: finite|_квитуемъ_, _сталося_||глагол: финитный|:фінітны|
||VERB|VBG|V|Vb|Vmn|verb: infinitive|_ведати_, _держатися_||глагол: инфинитив|:інфінітыў|
||VERB|VBG|V|Vb|Vmg|verb: gerundive|_маючи_, _вернувся_||глагол: деепричастие|:дзеепрыметнік|
||VERB|VBNH|V|Vb|Vmp|verb: short participle|_описано_||:причастие: краткая форма|:прыметнік: кароткая форма|
||VERB|VBNL|V|Vb|Vmp|verb: long participle|_седячихъ_, _купленые_||:причастие: полная форма|:прыметнік: поўная форма|
|PRED|PRAEDIC|VERB|V|Vb|Vm|predicative|_жаль_, _нетъ_, _вольно_|UDext|предикатив|прэдыкатыў|
|PREDPRO|PRAEDICPRO|VERB|V|Vb|Vm|predicative pronoun|_некого_, _нечого_|UDext|местоимение-предикатив|займеннік-прэдыкатыў|
|ADV|ADV||ADV|Av|R|adverb|_честно_, _тогды_|UD basic|наречие|прыслоўе|
|PARENTH|ADV||PARENTH|Av|R|parentheticals||UDext|вводное слово|ўводнае слова|
|PRON|PRON||SPRO|Pn|P|pronoun (nominal)|_она_, _што_|UD basic|местоимение-существительное|займеннік-назоўнік|
||PRON||SPRO|Pn|P|:personal|_ты_, _она_||:личное|:асабісты|
||PRON||SPRO|Pn|P|:relative/interrogative|_хто_, _иже_||:относительное/вопросительное|:адносны/пытальны|
||PRON||SPRO|Pn|P|:negative|_нихто_, _ништо_||:отрицательное|:негатыўны|
||PRON||SPRO|Pn|P|:other|_то_, _се_||:другое|:іншае|
|DET|DET||APRO|Dt|D|determiner (adjectival pronoun)|_мой_, _какий_|UD basic|местоимение-прилагательное|займеннік-прыметнік|
||DET|PRP$|APRO|Dt|D|:personal possessive|_мой_, _какий_||:личное притяжательное|:асабісты пасесіўны|
||DET|WDT|APRO|Dt|D|:relative/interrogative|_какий_, _который_||:относительное/вопросительное|:адносны/пытальны|
||DET|NEG|APRO|Dt|D|:negative|_никакий_, _ничей_||:отрицательное|:негатыўны|
||DET|DT|APRO|Dt|D|:other|_иный_, _такий_||:другое|:іншае|
|ADVPRO|ADVPRO||ADV|Av|R|adverbial pronoun|_гды_|UDext|местоименное наречие|займеннікавае прыслоўе|
|ADP|ADP||PR|Pp|S|preposition/adposition|_въ_, _обаполъ_|UD basic|предлог|прыназоўнік|
|SCONJ|SCONJ||CONJ|Cj|C|subordinating conjunction|_штобы_, _докуле_|UD basic|подчинительный союз|падпарадкавальны злучнік|
|CCONJ|CCONJ||CONJ|Cj|C|coordinating conjunction|_або_, _ани_|UD basic|сочинительный союз|складальны злучнік|
|PART|PART||PART|Pt|Q|particle|_не_, _ведь_|UD basic|частица|часціца|
|INTJ|INTJ||INTJ|Ij|I|interjection|_о_, _аллилуйя_|UD basic|междометие|выклічнік|
|X|X||NONLEX|Yx|X|foreign and non-words|_N_, _ска_|UD basic|не-слова|не-словы|
|SYM|SYM||X|Sy|X|symbol|_%_, _+_|UD basic|символ|сімвал|
|PUNCT|||PUNCT|Zz|Z|punctuation mark|_,_|UD basic|знак препинания|знак прыпынку|

PROPN: определяется по пометам persn, patrn, famn, zoon и в большинстве случаев abbr в поле «Грамматика» НКРЯ|+ существительное - имя собственное|+|(_Иван_, _Москва_, _СССР_); определяется по пометам persn, patrn, famn, zoon и в большинстве случаев abbr в поле «Грамматика»  
INIT: запись вида «заглавная буква с точкой» (_М._, _Р._). В поле «Лемма» инициал не раскрывается; грамматические признаки не указываются в НКРЯ, Abbr=Yes в UDext  
ANUM: _один_ размечается как NUM в UD, остальные как ADJ  
PRED: see the [list](https://github.com/olesar/Ruthenian/blob/main/wordlists/praedicatives.txt) of most frequent praedicatives  
PARENTH: parenthetically used discoursive markers  
PRON: see the [list](https://github.com/olesar/Ruthenian/blob/main/wordlists/pron_list.txt)  
DET: see the [list](https://github.com/olesar/Ruthenian/blob/main/wordlists/det_list.txt)  
ADP: see the [list](https://github.com/olesar/Ruthenian/blob/main/wordlists/adp_list.txt)  
SCONJ: see the [list](https://github.com/olesar/Ruthenian/blob/main/wordlists/sconj_list.txt); this is a default category if converting conjunctions from other inventories  
CCONJ: see the [list](https://github.com/olesar/Ruthenian/blob/main/wordlists/cconj_list.txt)  

Punctuation mark XPOS:
-PERIOD-  .?!  
-COMMA- ,;  
-QUOT-  «»"„“  
-COLON- :  
-DASH-  —-  
-HYPH-  -  
-LBR- ([{  
-RBR- )]}  
-NFP- other (…//...)
