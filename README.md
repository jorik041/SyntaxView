# SyntaxView
Code beautifier for Android

#Usage

Add to your Android layout xml:
```xml
<eu.fiskur.syntaxview.SyntaxView
    android:id="@+id/syntaxview"
    android:layout_width="match_parent"
    android:layout_height="match_parent"/>
```

Initialise and set theme:

```java
SyntaxView syntaxView = (SyntaxView) findViewById(R.id.syntaxview);
syntaxView.setup("monokai-sublime");
syntaxView.setLoadingColor(Color.parseColor("#00ffcc"));
```

Load file:

```java
boolean detectLanguage = true;
syntaxView.loadFile(file, detectLanguage);
```


