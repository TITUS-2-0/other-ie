# Dataset 'Missale'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/alban/buzuku/buzuk.htm).

* URL: https://titus2.uni-frankfurt.de/dataset/buzuk
* version: unreleased
* date: 2025-04-21

## Citation
```text
Digital version of Missale by Gjon Buzuku (draft version). By: Jost Gippert, Wolfgang Hock, Florian Matter. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://titus2.uni-frankfurt.de/dataset/buzuk, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| `Chapter` (hierarchical) | `div@chapter` (hierarchical) | Automatically translated into named div |
| `Page ` (linear) | `pb` (linear) |  |
| `Line` (linear) | `lb` (linear) |  |
| `Page of ms. A` (linear) | `pb@manuscript-a` (linear) |  |
| `Page of ms. B` (linear) | `pb@manuscript-b` (linear) |  |

### Structural overview
```text
text (@xml:lang=aln-Latn-x-buzuku)
  body
    div (@data-level=1, @n, @type=chapter, @xml:id)
      p (@xml:id) (multiple)
        [lb (@n) (multiple)]
        [lb (@break=no, @n) (multiple)]
      [pb (@main=yes, @n)]
      [pb (@n, @type=manuscript-a)]
    div (@data-level=1, @n, @type=chapter, @xml:id) (multiple)
      head (multiple)
        [lb (@n) (multiple)]
      p (@xml:id) (multiple)
        [lb (@n) (multiple)]
        [lb (@break=no, @n) (multiple)]
        [pb (@main=yes, @n) (multiple)]
        [pb (@n, @type=manuscript-a | manuscript-b) (multiple)]
        [pb (@type=manuscript-a | manuscript-b) (multiple)]
      [pb (@n)]
      [pb (@n, @type=manuscript-a | manuscript-b) (multiple)]
    div (@data-level=1, @n, @type=chapter, @xml:id)
      head
        [lb (@n)]
      [pb (@n, @type=manuscript-a)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="chapter-1" type="chapter" data-level="1">
        <pb n="4" main="yes"/>
        <pb type="manuscript-a" n="009r"/>
        <p xml:id="chapter-1-p-1">
          <lb n="1"/>O e ſene merii hiir plota ama / e p̱ mi-
          <lb n="2" break="no"/>ſerierſimeh tih neueh en anemicut nah
          <lb n="3"/>ruoih / e enditet ſeh moɿtſeh ſaneh nah
          <lb n="4"/>perɛeh. Laudi tuu clofte ћi ieh leem
          <lb n="5"/>en virћenet mena ћitune iaſte ferene / e
          <lb n="6"/>iet p̱ herre me atet becuom / e meh ſpir-
          <lb n="7" break="no"/>tine ſegñte per iete teh ieteſſe. Amen.</p>
        <p xml:id="chapter-1-p-2">
  ...
```
