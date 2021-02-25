# Good Practice Kapitel 1

<!-- markdownlint-configure-file { "MD024":
    { "allow_different_nesting": true } }
-->
Lorem Ipsum ist einfach ein Blindtext der Druck- und Satzindustrie. Lorem Ipsum
ist der Standard-Blindtext der Industrie seit dem Jahr 1500, als ein unbekannter
Drucker eine ein unbekannter Drucker eine Druckfahne nahm und sie zu einem
Schriftprobenbuch verarbeitete. Buch. Es hat nicht nur fünf Jahrhunderte
überlebt, sondern auch den Sprung in den elektronischen Schriftsatz überlebt und
ist im Wesentlichen unverändert geblieben. Populär wurde sie in den 1960er
Jahren mit der Veröffentlichung von Letraset-Bögen, die Lorem Ipsum-Passagen
enthielten, und in jüngerer Zeit mit und in jüngerer Zeit mit
Desktop-Publishing-Software wie Aldus PageMaker, die Versionen von Lorem Ipsum.

## G-1010: Niemals XYZ

### Grund

dd

### Rechtfertigung

Der Grund dafür ist:

1. weil 1=1
2. weil 2=2

### Beispiel (schlecht)

Dies ist ein SQL-Codeblock

```SQL
SELECT file_name FROM dba_data_files;
```

### Beispiel (gut)

Dies ist ein BASH-Codeblock

```BASH
if [ -z $TEST ]; then
    echo "\$TEST is empty"
else
    echo "\$TEST is defined"
fi
```

### Bewertung

| Priorität | Wirkung |
|-----------|---------|
| hoch      | mittel  |

## G-1011: Besser

### Grund

dd

### Begründung

Der Grund hierfür ist:

1. Weil 1=1
2. Weil 2=2

### Beispiel (schlecht)

Dies ist ein SQL-Codeblock

```SQL
SELECT file_name FROM dba_data_files;
```

### Beispiel (gut)

Dies ist ein BASH-Codeblock

```BASH
if [ -z $TEST ]; then
    echo "\$TEST is empty"
else
    echo "\$TEST is defined"
fi
```

### Bewertung

| Priorität | Wirkung |
|-----------|---------|
| hoch      | mittel  |
