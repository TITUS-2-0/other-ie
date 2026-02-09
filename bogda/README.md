# Dataset 'Cuneus prophetarum (1685)'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/alban/bogdani/bogda.htm).

* URL: https://github.com/TITUS-2-0/other-ie/tree/main/drafts/bogda
* version: 0.1.0
* date: 2025-12-04

## Citation
```text
Digital version of Cuneus prophetarum (1685) by Pjetër Bogdani (v0.1.0). By: Michiel de Vaan, Jost Gippert, Florian Matter. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/other-ie/tree/main/drafts/bogda, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| `Verse` (hierarchical) | `ab@verse` (hierarchical) |  |
| `Scala` (hierarchical) | `div@scala` (hierarchical) | Automatically translated into named div |
| `Chapter` (hierarchical) | `div@chapter` (hierarchical) | Automatically translated into named div |
| `Paragraph` (hierarchical) | `p` (hierarchical) | #   Part: milestone@part |
| `Page` (linear) | `pb` (linear) |  |

### Structural overview
```text
text (@xml:lang=aln-Latn-x-buzuku)
  body
    div (@data-level=1, @n, @type=part, @xml:id) (multiple)
      head (@xml:lang=und-Latn-x-general) (multiple)
      div (@data-level=2, @type=contents, @xml:id) (multiple)
        head (multiple)
        list
          head
          item (@n) (multiple)
            list (multiple)
              head (multiple)
              item (@n) (multiple)
        list
          item (@n) (multiple)
            list (multiple)
              head (multiple)
              item (@n) (multiple)
      div (@data-level=2, @n, @type=scala, @xml:id) (multiple)
        head (multiple)
        ab (@n, @type=verse, @xml:id) (multiple)
          [foreign (@xml:lang=lat-Latn) (multiple)]
            [foreign (@xml:lang=lat-Latn)]
          [pb (@n) (multiple)]
      div (@data-level=2, @n, @type=scala, @xml:id) (multiple)
        head (multiple)
        div (@data-level=3, @n, @type=chapter, @xml:id) (multiple)
          head (multiple)
          p (@n, @xml:id) (multiple)
            [pb (@n) (multiple)]
            [foreign (@xml:lang=lat-Latn | und-Latn-x-general) (multiple)]
          ab (@n, @type=verse, @xml:id) (multiple)
            [pb (@n) (multiple)]
        div (@data-level=3, @n, @type=chapter, @xml:id) (multiple)
          head (multiple)
          p (@n, @xml:id) (multiple)
            [pb (@n) (multiple)]
            [foreign (@xml:lang=und-Latn-x-general) (multiple)]
          [pb (@n)]
        div (@data-level=3, @n, @type=chapter, @xml:id)
          head
          ab (@n, @type=verse, @xml:id) (multiple)
            [pb (@n) (multiple)]
          [pb (@n)]
      div (@data-level=2, @n, @type=scala, @xml:id)
        div (@data-level=3, @n, @type=chapter, @xml:id) (multiple)
          head (multiple)
          p (@n, @xml:id) (multiple)
            [pb (@n) (multiple)]
          ab (@n, @type=verse, @xml:id) (multiple)
            [pb (@n) (multiple)]
      [pb (@n) (multiple)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="part-1" type="part" data-level="1">
        <head xml:lang="und-Latn-x-general">Vetus Testamentum</head>
        <div xml:id="part-1-contents-1" type="contents" data-level="2">
          <head>Contents</head>
          <list>
            <head>TE PRIMITE PERPARA LETTERARIT</head>
            <item n="1">
              <list>
                <head>Scala I. Si criioi ɛotüne nierine; Mcatit, e mengijet sè tijnaj.</head>
                <item n="I.I">Si ansctè Hüji ndè vetèhe.</item>
                <item n="I.II">Si anscte nder tre vete Gnia i vètèmi Hüj</item>
                <item n="I.III">Si e Caλeɛuene profetete te scene Tritatne.</item>
  ...
```
