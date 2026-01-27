# ðŸ“‘ XML & XSD Schema Validation Practices

<p align="center">
  <img src="https://img.shields.io/badge/XML-00599C?style=for-the-badge&logo=xml&logoColor=white" alt="XML" />
  <img src="https://img.shields.io/badge/Schema-XSD_1.0-FF6600?style=for-the-badge" alt="XSD" />
  <img src="https://img.shields.io/badge/Validation-W3C_Standards-047857?style=for-the-badge" alt="W3C" />
  <img src="https://img.shields.io/badge/Academic-1Âº_DAW_STUCOM-10B981?style=for-the-badge" alt="STUCOM" />
</p>

> ðŸŽ“ **Academic Project Notice:** This project was developed as a laboratory assignment for the **1st year of Web Application Development (DAW)** at **STUCOM Pelai** (Barcelona) within the Markup Languages and Information Management Systems module (LMSGI).

---

## ðŸ“Œ Overview / DescripciÃ³n General

### ðŸ‡¬ðŸ‡§ English
This repository contains structured **XML** datasets and strict **XML Schema Definitions (XSD)** created to practice data structuring, constraints, type definitions, and schema validation according to W3C standards.

### ðŸ‡ªðŸ‡¸ EspaÃ±ol
Este repositorio recopila prÃ¡cticas de diseÃ±o y validaciÃ³n de documentos **XML** mediante esquemas **XSD (XML Schema Definition)**, orientados a garantizar la integridad, tipos de datos y restricciones estructurales segÃºn los estÃ¡ndares del W3C.

---

## ðŸ“‚ Included Schemas & Datasets

| Dataset | XML Data File | XSD Schema File | Description |
| :--- | :--- | :--- | :--- |
| ðŸ“š **Books Catalog** | libro.xml | libro.xsd | Validates literary catalog metadata: ISBN, titles, authors, publishers, formats, and pricing rules. |
| ðŸŽµ **Music Catalog** | musica.xml | musica.xsd | Validates musical albums, tracklists, durations, artists, musical genres, and release years. |

---

## ðŸ” Validation Rules Tested

- **Simple & Complex Types:** Usage of xs:simpleType with regex restrictions (xs:pattern) and xs:complexType.
- **Cardinals & Sequences:** Strict ordering with xs:sequence, minOccurs, and maxOccurs.
- **Enumerations & Facets:** Allowed value restrictions (xs:enumeration), string lengths, and numeric ranges.

---

## ðŸš€ How to Validate

Using xmllint in terminal:
`ash
xmllint --noout --schema libro.xsd libro.xml
xmllint --noout --schema musica.xsd musica.xml
`

---

## ðŸ“„ License

Distributed under the **MIT License**.
