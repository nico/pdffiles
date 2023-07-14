jpegfiles
=========

Various PDF files for testing PDF readers.


Files
-----

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
