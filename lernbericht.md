# Lern-Bericht
Juan Vock
## Einleitung

Mit einem Bild entscheiden was bei der nächste Seite passiert.

## Was habe ich gelernt?

Ich habe gelernt, wie ich ein Bild einen Wert mitgebe und diese Information dann verarbeiten kann.
## Beschreibung

✍️ Verwenden Sie drei verschiedene Medien, um zu zeigen, was Sie gelernt haben. Zum Beispiel:

Ich habe mit habe ein CommandLink genommen, bei dem aber kein Text als Link ist, sondern ein Bild. Ich habe das Bild mit graphicImage im CommandLink hinzugefügt und dazu noch ein setPropertyActionListener dazugetan, damit man beim Klick vom Bild ein Value weitergeben kann. In der Java Klasse habe ich die Information mitgenommen als ein String und habe es mit einem Getter und Setter es verarbeitet.

```html
            <h:commandLink value="" action="page2.xhtml">
                <f:setPropertyActionListener target="#{helloManagedBean.favourite}" value="links"/>
                <h:graphicImage value = "/img/d.png" width="200"/>
            </h:commandLink>

```
```java
    public String getFavourite() {
        if ("links".equals(favourite)) {
            favourite = "d.png";
        } else {
            favourite = "h.png";
        }
        return favourite;
    }
```

```html
            <h:graphicImage value="/img/#{helloManagedBean.favourite}"/>
```
Youtube Video:
https://youtu.be/3IgRTQYaabA



## Verifikation

Beim vorhinige Text wird es erklärt, wie ich die Bilder hinzugefügt habe und welche Code ich benutzen musste.
Bei Code Ausschnitt sieht man genau wie ich das umgesetzt habe. Man sieht den HTML und den Java teil. Im Java sieht man auch wie ich das mit If und Else die Information verarbeitet habe.
Das Youtube Video zeigt, wie alles ohne Fehler läuft. Man drückt auf ein Bild und das Bild kommt auf der nächste Seite auf.

# Reflektion zum Arbeitsprozess

Ich hatte viel Wissen schon von Herr Colic bekommen über das Thema. So konnte ich es ohne sehr grossen Probeleme es programmieren. Ich überlegte mir, wie ich ein Bild auf einer anderen Seite mit Java anzeigen kann. Mir kam es im Sinn, dass ich dann mit einem String versuchen kann und es funktionierte.

Beim GraphicImage brauchte ich lange bis das Bild angezeigt wurde. Ich habe es zuerst mit Libray und Name versucht das Foto aufzurufen, aber es funktionierte nicht. Darum habe ich dann mit Value es versucht und funktionierte.

**VBV**: 
Nächstes Mal versuche nicht so lange auf eine Variante zu bleiben, sondern versuche schneller andere Alternativen zu suchen.
