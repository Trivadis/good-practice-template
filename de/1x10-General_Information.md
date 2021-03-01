# Einführung
<!-- markdownlint-configure-file { "MD013": { "tables": false } } -->
Fügen Sie eine kurze Einführung in den *Good Practice* Leitfaden ein.

## Scope

Definieren Sie den Geltungsbereich dieser *Good Practice*

## Dokumentationskonventionen

Definieren Sie die Dokumentationskonventionen.

### Schweregrad der Regel

!!! Fehler "Blocker"
    Wird oder kann zu einem Fehler führen.

!!! Gefahr "Kritisch"
    Wird einen hohen/direkten Einfluss auf die Wartungskosten haben.

!!! Warnung "Wichtig"
    Wird eine mittlere/potentielle Auswirkung auf die Wartungskosten haben.

!!! Hinweis "Gering"
    Wird eine geringe Auswirkung auf die Wartungskosten haben.

!!! info "Info"
    Sehr geringe Auswirkung; es handelt sich nur um einen Sanierungskostenbericht.

### Verwendete Schlüsselwörter

| Schlüsselwort | Bedeutung                                                                                     |
|---------------|-----------------------------------------------------------------------------------------------|
| Immer         | Betont, dass diese Regel durchgesetzt werden muss.                                            |
| Nie           | Betont, dass diese Aktion nicht stattfinden darf.                                             |
| Vermeiden     | Betont, dass die Aktion verhindert werden soll, aber es kann Ausnahmen geben.                 |
| Versuchen     | Betont, dass die Regel versucht werden soll, wann immer dies möglich und sinnvoll ist.        |
| Beispiel      | Steht vor Text, der zur Veranschaulichung einer Regel oder einer Empfehlung dient.            |
| Begründung    | Erklärt die Gedanken und den Zweck hinter einer Regel oder einer Empfehlung.                  |
| Einschränkung | Beschreibt die Bedingungen, die erfüllt sein müssen, damit eine Regel angewendet werden kann. |

### Validator-Unterstützung

Das Werkzeug PL/SQL Cop (siehe Kapitel "Werkzeugunterstützung") kann nicht
*alle* Richtlinien in diesem Dokument unterstützen. Richtlinien in diesem
Dokument unterstützen. Die Richtlinien, die *nicht* von PL/SQL Cop-Validatoren
nicht unterstützt werden, sind wie folgt gekennzeichnet:

!!! fehlt "Unsupported in PL/SQL Cop Validators"
    Grund, warum die spezifische Richtlinie nicht von den Validierern
    unterstützt wird.

Das PL/SQL Cop Repository dokumentiert die 
[Details der Validatoreinschränkungen](https://github.com/Trivadis/plsql-cop-cli/blob/main/validator-limitations.md#guidelines).

### Warum sind Standards wichtig

Für eine Maschine, die ein Programm ausführt, ist die Formatierung des Codes
nicht von Bedeutung. Jedoch Für das menschliche Auge ist gut formatierter Code
jedoch viel einfacher zu lesen. Moderne Werkzeuge können helfen, Formatierungs-
und Kodierungsregeln zu implementieren.

Die Implementierung von Formatierungs- und Kodierungsregeln hat folgende
Vorteile für PL/SQL-Entwicklung:

- Gut formatierter Code ist leichter zu lesen, zu analysieren und zu pflegen
  (nicht nur für den  Autor, sondern auch für andere Entwickler).
- Die Entwickler müssen keine eigenen Richtlinien definieren - es ist bereits
  definiert.
- Der Code hat eine Struktur, die es leichter macht, Fehler zu vermeiden.
- Der Code ist effizienter in Bezug auf Leistung und Organisation der
  gesamten Anwendung.
- Der Code ist modularer und damit leichter für andere Anwendungen zu verwenden.

### Wir haben andere Standards

Dieses Dokument definiert nur mögliche Standards. Diese Standards sind nicht in
Stein gegemeisselt, sondern sind als Richtlinien gedacht. Wenn es bereits
Standards gibt, die sich von denen Wenn es bereits Standards gibt, die sich von
denen in diesem Dokument unterscheiden, macht es keinen Sinn, sie zu ändern.

### Wir sind nicht mit allen Ihren Standards einverstanden

Es gibt grundsätzlich zwei Arten von Standards.

1. Nicht umstritten

    Diese Standards machen Sinn. Es gibt keinen Grund, sie nicht zu befolgen.
    Ein Beispiel für diese Kategorie ist
    [G-2150](../../4-language-usage/2-variables-and-types/1-general/g-2150):
    Vermeiden Sie Vergleiche mit NULL-Wert, erwägen Sie die Verwendung von IS
    [NOT] NULL.

2. Umstritten

    Fast jede Regel/Richtlinie fällt in diese Kategorie. Ein Beispiel für diese
    Kategorie ist
    [3 Leerzeichen Einzug](../../3-coding-style/coding-style/#rules). - Warum
    nicht 2 oder 4 oder sogar 8? Warum nicht Tabulatoren verwenden? Sie
    können für alle diese Optionen argumentieren. diese Optionen argumentieren.
    In den meisten Fällen spielt es keine Rolle, welche Option Sie wählen.
    Wichtiger ist es, konsistent zu sein. In diesem Fall macht es den Code
    leichter zu lesen.

Bei sehr kontroversen Regeln sind wir dazu übergegangen, die Argumentation
entweder als Fussnote oder direkt im Text.

Normalerweise ist es nicht hilfreich, ein Issue auf GitHub zu öffnen, um die
Änderung einer um die Änderung einer sehr umstrittenen Regel wie der genannten
zu beantragen. Zum Beispiel, verwenden Sie 2 Leerzeichen anstelle von 3
Leerzeichen für eine Einrückung zu verwenden. Dies führt zu einer Diskussion,
in der die Leute, die für 4 Leerzeichen sind, ebenfalls zu argumentieren
beginnen. Es gibt kein richtig oder falsch. Man muss sich nur auf einen Standard
einigen.

Effektiver ist es,
[dieses Repository](https://github.com/Trivadis/plsql-and-sql-coding-guidelines)
zu forken und die Standards so zu ändern, dass sie Ihren
Bedürfnissen/Erwartungen entsprechen.

## Box-Typen

Eine Liste aller verfügbaren Boxen und Optionen finden Sie in der
[`awesomebox`-Dokumentation](https://ctan.org/pkg/awesomebox).

```Markdown
::: note
**Note** Lorem ipsum dolor ...
:::
```

::: note
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam aliquet libero
quis lectus elementum fermentum.

Fusce aliquet augue sapien, non efficitur mi ornare sed. Morbi at dictum
felis. Pellentesque tortor lacus, semper et neque vitae, egestas commodo nisl.
:::

```Markdown
::: tip
**Tip** Lorem ipsum dolor ...
:::
```

::: tip
**Tipp** Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam aliquet
libero quis lectus elementum fermentum.

Fusce aliquet augue sapien, non efficitur mi ornare sed. Morbi at dictum
felis. Pellentesque tortor lacus, semper et neque vitae, egestas commodo nisl.
:::

```Markdown
::: warning
**Warnung** Lorem ipsum dolor ...
:::
```

::: warning
**Warnung** Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam aliquet
liberov quis lectus elementum fermentum.

Fusce aliquet augue sapien, non efficitur mi ornare sed. Morbi at dictum
felis. Pellentesque tortor lacus, semper et neque vitae, egestas commodo nisl.
:::

```Markdown
::: caution
**Vorsicht** Lorem ipsum dolor ...
:::
```

::: caution
**Vorsicht** Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam
aliquet libero quis lectus elementum fermentum.

Fusce aliquet augue sapien, non efficitur mi ornare sed. Morbi at dictum
felis. Pellentesque tortor lacus, semper et neque vitae, egestas commodo nisl.
:::

```Markdown
::: important
**Wichtig** Lorem ipsum dolor ...
:::
```

::: important
**Wichtig** Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam aliquet
libero quis lectus elementum fermentum.

Fusce aliquet augue sapien, non efficitur mi ornare sed. Morbi at dictum
felis. Pellentesque tortor lacus, semper et neque vitae, egestas commodo nisl.
:::

Markdown-Formatierung innerhalb der Umgebungen wird unterstützt.

::: important
**Lorem ipsum dolor** sit amet, `consectetur adipiscing` elit.

```JAVA
if(args.length < 2) {
    System.out.println("Lorem ipsum dolor sit amet");
}
```

*Nam aliquet libero
quis lectus elementum fermentum.*
:::
