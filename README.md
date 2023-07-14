jpegfiles
=========

Various PDF files for testing PDF readers.


Files
-----

### balloon\_a1b\_jp2k.pdf

Fairly normal file (not encrypted, not linearized, no object streams, normal
xref). Contains two `/Filter [/JPXDecode]` images.

From
<http://opf-labs.org/format-corpus/pdfCabinetOfHorrors/balloon_a1b_jp2k.pdf>.

### CIPA\_DC-007-2021\_E.pdf

- PDF 1.7
- Encrypted (V5, R6, AESV3 (!))
- xref stream
- obj streams
- not linearized

From <https://cipa.jp/std/documents/download_e.html?CIPA_DC-007-2021_E>.

### dummy.pdf

- PDF 1.4
- `/Info` object with UTF-16 strings
  - `Producer: OpenOffice.org 2.1`
- `/Outlines` data
- Embedded TTF font
- Streams have `/Length` as indirect object reference stored after the stream
- Fairly simple: Not linearized, no object streams, no xref stream, no
  incremental updates; regular `xref`, `trailer`, `startxref`, `%%EOF`.

From <https://www.w3.org/WAI/ER/tests/xhtml/testfiles/resources/pdf/dummy.pdf>.

### encryption\_nocopy.pdf

- PDF 1.7
- Encrypted (V4, R4, AESV2)
- Linearized
- XRef stream only (not hybrid)
- Object streams
- `/Columns` and `Predictor 12` in `/DecodeParams` of a `/FlateDecode` stream

From
<http://opf-labs.org/format-corpus/pdfCabinetOfHorrors/encryption_nocopy.pdf>.

### pdf-test.pdf

- PDF 1.6
- Linearized
- Encrypted (V2, R3, Length 128)
- Object streams
- Contains a bunch of bitmaps, partially in object streams
- Hybrid-reference file with `xref`, but first `trailer` also has a `/XRefStm`
  key pointing at a `/XRef` stream

Fairly complete edge-case workout (encrypted, linearized, obj stream, xref
stream, hybrid)!

From <https://www.orimi.com/pdf-test.pdf>.

### veraPDFHiRes.pdf

- Linearized
- Contains a `/Filter/DCTDecode` image

From <http://opf-labs.org/format-corpus/pdfCabinetOfHorrors/veraPDFHiRes.pdf>.
