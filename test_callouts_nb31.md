<!--

author:   Nicolai Bach

email:    nicolai.bach@fh-potsdam.de

version:  0.0.2

language: de

narrator: Deutsch Female

dark: false

comment:  Demo-Seite für `css/callouts.css`.

link: css/callouts.css

-->

# Callouts

Styles für verschiedene *Callout-Boxen*. In der [LiaScript Dokumentation](https://liascript.github.io/course/?https://raw.githubusercontent.com/liaScript/docs/master/README.md#1) habe ich keine gefunden.

How To
------

In den Metadaten von deinem Dokument muss das Stylesheet (die CSS-Datei) eingebunden werden:

```markdown
<!--

link: css/callouts.css

-->
```

Varianten
---------

```markdown
<!-- class = "callout info" -->
> Lorem ipsum dolor sit amet, consectetur adipiscing elit, …
```

<!-- class = "callout info" -->
> Lorem ipsum dolor sit amet, consectetur adipiscing elit, …

```markdown
<!-- class = "callout tip" -->
> Lorem ipsum dolor sit amet, consectetur adipiscing elit, …
```

<!-- class = "callout tip" -->
> Lorem ipsum dolor sit amet, consectetur adipiscing elit, …

```markdown
<!-- class = "callout success" -->
> Lorem ipsum dolor sit amet, consectetur adipiscing elit, …
```

<!-- class = "callout success" -->
> Lorem ipsum dolor sit amet, consectetur adipiscing elit, …

```markdown
<!-- class = "callout warning" -->
> Lorem ipsum dolor sit amet, consectetur adipiscing elit, …
```
<!-- class = "callout warning" -->
> Lorem ipsum dolor sit amet, consectetur adipiscing elit, …

```markdown
<!-- class = "callout danger" -->
> Lorem ipsum dolor sit amet, consectetur adipiscing elit, …
```

<!-- class = "callout danger" -->
> Lorem ipsum dolor sit amet, consectetur adipiscing elit, …

Mit eigenem Titel
-----------------

Anstelle des Standard-Titels für eine Box kannst du einen eigenen verweden. Dafür muss zusätzlich die Klasse `with-title` angegeben werden. Die erste Zeile deiner Box wird dann als Titel formatiert.

```markdown
<!-- class = "callout info with-title" -->
> Custom Title
> 
> Lorem ipsum dolor sit amet, consectetur adipiscing elit, …
```

<!-- class = "callout info with-title" -->
> Custom Title
> 
> Lorem ipsum dolor sit amet, consectetur adipiscing elit, …
