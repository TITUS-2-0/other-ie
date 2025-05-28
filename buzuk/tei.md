

### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Chapter | `div@chapter` | Automatically translated into named div |
| Page  | `pb` |  |
| Line | `lb` |  |
| Page of ms. A | `pb@manuscript-a` |  |
| Page of ms. B | `pb@manuscript-b` |  |

### Structural overview
```text
text (@xml:lang=aln-Latn-x-buzuku)
  body
    div (@data-level=1, @n, @type=chapter, @xml:id) (multiple)
      p (@xml:id) (multiple)
        [lb (@n) (multiple)]
        [lb (@break=no, @n) (multiple)]
        [pb (@main=yes, @n) (multiple)]
        [pb (@n, @type=manuscript-a | manuscript-b) (multiple)]
      [pb (@main=yes, @n)]
      [pb (@n, @type=manuscript-a)]
    div (@data-level=1, @n, @type=chapter, @xml:id) (multiple)
      head (@n) (multiple)
      p (@xml:id) (multiple)
        [lb (@n) (multiple)]
        [lb (@break=no, @n) (multiple)]
        [pb (@main=yes, @n) (multiple)]
        [pb (@n, @type=manuscript-a | manuscript-b) (multiple)]
        [pb (@type=manuscript-a | manuscript-b) (multiple)]
      head (multiple)
    div (@data-level=1, @n, @type=chapter, @xml:id)
      head (@n)
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="chapter-1" type="chapter" data-level="1">
				<pb n="4" main="yes"/>
				<pb type="manuscript-a" n="009r"/>
				<p xml:id="chapter-1-p-1">
					<lb n="1"/>O e ſene merii hiir plota ama / e p̱ mi-<lb n="2" break="no"/>ſerierſimeh tih neueh en anemicut nah<lb n="3"/>ruoih / e enditet ſeh moɿtſeh ſaneh nah<lb n="4"/>perɛeh. Laudi tuu clofte ћi ieh leem<lb n="5"/>en virћenet mena ћitune iaſte ferene / e<lb n="6"/>iet p̱ herre me atet becuom / e meh ſpir-<lb n="7" break="no"/>tine ſegñte per iete teh ieteſſe. Amen.<lb n="8"/>V̷ Tih ieh e becuome ender ћiξe graat.<lb n="9"/>R̷ E becuom anſte fruiti hi barcut tit.<lb n="10"/>Aña. Becuom ieh o merii am̀[a] e atii<lb n="11"/>ћi leue. Cancha e Ʒachariſſe pɿofete.<lb n="12"/>BEcuom clofte ɛot ɛoti ɣineh hi<lb n="13"/>iſraelit: per ſeh aih nah viɛitoih<lb n="14"/>e banih teh ſperblenete / e popu-<lb n="15" break="no"/>liſſe vet. E aih neue nah endereћi vir-<lb n="16" break="no"/>tutne tet ſelbuomit en ſtepiet ſeh daui-<lb n="17" break="no"/>dit ſerbetoɿit tii. Poɿ ſih pat ξaſuneh<lb n="18"/>per goiet teh ſegñtet ћi enſeh ɛanet en-<lb n="19" break="no"/>fill iane en pɿofeteſit ſeh tiis. E pat-<lb n="20" break="no"/>meh nah ſpetuom en anemiſit ſinees:<lb n="21"/>e enduoɿſit ſatunes ћi neue nah deſneh<lb n="22"/>cheћ. E aih erξ meh baam miſeriere<lb n="23"/>meh perint tane e meɣ arecoɿduom en<lb n="24"/>teſtamentit ſegñte ſeh tii. E cheio an-<lb n="25" break="no"/>ſte beia ћi pat baam aih Abɿaamit pe-<lb n="26" break="no"/>rindit tine: ſeh aih neue chis meh nah<lb n="27"/>ɣ ξane. Per ſeh nah ſih teh liberoniſ-<lb n="28" break="no"/>gnim en duoɿſit ſeh anemiћet tineue /<lb n="29"/>paa en mner nah atii te ſerbegnim. En-<lb n="30" break="no"/>de ſegñtenii / e endee dereite p̱ para tii:<lb n="31"/>p̱ ћiξe ditte tone. E tih d[ia]lleh te iees<lb n="32"/>griſune pɿofeta hi dnaltet p̱ ſeh tii chee<lb n="33"/>meh vote p̱ para faћeſe tine ɛot. Meh<lb n="34"/>traituõ vξete etii: meh ξane te ditunite ъ<lb n="35"/>ſelbuomit populiſſe tii: p̱ teh liruom teh<lb n="36"/>quatet. Per miſeriert teh maξe teh per<lb n="37"/>bɿendeſauet teh tine ɛot: ћi aih nah vi-<lb n="38" break="no"/>ɛitoih tue lene p̱ ſeh nalti. Per ſeh aih te<lb n="39"/>ɛdriξten ћiξe atah ћi ende Thereteh ie-<lb n="40" break="no"/>ſene / e ende hiiet teh moɿtſe meh ende-<lb n="41" break="no"/>reћune cãbete tone enbuξe teh paћſeh.<lb n="42"/>Laudi clofte atit e birit / e ſpirtit ſegñte.<lb n="43"/>Añ. E becuomeia ama / e tine ɛot me-<lb n="44" break="no"/>rii virћena p̱ iete te ieteſſe. Cliſah e tine<lb n="45"/>ɛot: teh ſecruomite e ſpirtit ſegñte: ћi<lb n="46"/>ſchleh tietere enbe ſẽbelture tãde pelћe-<lb n="47" break="no"/>ue tine ɛot ieɛɣ xp̅it oɿo p̱ populit: goie-<lb n="48" break="no"/>tareia ione / e p̱ pɿiftenit: e ɣ lut p̱ ſpirtit<lb n="49"/>teh grauet ðeuota. O ɛot chii miſerier.<lb n="50"/>O chɿiſt chii miſerier. O ɛot chii mi-<lb n="51" break="no"/>ſerier. ɛot endiglo oɿatene temeh / e em<lb n="52"/>tuu arte teh ξirete tem. Oɿatio.<lb n="53"/>O ɛot ћi enbarcut ſeh ſene meriſſe<lb n="54"/>virћene deſſe bire tãd tue paſune<lb n="55"/>ſalutuõ enћeli: tɣeih ξaſune meh ɣ ɛane<lb n="56"/>coɿp en nieriɣ: ban hiir atune ћi tuu teh<lb n="57"/>luſene poɿ ſih nah meh ћiξe ɛemere be-<lb n="58" break="no"/>ſoime aioh meh clene ama e tine ɛot a-<lb n="59" break="no"/>ſtɣ per para tuu per teh lutunit te ſaih:<lb n="60"/>nah teh iemi endimuom per chɿiſtneh<lb n="61"/>ɛotne tane. Amen.</p>
			</div>
```
