# Raksha-net
A resilient disaster communication system using ESP32, LoRa mesh networking, GNSS and AI-based message prioritization (integration).

### Disaster Mesh Communication Network

A resilient emergency communication system designed to enable communication during disasters when conventional cellular and internet networks are unavailable.

---

##  Problem

During disasters such as floods, earthquakes, landslides and other emergencies, conventional communication infrastructure can become unavailable.

This can make it difficult for:

- Victims to send SOS messages
- Rescue teams to receive accurate locations
- Emergency information to reach command centers
- Rescue teams to coordinate effectively

---

##  Our Solution

**Raksha-Net** uses a decentralized LoRa-based mesh network to provide communication between field devices without depending on cellular networks or the internet.

### System Architecture


📱 User Phone
      │
      │ Wi-Fi / Bluetooth
      ▼
┌─────────────────┐
│  Raksha-Net Node│
│     ESP32       │
│  + GNSS + LoRa  │
└────────┬────────┘
         │
         │ LoRa Mesh
         ▼
   ┌─────────────┐
   │ Mesh Nodes  │
   │  Node → Node│
   └──────┬──────┘
          │
          ▼
┌──────────────────┐
│ Gateway / Rescue │
│   Communication │
└────────┬─────────┘
         │
         ▼
   Rescue Dashboard
         │
         ▼
      AI Layer




##  Communication

Raksha-Net uses LoRa-based multi-hop communication to transmit emergency information across the mesh network.

Key concepts include:

- Multi-hop communication
- Store-and-forward messaging
- Self-healing mesh
- SOS prioritization
- Location sharing
- Route selection

# AI Integration

The AI layer is designed to assist the emergency communication system by:

Classifying emergency messages
Prioritizing SOS information
Assisting route selection
Considering factors such as signal strength, battery level and network conditions

The goal is to ensure that critical emergency information receives higher priority within the network.

# Hardware

The emergency node prototype consists of:

ESP32
LoRa communication module
GNSS/GPS module
SOS push button
SOS LED
Buzzer
Battery power system
3.3V voltage regulation
USB-C interface

# PCB Design

The PCB was designed using KiCad.

PCB 3D Model

The PCB integrates the controller, communication interfaces, emergency interface and power circuitry into a compact prototype.



# Repository Structure
Raksha-Net/
│
├── Hardware/
│   ├── KiCad/
│   │   ├── Emergency_LoRa_Node.kicad_pro
│   │   ├── Emergency_LoRa_Node.kicad_sch
│   │   └── Emergency_LoRa_Node.kicad_pcb
│   │
│   └── 3D/
│       └── PCB_3D_Render.png
│
├── Documentation/
│
├── Media/
│
└── README.md


## Smart India Hackathon 2026

Problem Statement: SIH26223
Domain: Hardware – Disaster Management

Team SIX MVPs
Manthan Gurav — Project Lead
Viraj Patil
Vaishnav Patil
Parul Sharma
Shreya Singh
Soham Nikam


## Project Status

The current PCB is a prototype design intended for demonstration and validation.

The exact commercially purchased components and footprints should be verified before manufacturing the final PCB.

## Project Demonstration

YouTube demonstration coming soon.

## License

This project is developed as part of Smart India Hackathon 2026.

