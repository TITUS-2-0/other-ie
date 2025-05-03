# Dataset 'Neo-Phrygian Inscriptions'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/phrygian/phryg.htm).

* URL: https://github.com/TITUS-2-0/other-ie/tree/main/drafts/phryg-neo/
* version: unreleased
* date: 2025-02-24

## Citation
```text
Digital version of Neo-Phrygian Inscriptions (draft version). By: Jost Gippert, A. Lubotsky, Florian Matter. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/other-ie/tree/main/drafts/phryg-neo/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Provenance | `div@provenance` | Automatically translated into named div |
| Inscription | `div@inscription` | Automatically translated into named div |
| Line | `lb` |  |

### Structural overview
```text
text (@xml:lang=xpg-Grek-x-nphryg)
  body
    div (@data-level=1, @n, @type=provenance, @xml:id)
      div (@data-level=2, @n, @type=inscription, @xml:id) (multiple)
        p (@xml:id) (multiple)
          choice (multiple)
            reg (@type=transliteration, @xml:lang=xpg-Latn-x-nphryg-tld) (multiple)
            orig (multiple)
              [foreign (@xml:lang=grc-Grek)]
            reg (@type=transliteration, @xml:lang=xpg-Latn-x-nphryg-tld)
              g (@type=decorative, @xml:lang=eng-Latn)
            orig
              g (@type=decorative, @xml:lang=eng-Latn)
            reg (@type=transliteration)
              [foreign (@xml:lang=grc-Grek | xpg-Latn-x-nphryg-tld) (multiple)]
            reg (@type=transliteration, @xml:lang=xpg-Latn-x-nphryg-tld)
              space (@type=vacat, @xml:id)
            orig
              space (@type=vacat, @xml:id)
          [lb (@n) (multiple)]
          [note (@xml:id, @xml:lang=eng-Latn) (multiple)]
            [foreign (@xml:lang=xpg-Latn-x-nphryg-tld) (multiple)]
        p (@xml:id) (multiple)
          choice (multiple)
            reg (@type=transliteration, @xml:lang=xpg-Latn-x-nphryg-tld) (multiple)
            orig (multiple)
          app (@xml:id) (multiple)
            rdg (@xml:id) (multiple)
              choice (multiple)
                reg (@type=transliteration, @xml:lang=xpg-Latn-x-nphryg-tld) (multiple)
                orig (multiple)
            rdg (@xml:id) (multiple)
              wit (multiple)
              [foreign (@xml:lang=xpg-Latn-x-nphryg-tld) (multiple)]
            rdg (@xml:id, @xml:lang=xpg-Latn-x-nphryg-tld)
              wit (@xml:lang=eng-Latn)
          [lb (@n) (multiple)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="_" xml:id="provenance-1" type="provenance" data-level="1">
				<div n="2" xml:id="provenance-1-inscription-1" type="inscription" data-level="2">
					<p xml:id="provenance-1-inscription-1-p-1">
						<lb n="1"/>
						<choice>
							<reg type="transliteration" xml:lang="xpg-Latn-x-nphryg-tld">ios ta mankai kakoun addaket ti/e</reg>
							<orig>ΙΟΣ ΤΑ ΜΑΝΚΑΙ ΚΑΚΟΥΝ ΑΔΔΑΚΕΤ ΤΙ/Ε</orig>
						</choice>
						<lb n="2"/>
						<choice>
							<reg type="transliteration" xml:lang="xpg-Latn-x-nphryg-tld">tit [t]etikmenos eitou</reg>
							<orig>ΤΙΤ [Τ]ΕΤΙΚΜΕΝΟΣ ΕΙΤΟΥ</orig>
  ...
```
