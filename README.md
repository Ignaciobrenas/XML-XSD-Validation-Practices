# 📑 XML & XSD Schema Validation Practices

<p align="center">
  <img src="https://img.shields.io/badge/XML-00599C?style=for-the-badge&logo=xml&logoColor=white" alt="XML" />
  <img src="https://img.shields.io/badge/Schema-XSD_1.0-FF6600?style=for-the-badge" alt="XSD" />
  <img src="https://img.shields.io/badge/Validation-W3C_Standards-047857?style=for-the-badge" alt="W3C Standards" />
  <img src="https://img.shields.io/badge/Academic-1º_DAW_STUCOM-10B981?style=for-the-badge" alt="STUCOM" />
</p>

> 🎓 **Proyecto Académico:** Prácticas de diseño y validación de esquemas XML conforme a los estándares de la W3C para el módulo de **Lenguajes de Marcas y Sistemas de Gestión de Información** en **STUCOM Pelai** (Barcelona), 1º de DAW.

---

## Descripción del Proyecto

Este repositorio contiene conjuntos de documentos **XML** y sus correspondientes esquemas de definición **XSD (XML Schema Definition)**. El objetivo es estructurar, tipar y validar información jerárquica asegurando restricciones de longitud, patrones regex, ocurrencias de elementos (`minOccurs`, `maxOccurs`) y tipos de datos estrictos.

---

## 📁 Archivos y Modelos

### 📚 Catálogo Bibliográfico (`libro.xml` & `libro.xsd`)
- **Raíz:** `<libros>`
- **Elementos:** `<libro>`, con atributos obligatorios de identificación y categorías.
- **Estructura interna:** `<titulo>`, `<autor>`, `<editorial>`, `<precio>` y `<fechaPublicacion>`.
- **Restricciones:** Tipos simples con patrones para códigos ISBN, fechas ISO y valores numéricos positivos para precios.

### 🎵 Catálogo Musical (`musica.xml` & `musica.xsd`)
- **Raíz:** `<discografia>`
- **Elementos:** Álbumes, artistas, sellos discográficos y listado ordenado de canciones (`<cancion>`).
- **Restricciones:** Duraciones en segundos o minutos, atributos de pista numérica y restricciones de año.

---

## 🚀 Validación de Esquemas

Es posible comprobar la conformidad de los archivos XML con herramientas estándar como `xmllint`:

```bash
# Validar catálogo de libros
xmllint --noout --schema libro.xsd libro.xml

# Validar catálogo musical
xmllint --noout --schema musica.xsd musica.xml
```

Salida esperada al ser válidos:
```text
libro.xml validates
musica.xml validates
```

---

## 👤 Autor

**Ignacio Breñas Muñoz** — 1º DAW, STUCOM Pelai
