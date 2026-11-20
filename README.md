# Traject

**Intelligent Shipment Monitoring and Handling-Event Detection Using IoT and Machine Learning**

Traject is an IoT-based shipment monitoring system designed to observe package conditions during transportation, identify potentially harmful handling events, and support more informed inspection decisions.

The project combines physical sensors, real-time data communication, machine learning, and a web-based monitoring interface to investigate how low-cost IoT technology can improve shipment visibility.

## The Problem

During transportation, packages may experience unexpected impacts, excessive vibration, unfavorable environmental conditions, or unauthorized handling.

Conventional sensor-based monitoring can record these events, but distinguishing routine transportation conditions from potentially harmful incidents remains challenging.

Traject aims to explore this problem through multi-sensor monitoring and intelligent event analysis.

## Proposed Solution

The system is designed around a sensor-equipped shipment prototype that collects movement, environmental, and light measurements.

Sensor readings are transmitted to an IoT backend, where they can be stored, analyzed, and displayed through a monitoring dashboard.

A machine learning component will be developed to distinguish between normal package handling and potentially concerning events.

### Planned Capabilities

- Real-time monitoring of shipment conditions.
- Detection and analysis of movement, vibration, and impacts.
- Temperature and humidity monitoring.
- Identification of potential package-opening events.
- Machine learning-based handling-event classification.
- Event history, visualization, and inspection alerts.
- Recovery from connectivity interruptions and device restarts.

## System Architecture

The proposed system consists of four main layers:

1. **Sensing Layer:** Physical sensors connected to a microcontroller.
2. **Communication Layer:** IoT protocols for transmitting sensor data.
3. **Processing Layer:** Data storage, concurrent processing, and machine learning inference.
4. **Application Layer:** A web dashboard for monitoring shipment conditions and detected events.

## Technology Stack

| Component             | Planned Technology     |
| --------------------- | ---------------------- |
| Microcontroller       | ESP32                  |
| Motion sensing        | MPU6050                |
| Environmental sensing | DHT11 / DHT22          |
| Light sensing         | LDR                    |
| Communication         | MQTT, HTTP, WebSocket  |
| Backend               | Python, FastAPI        |
| Database              | SQLite                 |
| Machine Learning      | Python, scikit-learn   |
| Web Interface         | Python-based dashboard |
| Version Control       | Git, GitHub            |

*The technology stack may be adjusted based on hardware availability and integration testing.*

## Development Roadmap

### Phase 1 — System Foundation

- [ ] Define system requirements and architecture.
- [ ] Integrate at least three physical sensors.
- [ ] Display real-time sensor measurements.
- [ ] Implement the required multithreaded processing structure.
- [ ] Design the machine learning integration and evaluation plan.
- [ ] Validate the initial sensing and processing pipeline.

### Phase 2 — Complete IoT System

- [ ] Assemble the physical shipment prototype.
- [ ] Implement MQTT, HTTP, and WebSocket communication.
- [ ] Develop the web monitoring dashboard.
- [ ] Collect and label handling-event sensor data.
- [ ] Train and evaluate machine learning models.
- [ ] Integrate real-time event classification.
- [ ] Implement automatic startup and connection recovery.
- [ ] Perform end-to-end testing.

## Experimental Evaluation

The project aims to evaluate whether multi-sensor machine learning can distinguish routine package handling from potentially harmful events more effectively than basic threshold-based detection.

Planned evaluation metrics include:

- Classification accuracy and macro F1-score.
- False-positive and false-negative rates.
- Event detection latency.
- Communication and recovery reliability.
- Performance under different handling conditions.

## Physical Prototype

The initial prototype will use a standard cardboard shipping box equipped with low-cost sensors and a microcontroller.

Controlled experiments will simulate normal carrying, vibration, impacts, and package opening.

The prototype is intended to demonstrate handling-event monitoring rather than directly verify damage to the contents of a shipment.

## Project Team

Developed by a five-member student team as part of the CSCI410 Internet of Things course at Nile University, Egypt.

## Project Status

**In development Phase 1**

The repository will be updated as implementation, integration, and experimental evaluation progress.
