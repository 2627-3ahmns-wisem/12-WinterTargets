# Frosty Targets – 3AHMNS

Unity-Version: **6000.3.24f1**. Projekt: Frosty Targets.

## Projekt öffnen
1. Unity Hub öffnen, **Add project from disk** wählen und diesen Ordner auswählen.
2. Unity **6000.3.24f1** verwenden und den ersten Paketimport abwarten.
3. Szene `Assets/MyGame/Scenes/ShootingScene.unity` öffnen, **Play** drücken.
4. `Assets/MyGame/Scripts/GameManager.cs` und `Target.cs` untersuchen.

## Hinweis bei `UnityEngine.UI` / `Text`-Fehlern
Das Paket **Unity UI (uGUI)** ist unter `Packages/manifest.json` als `com.unity.ugui` eingetragen. Falls trotzdem CS0234 oder CS0246 erscheint: `Window > Package Management > Package Manager` öffnen und unter **In Project** prüfen, ob Unity UI geladen ist. Im Paketmanager **Refresh/Resolve** ausführen; gegebenenfalls Unity schließen und den Ordner `Library` löschen, dann erneut öffnen. Nicht die `using UnityEngine.UI`-Zeile entfernen: sie wird für die vorhandene Punkteanzeige gebraucht.

## Unterricht
Das vorhandene Spawning, der Score und der Sieg bei zehn Treffern sind **Ausgangscode**. Schüler:innen erweitern diese Mechaniken anhand der GitHub-Issues. Der Erstimport ist eine Ausgangsversion; keine Aufgaben sind vorweg implementiert.

Festgestellte Probleme – Crosshair und Zielscheiben
Während des Testens des Spiels sind mir mehrere Probleme mit dem Crosshair und der Treffererkennung aufgefallen.
* Crosshair zu groß: Es wird beim Start des Spiels zu groß angezeigt, wodurch das Anvisieren und Treffen der Ziele erschwert wird.
* Bewegung über den gesamten Bildschirm: Das Crosshair bewegt sich im Game-Modus über den gesamten Bildschirm. Dabei wirkt die Steuerung teilweise verzögert.
* Fehlerhafte Treffererkennung: Die Zielscheiben lassen sich nicht treffen. Dadurch werden keine Punkte gezählt und die Treffer werden offenbar nicht richtig registriert.
Geplante Verbesserungen
Das Crosshair soll verkleinert und seine Steuerung verbessert werden, damit es sich besser bewegen lässt.
Zusätzlich soll die Treffererkennung überprüft und angepasst werden, damit angeklickte Zielscheiben zuverlässig erkannt werden und die Punkte korrekt zum Spielstand addiert werden.
Ziel der Verbesserungen ist es, die Steuerung zu optimieren, die Treffererkennung zuverlässig zu gestalten und das gesamte Spielerlebnis zu verbessern.
