# 📡 HealthSync Service Registry

Netflix Eureka Service Registry providing dynamic service discovery for MediCare HealthSync microservices.

## Student Information

| Field | Details |
|---|---|
| Student Name | Matheesha Abiman |
| Student Number | 241722050 |
| Slack Handle | [YOUR SLACK HANDLE - OPTIONAL] |
| GCP Project ID | `[YOUR GCP PROJECT ID]` |

## Project Description

The Service Registry maintains the locations and availability of active microservice instances. This enables load-balanced service-to-service communication and dynamic discovery.

## Service Information

| Property | Value |
|---|---|
| Technology | Netflix Eureka |
| Port | `9001` |
| Dashboard | `http://localhost:9001` |
| Function | Dynamic service discovery |

## Registered Business Services

- `PATIENT-SERVICE` — Port `8000`
- `DOCTOR-SERVICE` — Port `8001`
- `APPOINTMENT-SERVICE` — Port `8002`

## Architecture

```text
                 Eureka :9001
                    |
        +-----------+-----------+
        |           |           |
        v           v           v
   Patient       Doctor    Appointment
   :8000         :8001         :8002
```

## Technology Stack

- Java
- Spring Boot 3
- Spring Cloud
- Maven
- REST APIs
- Git and GitHub
- Google Cloud Platform (GCP)

## Getting Started

### Prerequisites

- JDK 21 or 25
- Maven
- Git
- MySQL and/or MongoDB as required by the service
- Node.js and npm for the web application
- GCP access for cloud deployment

### Clone

```bash
git clone <REPOSITORY_URL>
cd <REPOSITORY_FOLDER>
```

### Run

```bash
mvn clean install
mvn spring-boot:run
```

After startup, open:

```text
http://localhost:9001
```

## Parent Repository

Part of [medicare-healthsync-platform](https://github.com/Matheesha-Abiman/medicare-healthsync-platform).
