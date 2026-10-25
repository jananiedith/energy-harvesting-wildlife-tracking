System Architecture

1. Introduction

The proposed system integrates wildlife location tracking, wireless communication, and energy harvesting to develop a low-power wildlife monitoring prototype.

The architecture is divided into an energy subsystem, a tracking tag, a wireless communication link, and a receiver with a monitoring interface.

2. System Block Diagram

          
flowchart TD
    subgraph E["Energy Harvesting Subsystem"]
        S["Solar Panel"]
        P["Piezoelectric Harvester"]
        M["Energy Management Circuit"]
        B["Rechargeable Battery"]
        S --> M
        P --> M
        M --> B
    end

    subgraph T["Wildlife Tracking Tag"]
        G["GPS Module"]
        C["Microcontroller"]
        L1["LoRa Transmitter"]
        G --> C
        C --> L1
    end

    B -.-> C
    L1 -->|"Wireless Data"| L2["LoRa Receiver"]
    L2 --> D["Data Processing"]
    D --> H["Monitoring Dashboard"]

    H --> I["Tag ID, Location, Timestamp, Battery Status"]
    
                                           

3. Energy Subsystem

The energy subsystem explores solar and piezoelectric energy harvesting.

The harvested energy must pass through suitable power-management circuitry before it can safely charge an appropriate rechargeable battery or supply the electronics.

The actual charging arrangement depends on the selected battery chemistry, harvester output, and charging circuit.

4. Tracking Subsystem

The tracking tag contains a GPS receiver and a microcontroller.

The GPS receiver provides location information when satellite reception is available. The microcontroller processes the available location data and prepares a tracking message containing fields such as tag ID, latitude, longitude, and battery status.

5. Wireless Communication Subsystem

A compatible wireless transmitter sends tracking messages to a receiver.

If LoRa SX1278 modules are selected, both ends must use compatible radio settings and an appropriate permitted frequency for the deployment region.

Communication performance will be evaluated experimentally.

6. Receiver and Dashboard

The receiver obtains wireless packets and forwards the received data to a computer or dashboard.

The proposed interface may display:

- Tag identification.
- Latitude and longitude.
- Timestamp.
- Battery voltage.
- Received signal strength, when supported by the receiver.

Missing or invalid GPS readings should be identified rather than displayed as valid locations.

7. Data Flow

1. The energy subsystem collects available energy.
2. The power-management circuit supplies the electronics.
3. The GPS receiver obtains location information.
4. The microcontroller prepares a tracking packet.
5. The wireless transmitter sends the packet.
6. The receiver processes the packet.
7. The dashboard displays available tracking information.

8. Design Considerations

The design should account for energy availability, power consumption, radio range, GPS accuracy, antenna placement, enclosure protection, tag size, and animal safety.

The prototype will first be tested under laboratory conditions. Field deployment requires additional validation and appropriate permissions.

9. Implementation Status

This document describes the proposed architecture. Actual hardware connections, measured performance, and implemented features will be updated as development progresses.
