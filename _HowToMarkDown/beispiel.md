---
marp: true
title: "Vollständiges Markdown-Beispiel"
author: "Max Mustermann"
date: 2026-04-11
bibliography: refs.bib

---
# Überschrift 1: **Fette** und *kursiv* Text

Ein einfacher Absatz. Inline-Code: `print("Hallo")`. Inline-Formel: $E=mc^2$.

---
## Überschrift 2: Listen

**Aufzählungsliste:**
- Punkt 1
- Punkt 2 mit Unterpunkt (Komma: A, B)
- Punkt 3

**Nummerierte Liste:**
1. Erstes
2. Zweites
3. Drittes

---
## Überschrift 2: Zitate

> Dies ist ein Zitat.  
> Mehrzeilig mit Leerzeile. [@doe2024]

**Fußnote[^1].**

---
## Tabellen

| Tool     | Zweck     | Plattform |
|----------|-----------|-----------|
| Pandoc  | PDF/HTML | CLI      |
| Typora  | Editor   | Desktop  |
| VS Code | Erweiterungen | Alle   |

---
## Mathematische Formeln

**Inline:** $a^2 + b^2 = c^2$.

**Block:**
$$
\int_0^\infty e^{-x^2} \, dx = \frac{\sqrt{\pi}}{2}
$$

**Matrix:**
$$
\begin{pmatrix}
1 & 2 \\
3 & 4
\end{pmatrix}
$$

---
## Code-Blöcke

```python
def quadratisches_gleichung(a, b, c):
    return (-b ± sqrt(b**2 - 4*a*c)) / (2*a)
```

**Shell:**
```bash
pandoc datei.md -o datei.pdf --citeproc
```

---
## Diagramme (Mermaid)

```mermaid
graph TD
    A[Markdown] --> B(Pandoc)
    A --> C(Typora)
    B --> D[PDF]
    C --> E[Live-Vorschau]
```

---
## slide with two columns - solution 1
<title>slide with two columns</title>
<div style="display:flex; flex-wrap:wrap; gap:2rem; align-items:flex-start;">
  <div style="flex:1 1 45%; min-width:200px;">
    <h3>Left hand side</h3>
    <ul>
      <li>item</li>
      <li>item</li>
    </ul>
  </div>
  <div style="flex:1 1 45%; min-width:200px;">
    <h3>Right hand side</h3>
    <ul>
      <li>item</li>
      <li>item</li>
    </ul>
  </div>
</div>

---
## slide with two columns - solution 2
title: slide with two columns
<div style="display:flex; flex-wrap:wrap; gap:2rem; align-items:flex-start;" markdown="1">
<div style="flex:1 1 45%; min-width:200px;">

### Left hand side
- item
- item

</div>
<div style="flex:1 1 45%; min-width:200px;">

### Right hand side
- item
- item
</div>
</div>

---
## slide with two columns - solution 2 **Marp**

Markdown Presentation Ecosystem

https://marp.app/

![bg right:40% 80%](example.png)

---
## Links und Bilder

Lesen Sie mehr auf [Pandoc-Docs](https://pandoc.org).

![Beispielbild](/_HowToMarkDown/example.png){width=200px height=200px}

[^1]: Erste Fußnote mit Erklärung.

---
## Literatur

Siehe [@Max2024] für Details.


