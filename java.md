# Java - Hinweise

## Namenskonventionen

- Bezeichner enthalten keine Umlaute bzw. ß
- Namen von Packages enthalten nur Kleinbuchstaben
- Klassennamen beginnen mit einem Großbuchstaben
- Variablen- und Methodennamen beginnen mit einem Kleinbuchstaben

## JavaBeans

```
import java.io.Serializable;

public class Book implements Serializable {
    // Attribut
    private String title;

    // Standardkonstruktor (ohne Parameter)
    public Book() {
    }

    // Optional: onstruktor mit Parameter
    public Book(String title) {
        this.title = title;
    }

    // Getter-Methode für title
    public String getTitle() {
        return title;
    }

    // Setter-Methode für title
    public void setTitle(String title) {
        this.title = title;
    }

    // Optional: Überschreiben der toString-Methode für eine bessere Darstellung
    @Override
    public String toString() {
        return "Book{title='" + title + "'}";
    }
}
```


