# energy-harvesting-wildlife-tracking
 A low-power wireless wildlife tracking prototype using energy-harvesting tags.


Wireless Wildlife Tracking System Powered by Energy Harvesting Tags

1. Project Overview

The Wireless Wildlife Tracking System Powered by Energy Harvesting Tags is a proposed low-power wildlife monitoring system designed to track animal locations and monitor the status of tracking tags.

The system combines GPS-based location tracking, wireless communication, and energy harvesting techniques to explore a sustainable approach to wildlife monitoring.

Solar energy and piezoelectric energy harvesting are considered to supplement the energy supply of the tracking tag.

2. Problem Statement

Wildlife tracking systems require a reliable power source for location sensing and wireless data transmission. Frequent battery replacement can be difficult in remote environments and may disturb wildlife.

This project aims to develop a prototype that investigates energy harvesting and low-power wireless communication to support wildlife tracking with reduced maintenance requirements.

3. Objectives

- Develop a prototype for wireless wildlife tracking.
- Obtain geographical location information using a GPS module.
- Transmit tracking information wirelessly to a receiver.
- Explore solar and piezoelectric energy harvesting.
- Monitor battery status and evaluate power consumption.
- Test wireless communication range and location accuracy.
- Consider animal safety, tag weight, and environmental protection.

4. Proposed System Architecture

The system consists of two main sections.

A. Wildlife Tracking Tag

- Microcontroller
- GPS module
- Wireless transmitter
- Energy-harvesting sources
- Energy management circuit
- Rechargeable battery

B. Receiver and Monitoring System

- Wireless receiver
- Data processing software
- Monitoring dashboard
- Tracking information display

5. Proposed Hardware Components

- ESP32 or another suitable microcontroller
- NEO-6M GPS module
- LoRa SX1278 wireless module
- Solar panel
- Piezoelectric transducer
- Suitable energy harvesting and charging circuit
- Rechargeable battery with appropriate protection
- Receiver and monitoring computer

The final components will be confirmed during prototype development.

6. Proposed Software Tools

- Arduino IDE
- Embedded C/C++
- GitHub for source code management
- Serial Monitor for debugging
- Dashboard software, if implemented

7. Expected Outcomes

The prototype is intended to demonstrate location-data acquisition, wireless data transmission, and evaluation of harvested energy and power consumption.

Actual performance will be documented after testing.

8. Testing and Evaluation

The following tests are planned:

1. GPS location acquisition.
2. Wireless data transmission and reception.
3. Communication range measurement.
4. Energy-harvesting voltage and current measurement.
5. Battery performance and power consumption analysis.
6. System reliability and environmental suitability assessment.

9. Animal Safety and Ethical Considerations

Initial testing will be conducted using a laboratory prototype rather than attaching an unvalidated device to a wild animal.

Any future animal testing must consider tag weight, attachment method, radio exposure, waterproofing, and applicable wildlife permissions.

10. Current Project Status

Project stage: Initial development.

The hardware, firmware, and monitoring software will be developed and tested progressively. Completed features and measured results will be updated in this repository.

11. Future Enhancements

- Improved low-power operation.
- Energy-aware transmission scheduling.
- Battery and harvested-energy monitoring.
- Real-time tracking dashboard.
- Long-term field testing following appropriate approvals.
