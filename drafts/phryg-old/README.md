# Dataset 'Old Phrygian Inscriptions'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/phrygian/phryg.htm).

* URL: https://github.com/TITUS-2-0/other-ie/tree/main/drafts/phryg-old/
* version: unreleased
* date: 2025-02-21

## Citation
```text
Digital version of Old Phrygian Inscriptions (draft version). By: Jost Gippert, A. Lubotsky, Florian Matter. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/other-ie/tree/main/drafts/phryg-old/, visited on <insert date>)
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
text (@xml:lang=xpg-Grek-x-ophryg)
  body
    div (@data-level=1, @n, @type=provenance, @xml:id) (multiple)
      div (@data-level=2, @n, @type=inscription, @xml:id) (multiple)
        p (@xml:id) (multiple)
          choice (multiple)
            reg (@type=transliteration, @xml:lang=xpg-Latn-x-ophryg-tld) (multiple)
            orig (multiple)
            reg (@type=transliteration, @xml:lang=xpg-Latn-x-ophryg-tld)
              space (@type=hole, @xml:id)
            orig
              space (@type=hole, @xml:id)
            reg (@type=transliteration, @xml:lang=xpg-Latn-x-ophryg-tld) (multiple)
              gap (@precision=low, @quantity=10 | 11, @reason=lost, @unit=line, @xml:lang=eng-Latn) (multiple)
            orig (multiple)
              gap (@precision=low, @quantity=10 | 11, @reason=lost, @unit=line, @xml:lang=eng-Latn) (multiple)
          [lb (@n) (multiple)]
          [note (@xml:id, @xml:lang=eng-Latn) (multiple)]
        p (@xml:id) (multiple)
          app (@xml:id) (multiple)
            rdg (@xml:id) (multiple)
              choice (multiple)
                reg (@type=transliteration, @xml:lang=xpg-Latn-x-ophryg-tld) (multiple)
                orig (multiple)
            rdg (@xml:id) (multiple)
              corr (multiple)
                choice (multiple)
                  reg (@type=transliteration, @xml:lang=xpg-Latn-x-ophryg-tld) (multiple)
                  orig (multiple)
            rdg (@xml:id) (multiple)
              orig (multiple)
                choice (multiple)
                  reg (@type=transliteration, @xml:lang=xpg-Latn-x-ophryg-tld) (multiple)
                  orig (multiple)
          [lb (@n) (multiple)]
      div (@data-level=2, @n, @type=inscription-group, @xml:id)
        p (@xml:id)
          [note (@xml:id, @xml:lang=eng-Latn)]
        div (@data-level=3, @n, @type=inscription, @xml:id) (multiple)
          p (@xml:id) (multiple)
            choice (multiple)
              reg (@type=transliteration, @xml:lang=xpg-Latn-x-ophryg-tld) (multiple)
              orig (multiple)
            [lb (@n) (multiple)]
      div (@data-level=2, @n, @type=inscription-group, @xml:id) (multiple)
        div (@data-level=3, @n, @type=inscription, @xml:id) (multiple)
          p (@xml:id) (multiple)
            choice (multiple)
              reg (@type=transliteration, @xml:lang=xpg-Latn-x-ophryg-tld) (multiple)
              orig (multiple)
            [lb (@n) (multiple)]
            [note (@xml:id, @xml:lang=eng-Latn)]
          p (@xml:id)
            app (@xml:id)
              rdg (@xml:id) (multiple)
                choice (multiple)
                  reg (@type=transliteration, @xml:lang=xpg-Latn-x-ophryg-tld) (multiple)
                  orig (multiple)
            [lb (@n)]
          p (@xml:id) (multiple)
            app (@xml:id) (multiple)
              rdg (@xml:id) (multiple)
                choice (multiple)
                  reg (@type=transliteration, @xml:lang=xpg-Latn-x-ophryg-tld) (multiple)
                  orig (multiple)
              rdg (@xml:id, @xml:lang=xpg-Latn-x-ophryg-tld) (multiple)
                wit (@xml:lang=eng-Latn) (multiple)
            choice (multiple)
              reg (@type=transliteration, @xml:lang=xpg-Latn-x-ophryg-tld) (multiple)
              orig (multiple)
            [lb (@n) (multiple)]
      div (@data-level=2, @n, @type=inscription, @xml:id, @xml:lang=eng-Latn)
        p (@xml:id)
          [lb (@n)]
          [note (@xml:id)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="M" xml:id="provenance-1" type="provenance" data-level="1">
				<div n="1a" xml:id="provenance-1-inscription-1" type="inscription" data-level="2">
					<p xml:id="provenance-1-inscription-1-p-1">
						<lb n="1"/>
						<choice>
							<reg type="transliteration" xml:lang="xpg-Latn-x-ophryg-tld">ates : arkiaevais : akenanogavos : midai : lavagtaei : vanaktei : edaes</reg>
							<orig>ΑΤΕΣ : ΑΡΚΙΑΕFΑΙΣ : ΑΚΕΝΑΝΟΓΑFΟΣ : ΜΙΔΑΙ : ΛΑFΑΓΤΑΕΙ : FΑΝΑΚΤΕΙ : ΕΔΑΕΣ</orig>
						</choice>
					</p>
				</div>
				<div n="1b" xml:id="provenance-1-inscription-2" type="inscription" data-level="2">
					<p xml:id="provenance-1-inscription-2-p-2">
  ...
```
