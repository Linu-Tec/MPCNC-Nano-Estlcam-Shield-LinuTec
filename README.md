# 🌀 MPCNC Nano Estlcam Shield (LinuTec Version)

Ein leistungsstarkes und kostengünstiges CNC-Interface-Shield für die **MPCNC (Mostly Printed CNC)** und andere DIY-Fräsen. Das Board nutzt einen **Arduino Nano** als Steuerzentrale und dient als dedizierte Schnittstellenlösung für die Hardware-Steuerung über die Software **Estlcam**.

Es bietet im Vergleich zu Standard-GRBL-Shields (wie dem CNC Shield V3) erweiterte Filter, stabilere Signalwege und dedizierte Anschlussmöglichkeiten für Endschalter, Werkzeuglängensensoren sowie Relais-Ausgänge.

---

## 📋 Stückliste (Bill of Materials)

Hier findest du die vollständige Liste aller Bauteile, die für die Bestückung des MPCNC Nano Estlcam Shields benötigt werden.

**!Achtung! Nicht alle Artikel vorhanden!**

[Reichelt Warenkorb](https://www.reichelt.de/my/2279582)

---

### 🔌 Steckplätze & Klemmen

| Pos | Menge | Referenz | Bauteil / Bezeichnung | Kommentar |
| :---: | :---: | :--- | :--- | :--- |
| 🔲 | 1 | - | **Leiterplatte** | MPCNC Nano Estlcam Shield Platine (160x100mm) |
| 🔌 | 3 | J1, J16, J17 | **Schraubklemmen 2-polig** | 5mm Pinabstand (Anschlüsse) |
| 🔌 | 16 | J4-6, J12-J14, J18-J27 | **Schraubklemmen 3-polig** | 5mm Pinabstand (Anschlüsse) |
| 🔌 | 2 | 2x A1 | **Buchsenleisten 15-polig** | Pinabstand 2,54mm (für Arduino Nano) |
| 🔌 | 6 | je 2x A2-A4 | **Buchsenleisten 8-polig** | Pinabstand 2,54mm (für Treiberplatinen) |
| ⚙️ | 4 | *Verteilt* | **Stiftleisten 20-polig** | Pinabstand 2,54mm (Anschlüsse, Jumper) |
| ⚙️ | 20 | JP1-JP17 | **Jumperstecker** | Pinabstand 2,54mm (steckbar) |
| 🌀 | 1 | J2 | **Platinenstecker 3-polig** | MOLEX 22041031 (für Lüfteranschluss) |

### 🧠 ICs & Halbleiter

| Pos | Menge | Referenz | Bauteil / Bezeichnung | Kommentar |
| :---: | :---: | :--- | :--- | :--- |
| 🔋 | 1 | U6 | **IC L7805 (TO-220)** | 5V Spannungsregler |
| 🏎️ | 1 | U1 | **IC LM358 (DIP-8)** | Operationsverstärker (FU-Schaltung) |
| 🔌 | 1 | U5 | **IC ULN2003AN (DIP-16)**| Relaistreiber (Ausgangskanäle) |
| 🛡️ | 3 | U2, U3, U4 | **IC LTV-847 (DIP-16)** | Optokoppler (Eingangskanäle, Ausgang Spindel) |
| 🔲 | 2 | D2, D3 | **Dioden 1N5822** | Verpolungsschutz |

### 💡 Status- & Signal-LEDs

| Pos | Menge | Referenz | Bauteil / Bezeichnung | Kommentar |
| :---: | :---: | :--- | :--- | :--- |
| 🔴 | 1 | D1 | **LED 5mm Rot** | „Power On 5V“ |
| 🟢 | 1 | D4 | **LED 5mm Grün** | „Power On 12-36V“ |
| 🛑 | 3 | D5, D6, D7 | **LED 3mm Transparent Rot**| Ausgangssignal für OUT 1-3 |

### 🥢 Widerstände & Potentiometer

| Pos | Menge | Referenz | Bauteil / Bezeichnung | Kommentar |
| :---: | :---: | :--- | :--- | :--- |
| 🥢 | 10 | R4-R12, R14 | **Widerstand 220 Ω** | Rot-Rot-Braun-Gold (Vorwiderstand OK, LED) |
| 🥢 | 4 | R1, R16-R18 | **Widerstand 1 kΩ** | Braun-Schwarz-Rot-Gold (Vorwiderstand LED, TP-Filter) |
| 🥢 | 1 | R15 | **Widerstand 1,8 kΩ** | Braun-Silber-Rot-Gold (Vorwiderstand LED) |
| 🥢 | 3 | R2, R3, R13 | **Widerstand 10 kΩ** | Braun-Schwarz-Orange-Gold (Spannungsteiler FU / Vorwiderstand OK) |
| 🎛️ | 1 | RV1 | **Potentiometer 5 kΩ** | Für FU-Schaltung (Frequenzumrichter) |

### ⚡ Kondensatoren

| Pos | Menge | Referenz | Bauteil / Bezeichnung | Kommentar |
| :---: | :---: | :--- | :--- | :--- |
| ⚡ | 1 | C7 | **Kondensator (MLCC) 100nF**| Abblockkondensator μC |
| ⚡ | 1 | C6 | **Elko 0,1 μF (5x11mm)** | Spannungsregler 5V-Seite |
| ⚡ | 1 | C5 | **Elko 0,33 μF (5x11mm)**| Spannungsregler 12V-Seite |
| ⚡ | 4 | C1-C4 | **Elko 100 μF (8x12mm)** | Stabilisierung Treiber, TP-Filter |

### 🔩 Zubehör & Mechanik

| Pos | Menge | Referenz | Bauteil / Bezeichnung | Kommentar |
| :---: | :---: | :--- | :--- | :--- |
| 🥶 | 1 | HS1 | **Kühlkörper** | Für 5V-Spannungsregler (L7805) |
| 🔩 | 1 | für HS1 | **Schraube M3x8** | Für Montage des Kühlkörpers |
| 🔲 | 4 | U2-U5 | **IC-Sockel DIP-16** | Für alle 16-Pin ICs (Optional) |
| 🔲 | 2 | U1, U7 | **IC-Sockel DIP-8** | Für alle 8-Pin ICs (Optional) |

> ℹ️ *Verteilung der 20-poligen Stiftleisten:* Aufgeteilt auf die Anschlüsse/Jumper J3, J7-J11, J15, J28, J29 und JP1-JP17.


---

Es fehlt:
- Schraube M3x8
- Elektrolyt-Kondensator 0,1μF, 5x11mm
- Elektrolyt-Kondensator 0,33μF, 5x11mm
- Elektrolyt-Kondensator 100μF, 8x12mm
- Kühlkörper für 5V-Spannungsregler (für L7805)

---

## 🛠️ Technische Spezifikationen & Funktionen

* **Software-Unterstützung:** Nahtlose Integration in die **Estlcam Klemmenbelegung (Arduino Nano)**.
* **Achsen-Steuerung:** Unterstützung für X-, Y- und Z-Achsen.
* **Erweiterbarkeit:** Pins für Werkzeuglängensensor (Messescheibe), Spindelsteuerung (Relais/PWM) und Not-Aus (Estop) sind direkt herausgeführt.
* **Signalstabilität:** Hardwareseitige Filterkondensatoren an den Eingängen minimieren Fehlauslösungen durch elektromagnetische Störungen (EMV) von der Frässpindel.

---

## ⚙️ Estlcam Firmware-Inbetriebnahme

Da Estlcam eine eigene, closed-source Firmware auf den Arduino Nano flasht, wird der Code direkt aus der Software heraus installiert:

1. Verbinde den Arduino Nano (noch ohne Motorspannung) per USB mit deinem PC.
2. Öffne **Estlcam** und gehe in die **Einstellungen ➔ CNC-Steuerung**.
3. Wähle als Hardware **"Arduino Nano"** aus.
4. Stelle das Pin-Mapping passend zum Shield-Layout ein (Estlcam Standard-Nano-Belegung).
5. Klicke auf **"Steuerung programmieren"**. Nach dem Flash-Vorgang ist das Board einsatzbereit.

---

## 📺 Projekt-Video auf YouTube

Schau dir das vollständige Video zum Aufbau und der Inbetriebnahme des MPCNC Estlcam Shields auf YouTube an:

[<img width="418" height="229" alt="image" src="https://github.com/user-attachments/assets/a4a38104-90d5-4306-8764-ed6bc58f201b" />
](https://youtu.be/ErM-tjGVLzc)

*Klicke auf das Bild, um das Video direkt auf YouTube abzuspielen.*



---

## 📂 Repository-Struktur

* `/hardware` - Schaltpläne, Platinenlayouts und die für die Fertigung benötigten Gerber-Dateien.
* `/3d-prints` - STL-Dateien für passende Gehäuse oder Hutschienen-Halterungen.
* `/docs` - Anschlusspläne und Pin-Belegungsdiagramme als Referenz.

---

## 📝 Lizenz

Dieses Projekt steht unter der **MIT-Lizenz**. Genauere Informationen findest du in der Datei `LICENSE`.



## PCB MPCNC-Nano-Estlcam-Shield
- [MPCNC-Nano-Estlcam-Shield](https://github.com/tnn85/MPCNC-Nano-Estlcam-Shield)
