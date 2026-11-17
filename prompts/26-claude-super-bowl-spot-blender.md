# Super-Bowl-Spot mit dem Claude-Logo in Blender

Voraussetzung: Blender (über das Blender-MCP oder per Kommandozeile), ffmpeg und die Higgsfield CLI für Musik und Sounds. Dem Prompt ein Bild des Claude-Logos als Vorlage anhängen.

```text
Mach ein Video in Blender (3D), in dem das Claude-Logo fleißig arbeitet. Dabei macht es folgende drei Dinge:

1. Ein Auto reparieren (angelehnt an den Post): https://x.com/zulali/status/2120204711790023128
2. Einen Fernseher von Werbung befreien (angelehnt an den Post): https://x.com/gathint/status/2111379569030939102
3. Sich an einen PC setzen, die Tastatur bedienen und den PC aufräumen: überflüssige Dateien entfernen, RAM freigeben usw.

Das soll ein inspirierendes Video werden, das als Werbespot beim Super Bowl laufen könnte – direkt für Anthropic. Designern und Video-Cuttern muss die Kinnlade runterfallen.

Das Claude-Logo sieht so aus wie das Beispiel, das ich mitgegeben habe, es soll aber natürlich ein 3D-Männchen sein. Zum Start verwandelt sich das flache Logo in die 3D-Figur. Jede der drei Szenen zeigt erst das Problem (qualmendes Auto, Fernseher voller Werbekacheln, glühender, überlasteter PC) und dann sichtbar die Lösung. Am Ende stehen alle drei reparierten Dinge nebeneinander, dazu ein Schlussbild mit Figur, Wortmarke und einem kurzen Claim. Verwende keine echten Markenlogos für Auto oder Fernseher.

Technik: 1920×1080, 24 fps, Länge irgendwas zwischen 30 und 60 Sekunden, kannst du selbst entscheiden, wie es für dich am besten ausgeht. Alles per Skript gebaut, die .blend-Datei soll sich normal öffnen lassen.

Ton: Musik und Sounds generierst du mit ElevenLabs über die Higgsfield CLI. Falls dafür keine Credits da sind, synthetisiere Musik und Soundeffekte selbst, im Takt zum Schnitt, und leg ein Skript bei, mit dem ich die ElevenLabs-Musik später nachziehen kann. Mische auf etwa −14 LUFS.

Prüfe das Ergebnis an Einzelbildern in voller Auflösung und sag ehrlich, was du nur stichprobenartig kontrolliert hast.
```
