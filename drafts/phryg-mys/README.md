# Dataset '"Mysian" inscriptions'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/phrygian/phryg.htm).

* URL: https://github.com/TITUS-2-0/other-ie/tree/main/drafts/phryg-mys/
* version: unreleased
* date: 2025-02-24

## Citation
```text
Digital version of "Mysian" inscriptions (draft version). By: Jost Gippert, A. Lubotsky, Florian Matter. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/other-ie/tree/main/drafts/phryg-mys/, visited on <insert date>)
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
text (@xml:lang=yms-Grek)
  body
    div (@data-level=1, @n, @type=provenance, @xml:id)
      div (@data-level=2, @n, @type=inscription, @xml:id) (multiple)
        app (@xml:id) (multiple)
          rdg (@xml:id) (multiple)
            choice (multiple)
              reg (@type=transliteration, @xml:lang=yms-Latn-x-tld) (multiple)
              orig (multiple)
          rdg (@xml:id) (multiple)
            wit (multiple)
            choice (multiple)
              reg (@type=transliteration, @xml:lang=yms-Latn-x-tld) (multiple)
              orig (multiple)
        [lb (@n) (multiple)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="BO" xml:id="provenance-1" type="provenance" data-level="1">
				<div n="1" xml:id="provenance-1-inscription-1" type="inscription" data-level="2">
					<lb n="1"/>
					<app xml:id="provenance-1-inscription-1-app-1">
						<rdg xml:id="provenance-1-inscription-1-app-1-rdg-1">
							<choice>
								<reg type="transliteration" xml:lang="yms-Latn-x-tld">]e[ ]y...</reg>
								<orig>]Ε[ ]J...</orig>
							</choice>
						</rdg>
						<rdg xml:id="provenance-1-inscription-1-app-1-rdg-2">
							<wit>Friedrich</wit>
  ...
```
