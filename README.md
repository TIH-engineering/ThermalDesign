# ThermalDesign

[![release](https://img.shields.io/github/v/release/TIH-engineering/ThermalDesign?label=release)](https://github.com/TIH-engineering/ThermalDesign/releases)
[![Build](https://github.com/TIH-engineering/ThermalDesign/actions/workflows/build.yml/badge.svg)](https://github.com/TIH-engineering/ThermalDesign/actions/workflows/build.yml)
![Hardware](https://img.shields.io/badge/Hardware-KiCad-blue)
![License](https://img.shields.io/badge/License-CC--BY--NC--SA--4.0-lightgrey)

## 🔌 Leiterplattenbeschreibung

Die Leiterplatte **ThermalDesign** dient zur praktischen Untersuchung des **thermischen Verhaltens elektronischer Bauteile**. Als Versuchsobjekt werden mehrere LM317-Linearregler unter unterschiedlichen thermischen Bedingungen und bei verschiedenen Belastungen betrieben.

Die Leiterplatte enthält vier vergleichbare Spannungsreglerstufen mit einer Ausgangsspannung von etwa **2,5 V**. Die Regler unterscheiden sich insbesondere hinsichtlich ihrer thermischen Anbindung:

- **LM317 im SOT-223-Gehäuse**
- **LM317 im TO-220-Gehäuse**
- **LM317 im SOT-223-Gehäuse mit zusätzlicher Kupferfläche zur Wärmeabfuhr**
- **LM317 im TO-220-Gehäuse mit Kühlkörper**

Über verschiedene Lastwiderstände können unterschiedliche Lastfälle eingestellt werden. Vorgesehen sind Untersuchungen bei ungefähr:

- **100 mA**
- **250 mA**
- **500 mA**
- **1 A** als gepulste Last

Die 1-A-Last wird über einen MOSFET geschaltet und kann mit einem externen PWM-Signal angesteuert werden. Dadurch lassen sich neben stationären Temperaturzuständen auch **dynamische Erwärmungs- und Abkühlvorgänge** untersuchen.

Mit der Leiterplatte können unter anderem der Zusammenhang zwischen **Verlustleistung, Bauteiltemperatur, thermischem Widerstand, Gehäusebauform, Kupferfläche und Kühlkörper** experimentell untersucht werden. Die Messergebnisse können mit theoretischen Berechnungen oder thermischen Ersatzschaltbildern verglichen werden.

> **Einsatzgebiet:** Laborübungen und Unterricht zu thermischem Design, Verlustleistung, Wärmewiderständen, Linearreglern und Kühlung elektronischer Bauteile

---

## 📥 Downloads

| Datei | Beschreibung |
|---|---|
| 📄 [Schaltplan (PDF)](../../releases/latest/download/schematic.pdf) | Schaltplan der Leiterplatte |
| 🖨️ [Leiterplatte (PDF)](../../releases/latest/download/pcb.pdf) | Leiterplattenansicht als PDF |
| 🔩 [Bohrplan (PDF)](../../releases/latest/download/drill.pdf) | Bohrdaten / Bohrplan |
| 📋 [Stückliste (Excel)](../../releases/latest/download/bom.xlsx) | Bill of Materials |
| 🌐 [Interactive BOM](../../releases/latest/download/ibom.html) | Interaktive Bestückungsansicht |
| 📦 [Fertigungsdaten](../../releases/latest/download/kicad.zip) | Gerber- und Bohrdaten |
| 🧊 [STEP-Modell](../../releases/latest/download/pcb.step) | 3D-Modell der Leiterplatte |

Die Dateien werden automatisch durch den Release-Workflow erzeugt.

---

## 🖥️ Leiterplatte

### Vorschau

| Oberseite | Unterseite |
|:---:|:---:|
| ![PCB Top](../../releases/latest/download/top.kicad.thumbnail.png) | ![PCB Bottom](../../releases/latest/download/bottom.kicad.thumbnail.png) |

### Oberseite

![PCB Top](../../releases/latest/download/top.kicad.png)

### Unterseite

![PCB Bottom](../../releases/latest/download/bottom.kicad.png)

---

## ℹ️ Projektinformationen

| Eigenschaft | Wert |
|---|---|
| **Projekt** | ThermalDesign |
| **Software** | KiCad 10 |
| **Repository** | TIH-engineering/ThermalDesign |
| **Autor** | [TIH] |
| **Lizenz** | CC BY-NC-SA 4.0 |

---

## 🗂️ Repository-Struktur

```text
.
├── .github/
│   └── workflows/       # GitHub Actions
├── .kibot/              # KiBot-Konfiguration
├── pcb/
│   ├── lib/             # Projektspezifische Bibliotheken
│   └── ...              # KiCad-Projektdateien
├── .gitignore
├── LICENSE
└── README.md