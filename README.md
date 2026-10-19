# Kage no Shiro – Prototyp zum Mitspielen

Shinobi-Koop für 1–4 Spieler (Unreal Engine 5.8). Frühe Testversion: Graybox-Festung, Parkour (Kanten, Wandlauf, Enterhaken), Kampf mit Haltung, Abwehr und Deflect gegen eine Trainingswache.

## Herunterladen

Unter **Releases** (rechts) die neueste `KageNoShiro_Windows.zip` laden, entpacken und `KageNoShiro.exe` starten. Windows 10/11, 64 Bit; eine Grafikkarte mit DirectX 12.

## Zusammen spielen (direkte Verbindung)

1. Einer klickt im Startmenü auf **Spiel hosten**. Das Menü zeigt seine Adressen.
2. Die anderen geben die Adresse des Hosts ein und klicken **Beitreten**.
3. Beim ersten Start die Windows-Firewall-Frage mit „Zugriff zulassen“ beantworten.

| Ihr seid … | Adresse | Was nötig ist |
|---|---|---|
| im selben WLAN/LAN | lokale IP des Hosts (z. B. 192.168.1.20) | nichts |
| an verschiedenen Orten, mit VPN | VPN-IP des Hosts (Tailscale: 100.x.y.z) | beide nutzen Tailscale oder ZeroTier im selben Netz |
| an verschiedenen Orten, direkt | öffentliche IP des Hosts | Portweiterleitung **UDP 7777** am Router des Hosts |

Am einfachsten ist das VPN. Bei manchen Anschlüssen (DS-Lite, Mobilfunk) funktioniert der direkte Weg nicht.
Alle Spieler brauchen dieselbe Version. Mehr steht in `LIESMICH.txt` im ZIP.

## Steuerung

WASD/Maus gehen und umsehen · Umschalt rennen · Leertaste springen (Kante: hochziehen, Wand: abspringen) · C ducken (Kante: loslassen) · E Enterhaken · linke Maustaste Angriff · rechte Maustaste Abwehr (kurz vor dem Treffer: Deflect) · Esc Menü. Gamepad wird unterstützt.

## Hinweise

Figuren: Unreal-Mannequin (Epic Games). Animationen: Mixamo (Adobe). Die Inhalte sind Teil des Spiels und dürfen nicht einzeln weiterverwendet werden. Prototyp ohne Gewähr.
