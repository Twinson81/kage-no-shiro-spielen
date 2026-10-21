# Kage no Shiro – Prototyp zum Mitspielen

Shinobi-Koop für 1–4 Spieler (Unreal Engine 5.8). Frühe Testversion: Graybox-Festung, Parkour (Kanten, Wandlauf, Enterhaken, Doppelsprung), Schleichen, Kampf mit Haltung, Abwehr und Deflect gegen eine Trainingswache – mit Kampfkunst oder Schwert.

## Herunterladen

Unter **Releases** (rechts) die neueste `KageNoShiro_Windows.zip` laden, entpacken und `KageNoShiro.exe` starten. Windows 10/11, 64 Bit; eine Grafikkarte mit DirectX 12.

**Updates:** Ab Version 0.2.0 prüft das Hauptmenü beim Start, ob es hier eine neuere Version gibt. Dann erscheint **Jetzt aktualisieren** – das Spiel lädt die neue Version, prüft sie und startet neu. Wer noch 0.1.0 hat, lädt 0.2.0 einmal von Hand.

## Zusammen spielen (direkte Verbindung)

1. Alle tragen im Startmenü ihren Namen ein.
2. Einer klickt auf **Spiel hosten** und landet in der **Lobby**. Dort stehen Einladecodes (z. B. `7H3KQ-0M8ZA`) mit Kopieren-Knopf.
3. Die anderen geben den Code (oder die IP) ein und klicken **Beitreten**. In der Lobby sieht man, wer da ist und wer bereit ist; der Host startet das Spiel.
4. Beim ersten Start die Windows-Firewall-Frage mit „Zugriff zulassen“ beantworten.

Der Einladecode ist die verpackte Adresse des Hosts – es gibt keinen Server dazwischen. Darum gilt weiter:

| Ihr seid … | Code aus der Lobby | Was nötig ist |
|---|---|---|
| im selben WLAN/LAN | LAN | nichts |
| an verschiedenen Orten, mit VPN | VPN (100.x.y.z) | beide nutzen Tailscale oder ZeroTier im selben Netz |
| an verschiedenen Orten, direkt | Internet | Portweiterleitung **UDP 7777** am Router des Hosts |

Am einfachsten ist das VPN. Bei manchen Anschlüssen (DS-Lite, Mobilfunk) funktioniert der direkte Weg nicht.
Alle Spieler brauchen dieselbe Version; mit einer anderen lehnt der Host den Beitritt ab. Mehr steht in `LIESMICH.txt` im ZIP.

## Steuerung

WASD/Maus gehen und umsehen · Umschalt rennen · Leertaste springen (in der Luft nochmal: Doppelsprung mit Salto; Kante: hochziehen; Wand: abspringen) · C ducken und schleichen (Kante: loslassen) · E Enterhaken · linke Maustaste Angriff · rechte Maustaste Abwehr (kurz vor dem Treffer: Deflect) · Q zwischen Kampfkunst und Schwert wechseln · Esc Menü. Gamepad wird unterstützt.

**Kampf:** Ihr beginnt ohne Waffe mit Fäusten und Tritten. Am Schwertständer im Hof hebt jeder ein Schwert auf; danach wechselt Q zwischen Kampfkunst und Schwert.

## Hinweise

Figuren: Unreal-Mannequin (Epic Games). Animationen: Mixamo (Adobe). Die Inhalte sind Teil des Spiels und dürfen nicht einzeln weiterverwendet werden. Prototyp ohne Gewähr.
