# Russian National Corpus tagset (main corpus): conversion table to UD 2.0

Created: 11 Jan 2017

## Parts of speech (XPOS)

|Status|RNC tag|UPOS tag|description(RUS)|description(ENG)|
|---|---|---|---|---|
||S|NOUN|существительное (_яблоня_, _лошадь_, _корпус_, _вечность_)|noun|
|+|S|PROPN|+ существительное - имя собственное|(_Иван_, _Москва_, _СССР_); определяется по пометам persn, patrn, famn, zoon и в большинстве случаев abbr в поле «Грамматика»|proper noun|
|-|INIT|PROPN|инициал (запись вида «заглавная буква с точкой» (_М._, _Р._). В поле «Лемма» инициал не раскрывается; грамматические признаки не указываются)|proper noun (initial letter)|
||A|ADJ|прилагательное (_коричневый_, _таинственный_, _морской_)|adjective|
||NUM|NUM|числительное (_четыре_, _4_, _много_)|numeral|
|-|ANUM|ADJ|числительное-прилагательное (_седьмой_, _восьмидесятый_); NB за исключением _один_ (размечается как NUM)|ordinal numeral|
||V|VERB|глагол (_пользоваться_, _обрабатывать_)|verb|
|+|V|AUX|вспомогательный глагол _быть_ (выполняющий функции грамматического показателя)|auxiliary|
|-|PRAEDIC|VERB|предикатив (_жаль_, _хорошо_, _пора_), см. [список](https://github.com/olesar/ruUD/blob/master/praedic_list.md)|predicative|
|-|PRAEDICPRO|VERB|местоимение-предикатив (_некого_, _нечего_)|predicative pronoun|
||ADV|ADV|наречие (_сгоряча_, _очень_)|adverb|
|-|PARENTH|ADV|вводное слово (_кстати_, _по-моему_)|parenthetically used discoursive markers|
|\*|SPRO|PRON|местоимение-существительное (_она_, _что_), см. [список](https://github.com/olesar/ruUD/blob/master/pron_list.md)|pronoun (as noun)|
|\*|APRO|DET|местоимение-прилагательное (_этот_, _твой_); NB за исключением _который_ (размечается как PRON), см. [список](https://github.com/olesar/ruUD/blob/master/det_list.md)|adjectival pronoun/determiner|
|-|ADVPRO|ADV||местоименное наречие (_где_, _вот_)	adverbial pronoun|
||PR|ADP|предлог (_под_, _напротив_)|preposition/adposition|
||CONJ|SCONJ|союз (_что_, _чтобы_); при конвертации по умолчанию подчинительный|subordinating conjunction|
|+|CONJ|CCONJ|+ сочинительный союз (_и_, _но_), см. [список](https://github.com/olesar/ruUD/blob/master/conj_list.md)|coordinating conjunction|
||PART|PART|частица (_бы_, _же_, _пусть_)|particle|
||INTJ|INTJ|междометие (_увы_, _батюшки_)|interjection|
||NONLEX|X|не-слова (_шшетт_, _bolo_)|foreign and non-words |
|+||SYM|символ (_%_, _$_)|symbol|
|+||PUNCT|знак препинания|punctuation mark|

## Grammatical features (FEAT)

|Status|RNC tag|FEAT feature|description(RUS)|description(ENG)|
|---|---|---|---|---|
||m|Gender=Masc|мужской род (_работник_, _стол_)|masculine gender|
||f|Gender=Fem|женский род (_работница_, _табуретка_)|feminine gender|
||n|Gender=Neut|средний род (_животное_, _озеро_)|neuter gender|
|~|mf|Gender=Masc|«общий род» (_задира_, _пьяница_); в большинстве случаев приравнивание к м. р. не будет порождать ошибки|common gender (the feature Gender=Com is not available in Russian UD)|
||anim|Animacy=Anim|одушевленность (_человек_, _ангел_, _утопленник_)|animate|
||inan|Animacy=Inan|неодушевленность (_рука_, _облако_, _культура_)|inanimate|
||sg|Number=Sing|единственное число (_яблоко_, _гордость_)|singular number|
||pl|Number=Plur|множественное число (_яблоки_, _ножницы_, _детишки_)|plural number|
||nom|Case=Nom|именительный падеж (_голова_, _сын_, _степь_, _сани_, _который_)|Nominative case|
||gen|Case=Gen|родительный падеж (_головы_, _сына_, _степи_, _саней_, _которого_)|Genitive case|
||dat|Case=Dat|дательный падеж (_голове_, _сыну_, _степи_, _саням_, _которому_)|Dative case|
||acc|Case=Acc|винительный падеж (_голову_, _сына_, _степь_, _сани_, _который/которого_)|Accusative case|
||ins|Case=Ins|творительный падеж (_головой_, _сыном_, _степью_, _санями_, _которым_)|Instrumental case|
||loc|Case=Loc|предложный падеж ([_о_] _голове_, _сыне_, _степи_, _санях_, _котором_)|Locative case|
||voc|Case=Voc|звательная форма (_Господи_, _Серёж_, _ребят_)|Vocative case|
||gen2|Case=Par|второй родительный падеж (_чашка чаю_)|Partitive case|
|-|dat2|Case=Dat|дистрибутивный дательный ([_по_] _многу_, _нескольку_, _стольку_)|second Dative case|
|-|acc2|Case=Nom|второй винительный падеж (_постричься в монахи_; _по два человека_)|second Accusative case (in UD is treated as Nominative, still animate)|
|-|loc2|Case=Loc|второй предложный падеж (_в лесу_, _на оси́_)|second Locative case|
|-|adnum|Case=Gen|счётная форма (_два часа́_, _три шара́_)|adnumeral form|
||brev|Variant=Short|краткая форма (_высок_, _нежна_, _прочны_, _рад_)|short form|
|-|plen||полная форма (_высокий_, _нежная_, _прочные_, _морской_)|full form|
|+||Degree=Pos|позитивная степень (_глубокий_); присваивается всем формам прилагательных, наречий и предикативов, не имеющих сравнительной или превосходной степени|positive, first degree|
||comp|Degree=Cmp|сравнительная степень (_глубже_)|comparative degree|
|-|comp2|Degree=Cmp|форма «по+сравнительная степень» (_поглубже_)|second comparative degree (_po_ + comparative)|
|\*|supr|Degree=Sup|превосходная степень (_глубочайший_); ! в НКРЯ отсутствует и лемматизируется по образцу _глубочайший_, должна быть различена с позитивной степенью|superlative degree	|
||pf|Aspect=Perf|совершенный вид (_пошёл_, _встречу_)|perfective aspect|
||ipf|Aspect=Imp|несовершенный вид (_ходил_, _встречаю_)|imperfective aspect|
|-|intr||непереходность (_ходить_, _вариться_)|intransitive verb|
|-|tran||переходность (_вести_, _варить_)|transitive verb|
||act|Voice=Act|действительный залог (_разрушил_, _разрушивший_)|active voice|
||pass|Voice=Pass|страдательный залог (только у причастий: _разрушаемый_, _разрушенный_)|passive voice|
||med|Voice=Mid|медиальный, или средний залог (глагольные формы на _-ся_: _разрушился_ и т.п.)|middle voice|
||inf|VerbForm=Inf|инфинитив (_украшать_)|infinitive|
|+||VerbForm=Fin|финитная форма; в НКРЯ отсутствует, присваивается по умолчанию всем формам, не являющимся инфинитивом, причастием и деепричастием|finite verb|
||partcp|VerbForm=Part|причастие (_украшенный_)|participle|
||ger|VerbForm=Conv|деепричастие (_украшая_)|gerundive (converb)|
||indic|Mood=Ind|изъявительное наклонение (_украшаю_, _украшал_, _украшу_)|indicative mood|
||imper|Mood=Imp|повелительное наклонение (_украшай_)|imperative mood|
|-|imper2|Mood=Imp|форма повелительного наклонения 1 л. мн. ч. на -те (_идемте_)|second imperative (imperative on _-мте_)|
||praet|Tense=Past|прошедшее время (_украшали_, _украшавший_, _украсив_)|past tense|
||praes|Tense=Pres|настоящее время (_украшаем_, _украшающий_, _украшая_)|present tense|
||fut|Tense=Fut|будущее время (_украсим_); у глаголов несовершенного вида сложная форма размечается в два слова как _буду_ + инфинитив|future tense|
||1p|Person=1|первое лицо (_украшаю_)|first person|
||2p|Person=2|второе лицо (_украшаешь_)|second person|
||3p|Person=3|третье лицо (_украшает_)|third person|
|-|persn||личное имя (_Иван_, _Дарья_, _Леопольд_, _Эстер_, _Гомер_, _Маугли_)|name of a person, first, given name|
|-|patrn||отчество (_Иванович_, _Павловна_)|patronymic name|
|-|famn||фамилия (_Николаев_, _Волконская_, _Гумбольдт_)|family name, second name |
|-|zoon||кличка животного (_Шарик_, _Дочка_)|zoonym|
|-|0||несклоняемое (_шоссе_, _Седых_)|indeclinable|
|-|anom||аномальная форма (различного рода морфологические аномалии, возможные у устаревших или просторечных нелитературных форм (_три дни_ при нормативном _три дня_, _ляжь_ при нормативном _ляг_))|grammatically anomalous form|
|-|distort|Typo=Yes|искаженная форма (орфографическое и/или фонетическое искажение слова, часто передающее различные особенности произношения (_дэвушка_, _това’ищи_, _про-хо-ди_, _низнаю_))|distorted form|
|-|ciph||цифровая запись (запись числительного, числительного-прилагательного или прилагательного (полностью или частично) при помощи цифр (_73_, _LXXIII_, _73-й_, _22-летний_). Для этих словоформ в поле «Лемма» также употребляется цифровая запись; число и падеж указываются только в тех случаях, когда выписано окончание (типа _14-му_))|digital|
|-|abbr|Abbr=Yes|сокращение (сокращенная запись (_тов._, _гг._, _ч._). В поле «Лемма» сокращение (кроме инициалов) раскрывается, указывается грамматическая форма, соответствующая контексту. Специально отметим, что акронимы вроде _ООН_, _вуз_ и усеченные слова вроде _зав_, _зам_, записываемые без точки и не раскрываемые при чтении, не получают пометы abbr и трактуются как обычные слова (склоняемые или несклоняемые))|abbreviation|
