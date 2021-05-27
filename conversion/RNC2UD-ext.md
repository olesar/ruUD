# Russian National Corpus tagset (main corpus): conversion table to UD 2.0

Created: 01 Nov 2020  Edited: 03 Feb 2021

## Universal parts of speech (UPOS)

|Status|UDext|RNC|UD|description(RUS)|description(ENG)|AUT Aranea|MulTEXT|
|---|---|---|---|---|---|---|---|
|~|NOUN|S|NOUN|существительное (_яблоня_, _лошадь_, _корпус_, _вечность_)|noun|Nn|Nc|
|+|PROPN|S|PROPN|+ существительное - имя собственное|(_Иван_, _Москва_, _СССР_); определяется по пометам persn, patrn, famn, zoon и в большинстве случаев abbr в поле «Грамматика» НКРЯ|proper noun|Nn|Np|
|-|PROPN|INIT|PROPN|инициал (запись вида «заглавная буква с точкой» (_М._, _Р._). В поле «Лемма» инициал не раскрывается; грамматические признаки не указываются в НКРЯ, Abbr=Yes в UDext)|proper noun (initial letter)|Nn|W|
|=|ADJ|A|ADJ|прилагательное (_коричневый_, _таинственный_, _морской_)|adjective|Aj|A|
|~|NUM|NUM|NUM|числительное (_четыре_, _4_, _много_)|numeral|Nm|M|
|!|ANUM|ANUM|ADJ|числительное-прилагательное (_седьмой_, _восьмидесятый_); NB за исключением _один_ (размечается как NUM в UD)|ordinal numeral|Aj|A|
|~|VERB|V|VERB|глагол (_пользоваться_, _обрабатывать_)|verb|Vb|Vm|
|+|AUX|V|AUX|вспомогательный глагол _быть_ (выполняющий функции грамматического показателя)|auxiliary|Vb|Va|
|!|PRED|PRAEDIC|VERB|предикатив (_жаль_, _хорошо_, _пора_), см. [список](https://github.com/olesar/ruUD/blob/master/praedic_list.md)|predicative|||
|!|PREDPRO|PRAEDICPRO|VERB|местоимение-предикатив (_некого_, _нечего_)|predicative pronoun|||
|=|ADV|ADV|ADV|наречие (_сгоряча_, _очень_)|adverb|Av|R|
|!|PARENTH|PARENTH|ADV|вводное слово (_кстати_, _по-моему_)|parenthetically used discoursive markers|Av|R|
|=|PRON|SPRO|PRON|местоимение-существительное (_она_, _что_), см. [список](https://github.com/olesar/ruUD/blob/master/pron_list.md)|pronoun (as noun)|Pn|P|
|=|DET|APRO|DET|местоимение-прилагательное (_этот_, _твой_); NB за исключением _который_ (размечается как PRON), см. [список](https://github.com/olesar/ruUD/blob/master/det_list.md)|adjectival pronoun/determiner|Dt|D|
|!|ADVPRO|ADVPRO|ADV||местоименное наречие (_где_, _вот_)	adverbial pronoun|Av|R|
|=|ADP|PR|ADP|предлог (_под_, _напротив_)|preposition/adposition|Pp|S|
|~|SCONJ|CONJ|SCONJ|союз (_что_, _чтобы_); при конвертации по умолчанию подчинительный|subordinating conjunction|Cj|C|
|+|CCONJ|CONJ|CCONJ|+ сочинительный союз (_и_, _но_), см. [список](https://github.com/olesar/ruUD/blob/master/conj_list.md)|coordinating conjunction|Cj|C|
|=|PART|PART|PART|частица (_бы_, _же_, _пусть_)|particle|Pt|Q|
|=|INTJ|INTJ|INTJ|междометие (_увы_, _батюшки_)|interjection|Ij|I|
|=|X|NONLEX|X|не-слова (_шшетт_, _bolo_)|foreign and non-words |Yx|X|
|+|SYM||SYM|символ (_%_, _$_)|symbol|Sy||
|+|PUNCT||PUNCT|знак препинания|punctuation mark|Zz||

Легенда:  
 = точное соответствие (NB отдельные лексические несоответствия)  
 ~ дефолтное соответствие: классы в целом совпадают, с точностью до выделения новых частеречных подклассов и точечных лексических несоответствий  
 \+ добавление подкласса в базовом UD  
 ! добавление подкласса в UDext  
 \- нет соответствия в UD   
 \* нет соответствия в НКРЯ   
 не помечены признаки, которые пока не используются в UD


## Grammatical features (FEAT)

|Status|UDext|RNC|UD|description(RUS)|description(ENG)|MulTEXT|
|---|---|---|---|---|---|---|
|=|Gender=Masc|m|Gender=Masc|мужской род (_работник_, _стол_)|masculine gender|2:m|
|=|Gender=Fem|f|Gender=Fem|женский род (_работница_, _табуретка_)|feminine gender|2:f|
|=|Gender=Neut|n|Gender=Neut|средний род (_животное_, _озеро_)|neuter gender|2:n|
|!|Gender=Com|mf|Gender=Masc|«общий род» (_задира_, _пьяница_); в большинстве случаев приравнивание к м. р. не будет порождать ошибки|common gender (the feature Gender=Com not in use in basic UD)|2:c|
|=|Animacy=Anim|anim|Animacy=Anim|одушевленность (_человек_, _ангел_, _утопленник_)|animate|5:y|
|=|Animacy=Inan|inan|Animacy=Inan|неодушевленность (_рука_, _облако_, _культура_)|inanimate|5:n|
|=|Number=Sing|sg|Number=Sing|единственное число (_яблоко_, _гордость_)|singular number|3:s|
|=|Number=Plur|pl|Number=Plur|множественное число (_яблоки_, _ножницы_, _детишки_)|plural number|3:p|
|=|Number=Count|adnum|Number=Count|счётная форма (_два часа́_, _три шара́_)|adnumeral form (NB ignore sg in RNC)||
|=|Case=Nom|nom|Case=Nom|именительный падеж (_голова_, _сын_, _степь_, _сани_, _который_)|Nominative case|4:n|
|=|Case=Gen|gen|Case=Gen|родительный падеж (_головы_, _сына_, _степи_, _саней_, _которого_)|Genitive case|4:g|
|=|Case=Par|gen2|Case=Par|второй родительный падеж (_чашка чаю_)|Partitive case|6:p|
|=|Case=Dat|dat|Case=Dat|дательный падеж (_голове_, _сыну_, _степи_, _саням_, _которому_)|Dative case|4:d|
|=|Case=Acc|acc|Case=Acc|винительный падеж (_голову_, _сына_, _степь_, _сани_, _который/которого_)|Accusative case|4:a|
|=|Case=Ins|ins|Case=Ins|творительный падеж (_головой_, _сыном_, _степью_, _санями_, _которым_)|Instrumental case|4:i|
|=|Case=Loc|loc|Case=Loc|предложный падеж ([_о_] _голове_, _сыне_, _степи_, _санях_, _котором_)|Locative case|4:l|
|=|Case=Voc|voc|Case=Voc|звательная форма (_Господи_, _Серёж_, _ребят_)|Vocative case|4:v|
|-|Case=Dat|dat2|Case=Dat|дистрибутивный дательный ([_по_] _многу_, _нескольку_, _стольку_)|second Dative case||
|!|Case=Acc2|acc2|Case=Nom|второй винительный падеж (_постричься в монахи_; _по два человека_)|second Accusative case (in UD is treated as Nominative, still animate)||
|!|Case=Loc2|loc2|Case=Loc|второй предложный падеж (_в лесу_, _на оси́_)|second Locative case|6:l|
|=|Variant=Short|brev|Variant=Short|краткая форма (_высок_, _нежна_, _прочны_, _рад_)|short form|6:s|
|-||plen||полная форма (_высокий_, _нежная_, _прочные_, _морской_)|full form (Variant=Long not in use)|6:f|
|=|Degree=Pos||Degree=Pos|позитивная степень (_глубокий_); присваивается всем формам прилагательных, наречий и предикативов, не имеющих сравнительной или превосходной степени|positive, first degree|2:p|
|=|Degree=Cmp|comp|Degree=Cmp|сравнительная степень (_глубже_)|comparative degree|2:c|
|!|Degree=Cmp2|comp2|Degree=Cmp|форма «по+сравнительная степень» (_поглубже_)|second comparative degree (_po_ + comparative)|2:c|
|=|Degree=Sup|supr|Degree=Sup|превосходная степень (_глубочайший_); NB в НКРЯ присутствует не во всех корпусах и лемматизируется по образцу _глубочайший_, должна быть различена с позитивной степенью|superlative degree	|2:s|
|=|Aspect=Perf|pf|Aspect=Perf|совершенный вид (_пошёл_, _встречу_)|perfective aspect|9:e|
|=|Aspect=Imp|ipf|Aspect=Imp|несовершенный вид (_ходил_, _встречаю_)|imperfective aspect|9:p|
|!|Transit=Intr|intr||непереходность (_ходить_, _вариться_)|intransitive verb|
|!|Transit=Tran|tran||переходность (_вести_, _варить_)|transitive verb|
|=|Voice=Act|act|Voice=Act|действительный залог (_разрушил_, _разрушивший_)|active voice|7:a|
|=|Voice=Pass|pass|Voice=Pass|страдательный залог (только у причастий: _разрушаемый_, _разрушенный_)|passive voice|7:p|
|=|Voice=Mid|med|Voice=Mid|медиальный, или средний залог (глагольные формы на _-ся_: _разрушился_ и т.п.)|middle voice|7:m|
|=|VerbForm=Inf|inf|VerbForm=Inf|инфинитив (_украшать_)|infinitive|2:n|
|\*|VerbForm=Fin||VerbForm=Fin|финитная форма; в НКРЯ отсутствует, присваивается по умолчанию всем формам, не являющимся инфинитивом, причастием и деепричастием|finite verb||
|=|VerbForm=Part|partcp|VerbForm=Part|причастие (_украшенный_)|participle|2:p|
|=|VerbForm=Conv|ger|VerbForm=Conv|деепричастие (_украшая_)|gerundive (converb)|2:g|
|=|Mood=Ind|indic|Mood=Ind|изъявительное наклонение (_украшаю_, _украшал_, _украшу_)|indicative mood|2:i|
|=|Mood=Imp|imper|Mood=Imp|повелительное наклонение (_украшай_)|imperative mood|2:m|
|!|Mood=Imp2|imper2|Mood=Imp|форма повелительного наклонения 1 л. мн. ч. на -те (_идемте_)|second imperative (imperative on _-мте_)|2:m|
|=|Mood=Cnd|cond|Mood=Cnd|сослагательное наклонение (_бы_, _б_, _чтобы_)|indicative mood|2:c|
|=|Tense=Past|praet|Tense=Past|прошедшее время (_украшали_, _украшавший_, _украсив_)|past tense|3:s|
|=|Tense=Pres|praes|Tense=Pres|настоящее время (_украшаем_, _украшающий_, _украшая_)|present tense|3:p|
|=|Tense=Fut|fut|Tense=Fut|будущее время (_украсим_); у глаголов несовершенного вида сложная форма размечается в два слова как _буду_ + инфинитив|future tense|3:f|
|=|Person=1|1p|Person=1|первое лицо (_украшаю_)|first person|4:1|
|=|Person=2|2p|Person=2|второе лицо (_украшаешь_)|second person|4:2|
|=|Person=3|3p|Person=3|третье лицо (_украшает_)|third person|4:3|
|\*|Polarity=Yes||Polarity=Yes|отрицательная частица, глагол и т.д.|negative polarity|
|\*|PronType=Prs||PronType=Pers|личное/притяжательное местоимение (_я_, _мой_), также ставится у возвратных|personal pronoun|1:p|
|\*|PronType=Dem||PronType=Dem|указательное местоимение (_этот_, _такой_)|demonstrative pronoun|1:d|
|\*|PronType=Tot||PronType=Tot|кванторное местоимение (_все_, _весь_, _каждый_, _любой_)|total (collective) pronoun|1:n|
|\*|PronType=Int||PronType=Int|вопросительное местоимение (_кто_, _чей_)|interrogative pronoun|1:q|
|\*|PronType=Rel||PronType=Rel|относительное местоимение (_который_, _кто_)|relative pronoun|1:r|
|\*|PronType=Neg||PronType=Neg|отрицательное местоимение (_никто_, _ничей_)|negative pronoun|1:z|
|\*|PronType=Ind||PronType=Ind|неопределенное местоимение (_кто-то_, _чей-нибудь_)|indefinite pronoun|1:i|
|\*|PronType=Rcp||PronType=Rcp|взаимное местоимение (_друг друга_)|reciprocal pronoun|
|\*|PronType=Emp||PronType=Emp|выделительное местоимение (_сам_, _самый_)|emphatic pronoun|
|\*|PronType=Exc||PronType=Exc|восклицательное местоимение (_как!_, _каков!_)|exclamative pronoun|
|\*|Reflex=Yes||Reflex=Yes|возвратное (_себя_, _свой_)|reflexive (pronoun)|1:x|
|\*|Poss=Yes||Poss=Yes|притяжательное (_мой_, _свой_)|possessive (pronoun)|1:s|
|\*|NumType=Card||NumType=Card|количественное числительное (_два_,_21_)|cardinal numeral|1:c|
|\*|NumType=Sets||NumType=Sets|собирательное числительное (_двое_, _пятеро_)|collective numeral|1:l|
|\*|NumType=Frac||NumType=Frac|доля (_пол_, _1/5_)|fraction||
||NumType=Ord||NumType=Ord|порядковое числительное (_второй_, _2-ой_)|ordinal numeral|1:o|
|=|NameType=Giv|persn|NameType=Giv|личное имя (_Иван_, _Дарья_, _Леопольд_, _Эстер_, _Гомер_, _Маугли_)|name of a person: first, given name|
|=|NameType=Patrn|patrn|NameType=Patrn|отчество (_Иванович_, _Павловна_)|patronymic name|
|=|NameType=Sur|famn|NameType=Sur|фамилия (_Николаев_, _Волконская_, _Гумбольдт_)|family name, second name |
|\+|NameType=Prs|persn|NameType=Prs|другие имена лиц (_Жирик_, _ЕБН_, _ВИЛ_)|other name of a person|
|=|NameType=Zoo|zoon|NameType=Zoo|кличка животного (_Шарик_, _Дочка_)|zoonym|
|=|NameType=Geo|topon|NameType=Geo|топоним (_Москва_, _Полянка_)|toponym|
|\*|NameType=Com| |NameType=Com|название организации (_МТС_, _Зенит_)|name of a company|
|\*|NameType=Pro| |NameType=Pro|название продукции (_Звезда_, _Бирюса_)|toponym|
|\*|NameType=Oth| |NameType=Oth|другие имена собственные (_Оскар_, _ЕГЭ_)|other personal names|
|!|Indecl=Yes|0|Indecl=Yes|несклоняемое (_шоссе_, _Седых_)|indeclinable|
|!|Anom=Yes|anom|Anom=Yes|аномальная форма (различного рода морфологические аномалии, возможные у устаревших или просторечных нелитературных форм (_три дни_ при нормативном _три дня_, _ляжь_ при нормативном _ляг_))|grammatically anomalous form|
|=|Abbr=Yes|abbr|Abbr=Yes|сокращение (сокращенная запись (_тов._, _гг._, _ч._). В поле «Лемма» сокращение (кроме инициалов) раскрывается, указывается грамматическая форма, соответствующая контексту. Специально отметим, что акронимы вроде _ООН_, _вуз_ и усеченные слова вроде _зав_, _зам_, записываемые без точки и не раскрываемые при чтении, не получают пометы abbr и трактуются как обычные слова (склоняемые или несклоняемые))|abbreviation|
|=|Typo=Yes|distort|Typo=Yes|искаженная форма (орфографическое и/или фонетическое искажение слова, часто передающее различные особенности произношения (_дэвушка_, _това’ищи_, _про-хо-ди_, _низнаю_))|distorted form|
|\*|Foreign=Yes||Foreign=Yes|неосвоенное слово (часто у X или если затруднительно определить грамматические признаки)|foreign|
|=|NumForm=Digit|ciph|NumForm=Digit|цифровая запись (запись числительного, числительного-прилагательного или прилагательного (полностью или частично) при помощи цифр (_73_, _LXXIII_, _73-й_, _22-летний_). Для этих словоформ в поле «Лемма» также употребляется цифровая запись; число и падеж указываются только в тех случаях, когда выписано окончание (типа _14-му_))|digital|5:d|
|\*|NumForm=Word||NumForm=Word|буквенная запись числительного, числительного-прилагательного (_первому_)|word|5:l|
|\*|NumForm=Roman||NumForm=Roman|запись числительного, числительного-прилагательного латинскими буквами (_V-IX_)|roman letters|5:r|
||(NumForm=Combi)|ciph||комбинированная запись (_73-ий_, _22-летний_)|digital|

For MulTEXT-East v4,  see https://www.sketchengine.eu/russian-tagset/. Features such as `2:m` means the `2nd` position of the value `m` in the positional MorphoSyntacticDescripttion (MSD): positions of Animacy, Case, Gender, and Number are given for nouns; positions of VerbForm, Aspect, Tense, Voice, Person - for verbs, positions of Possessiveness, Degree, Variant - for adjectives, PronType and Reflex - for pronouns, NumType=for numerals.

Universal UD guidelines: https://universaldependencies.org/u/feat/index.html  

Russian UD guidelines: https://universaldependencies.org/ru/feat/index.html  

More on the tag statistics in UD: https://github.com/UniversalDependencies/UD_Russian-Taiga/blob/dev/stats.xml  
