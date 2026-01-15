

### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| `Chapter` (hierarchical) | `div@chapter` (hierarchical) | Automatically translated into named div |
| `Paragraph` (hierarchical) | `p` (hierarchical) |  |
| `Line` (hierarchical) | `lb` (hierarchical) |  |
| `Page` (linear) | `pb` (linear) |  |

### Structural overview
```text
text (@xml:lang=aln-Latn-x-buzuku)
  front (@xml:id)
    titlePage (@xml:id, @xml:lang=lat-Latn)
      docTitle (@xml:id)
        titlePart (@xml:id) (multiple)
      byline
        docAuthor
      docImprint
        pubPlace (@xml:id)
        publisher (@xml:id)
        docDate
      imprimatur
      [milestone (@facs=#facs-236, @unit=ref, @xml:id)]
    div (@data-level=1, @type=dedication, @xml:id)
      head
        [foreign (@xml:lang=lat-Latn) (multiple)]
      signed
        [foreign (@xml:lang=lat-Latn)]
      p (@xml:id) (multiple)
        [foreign (@xml:lang=lat-Latn) (multiple)]
      [milestone (@facs=#facs-234 | #facs-235, @unit=ref, @xml:id) (multiple)]
    div (@data-level=1, @type=preface, @xml:id)
      head
        [foreign (@xml:lang=lat-Latn)]
      p (@xml:id)
        [milestone (@facs=#facs-228 | #facs-229 | #facs-230 | #facs-231 | #facs-232, @unit=ref, @xml:id) (multiple)]
        [foreign (@xml:lang=lat-Latn) (multiple)]
      closer
        dateline
        salute
        signed
      [milestone (@facs=#facs-233, @unit=ref, @xml:id)]
    div (@data-level=1, @type=imprimatur, @xml:id)
      p (@xml:id) (multiple)
      signed (multiple)
      [milestone (@facs=#facs-227, @unit=ref, @xml:id)]
    div (@data-level=1, @type=notes, @xml:id)
      head
      p (@xml:id)
        [foreign (@xml:lang=lat-Latn) (multiple)]
        [milestone (@facs=#facs-225, @unit=ref, @xml:id)]
      [milestone (@facs=#facs-226, @unit=ref, @xml:id)]
    div (@data-level=1, @type=commendatory_poems, @xml:id)
      lg (@xml:id) (multiple)
        head (multiple)
          [milestone (@facs=#facs-223 | #facs-224, @unit=ref, @xml:id) (multiple)]
          [foreign (@xml:lang=lat-Latn) (multiple)]
        l (@xml:id) (multiple)
    div (@data-level=1, @type=contents, @xml:id)
      head (multiple)
      list
        item (multiple)
      [milestone (@facs=#facs-221 | #facs-222, @unit=ref, @xml:id) (multiple)]
      [pb (@n)]
  body
    div (@data-level=1, @n, @type=dictionary, @xml:id)
      head (multiple)
      entry (multiple)
        sense (multiple)
          gloss (@xml:lang=lat-Latn) (multiple)
        form (multiple)
        form (multiple)
          corr (multiple)
        form
          choice
            sic
            corr
      [lb (@n) (multiple)]
      [pb (@n) (multiple)]
      [milestone (@facs=#facs-100 | #facs-101 | #facs-102 | #facs-103 | #facs-104 | #facs-105 | #facs-106 | #facs-107 | #facs-108 | #facs-109 | #facs-110 | #facs-111 | #facs-112 | #facs-113 | #facs-114 | #facs-115 | #facs-116 | #facs-117 | #facs-118 | #facs-119 | #facs-120 | #facs-121 | #facs-122 | #facs-123 | #facs-124 | #facs-125 | #facs-126 | #facs-127 | #facs-128 | #facs-129 | #facs-130 | #facs-131 | #facs-132 | #facs-133 | #facs-134 | #facs-135 | #facs-136 | #facs-137 | #facs-138 | #facs-139 | #facs-140 | #facs-141 | #facs-142 | #facs-143 | #facs-144 | #facs-145 | #facs-146 | #facs-147 | #facs-148 | #facs-149 | #facs-150 | #facs-151 | #facs-152 | #facs-153 | #facs-154 | #facs-155 | #facs-156 | #facs-157 | #facs-158 | #facs-159 | #facs-160 | #facs-161 | #facs-162 | #facs-163 | #facs-164 | #facs-165 | #facs-166 | #facs-167 | #facs-168 | #facs-169 | #facs-170 | #facs-171 | #facs-172 | #facs-173 | #facs-174 | #facs-175 | #facs-176 | #facs-177 | #facs-178 | #facs-179 | #facs-180 | #facs-181 | #facs-182 | #facs-183 | #facs-184 | #facs-185 | #facs-186 | #facs-187 | #facs-188 | #facs-189 | #facs-190 | #facs-191 | #facs-192 | #facs-193 | #facs-194 | #facs-195 | #facs-196 | #facs-197 | #facs-198 | #facs-199 | #facs-200 | #facs-201 | #facs-202 | #facs-203 | #facs-204 | #facs-205 | #facs-206 | #facs-207 | #facs-208 | #facs-209 | #facs-210 | #facs-211 | #facs-212 | #facs-213 | #facs-214 | #facs-215 | #facs-216 | #facs-217 | #facs-218 | #facs-219 | #facs-220 | #facs-35 | #facs-36 | #facs-37 | #facs-38 | #facs-39 | #facs-40 | #facs-41 | #facs-42 | #facs-43 | #facs-44 | #facs-45 | #facs-46 | #facs-47 | #facs-48 | #facs-49 | #facs-50 | #facs-51 | #facs-52 | #facs-53 | #facs-54 | #facs-55 | #facs-56 | #facs-57 | #facs-58 | #facs-59 | #facs-60 | #facs-61 | #facs-62 | #facs-63 | #facs-64 | #facs-65 | #facs-66 | #facs-67 | #facs-68 | #facs-69 | #facs-70 | #facs-71 | #facs-72 | #facs-73 | #facs-74 | #facs-75 | #facs-76 | #facs-77 | #facs-78 | #facs-79 | #facs-80 | #facs-81 | #facs-82 | #facs-83 | #facs-84 | #facs-85 | #facs-86 | #facs-87 | #facs-88 | #facs-89 | #facs-90 | #facs-91 | #facs-92 | #facs-93 | #facs-94 | #facs-95 | #facs-96 | #facs-97 | #facs-98 | #facs-99, @unit=ref, @xml:id) (multiple)]
    div (@data-level=1, @n, @type=chapter, @xml:id) (multiple)
      head (multiple)
        [foreign (@xml:lang=lat-Latn | und-Latn-x-general) (multiple)]
      p (@n, @xml:id) (multiple)
        [foreign (@xml:lang=ita-Latn | lat-Latn | tur-Latn | und-Latn-x-general) (multiple)]
        [lb (@n) (multiple)]
        [pb (@n) (multiple)]
        [milestone (@facs=#facs-1 | #facs-10 | #facs-11 | #facs-12 | #facs-13 | #facs-14 | #facs-15 | #facs-16 | #facs-17 | #facs-18 | #facs-19 | #facs-2 | #facs-20 | #facs-21 | #facs-22 | #facs-23 | #facs-24 | #facs-25 | #facs-26 | #facs-27 | #facs-28 | #facs-29 | #facs-3 | #facs-30 | #facs-31 | #facs-32 | #facs-33 | #facs-34 | #facs-4 | #facs-5 | #facs-6 | #facs-7 | #facs-8 | #facs-9, @unit=ref, @xml:id) (multiple)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="Alph." type="dictionary" xml:id="front-1-dedication-1-preface-1-imprimatur-1-notes-1-commendatory_poems-1-contents-1-dictionary-1" data-level="1">
        <head>DICTIONARIUM</head>
        <head>LATINO-EPIROTICVM</head>
        <lb n="1"/>
        <entry>
          <sense>
            <gloss xml:lang="lat-Latn">Ab altera parte</gloss>
          </sense>
          <form>Mbe tieteret ane</form>
        </entry>
        <lb n="2"/>
        <entry>
  ...
```
