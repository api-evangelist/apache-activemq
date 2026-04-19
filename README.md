# Apache ActiveMQ (apache-activemq)
Apache ActiveMQ is an open-source, high-performance message broker written in Java, developed by the Apache Software Foundation. It implements the Jakarta Messaging (JMS) API and supports multiple messaging protocols including AMQP, STOMP, MQTT, OpenWire, and HTTP/WebSocket, enabling reliable asynchronous messaging between distributed applications and microservices. ActiveMQ provides features such as network of brokers, message persistence (KahaDB, JDBC), high availability, message scheduling, and a web console with REST and Jolokia management APIs.

**URL:** [https://activemq.apache.org/](https://activemq.apache.org/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - AMQP, Apache, Java, JMS, Message Broker, Messaging, MQTT, Open Source, STOMP

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-04-19

## APIs

### Apache ActiveMQ REST API
The ActiveMQ REST API provides HTTP-based access to messaging operations, allowing clients to produce and consume messages from queues and topics without a native JMS client. It supports sending messages via POST, receiving via GET, and subscribing with client IDs for persistent consumption.

**Human URL:** [https://activemq.apache.org/components/classic/documentation/rest](https://activemq.apache.org/components/classic/documentation/rest)

#### Tags

 - Messaging, REST

#### Properties

- [Documentation](https://activemq.apache.org/components/classic/documentation/rest)
- [OpenAPI](openapi/apache-activemq-rest-openapi.yaml)

### Apache ActiveMQ Jolokia Management API
The Jolokia JMX-HTTP bridge API provides HTTP access to JMX metrics and management operations for the ActiveMQ broker, enabling monitoring of broker health, queue depths, consumer counts, and other operational metrics without requiring a JMX client.

**Human URL:** [https://activemq.apache.org/components/classic/documentation/web-console](https://activemq.apache.org/components/classic/documentation/web-console)

#### Tags

 - Management, Monitoring, JMX

#### Properties

- [Documentation](https://activemq.apache.org/components/classic/documentation/web-console)

### Apache ActiveMQ Broker
The ActiveMQ Classic broker provides high-performance asynchronous messaging through multiple protocol interfaces including OpenWire, AMQP, STOMP, and MQTT. It includes a web-based management console, message persistence, network of brokers for load distribution, and high availability configurations.

**Human URL:** [https://activemq.apache.org/components/classic/documentation](https://activemq.apache.org/components/classic/documentation)

#### Tags

 - Broker, Messaging

#### Properties

- [Documentation](https://activemq.apache.org/components/classic/documentation)
- [GettingStarted](https://activemq.apache.org/components/classic/documentation/getting-started)

## Common Properties

- [GitHubOrganization](https://github.com/apache)
- [GitHubRepository](https://github.com/apache/activemq)
- [Documentation](https://activemq.apache.org/)
- [GettingStarted](https://activemq.apache.org/components/classic/documentation/getting-started)
- [FAQ](https://activemq.apache.org/faq)
- [Support](https://activemq.apache.org/support)
- [TermsOfService](https://www.apache.org/licenses/)
- [ChangeLog](https://activemq.apache.org/components/classic/download)

## Features

| Name | Description |
|------|-------------|
| Multi-Protocol Support | Supports AMQP, STOMP, MQTT, OpenWire, JMS, Jakarta Messaging, HTTP, and WebSocket protocols for broad client compatibility. |
| Message Persistence | Provides KahaDB and JDBC-based message persistence options to ensure message durability across broker restarts. |
| Network of Brokers | Enables distributed messaging topologies by linking multiple brokers in a network for load balancing and failover. |
| High Availability | Supports shared storage and master-slave configurations for high availability deployments. |
| Message Scheduling | Built-in message scheduling capabilities allow delayed or recurring message delivery. |
| REST Messaging API | HTTP-based REST API for producing and consuming messages from queues and topics without native JMS clients. |
| Jolokia Management API | JMX-over-HTTP bridge via Jolokia for broker monitoring and management. |
| Web Console | HTML5 web-based management console accessible at /admin for queue and topic management, subscriber monitoring, and message browsing. |
| Docker Support | Official Docker image apache/activemq-classic available on Docker Hub for containerized deployments. |
| Embeddable Broker | ActiveMQ can be embedded directly into Java applications for in-process messaging. |

## Use Cases

| Name | Description |
|------|-------------|
| Microservices Messaging | Decouple microservices using asynchronous message queues and topics for event-driven architectures. |
| Enterprise Integration | Connect disparate enterprise systems and applications using standard messaging protocols. |
| IoT Messaging | Use MQTT protocol support for IoT device communication and telemetry data pipelines. |
| Workload Distribution | Distribute work items across consumer pools using competing consumers on queues. |
| Event Streaming | Publish events to topics and fan out to multiple subscriber applications. |
| Legacy JMS Integration | Bridge legacy JMS-based applications with modern services using OpenWire and JMS API support. |

## Integrations

| Name | Description |
|------|-------------|
| Spring Framework | Deep integration with Spring and Spring Boot via spring-boot-starter-activemq. |
| Apache Camel | Native Apache Camel ActiveMQ component for enterprise integration patterns. |
| Docker | Official Docker Hub image apache/activemq-classic for containerized deployments. |
| Kubernetes | Deployable on Kubernetes using the official Docker image and StatefulSets. |
| Hawtio | HTML5 management console integration via hawtio for advanced broker management. |
| RHQ | Operational monitoring integration with RHQ for enterprise monitoring. |
| Apache Karaf | OSGi integration with Apache Karaf for modular enterprise deployments. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Apache ActiveMQ REST API](openapi/apache-activemq-rest-openapi.yaml)

### JSON Schema

- [Jolokia Response](json-schema/rest-jolokia-response-schema.json)
- [Jolokia Error](json-schema/rest-jolokia-error-schema.json)

### JSON Structure

- [Jolokia Response Structure](json-structure/rest-jolokia-response-structure.json)
- [Jolokia Error Structure](json-structure/rest-jolokia-error-structure.json)

### JSON-LD

- [Apache ActiveMQ REST Context](json-ld/apache-activemq-rest-context.jsonld)

### Examples

- [Jolokia Response Example](examples/rest-jolokia-response-example.json)
- [Jolokia Error Example](examples/rest-jolokia-error-example.json)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Apache ActiveMQ REST API](capabilities/shared/activemq-rest.yaml) — 3 operations for messaging and broker management

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Apache ActiveMQ Messaging Workflow](capabilities/activemq-messaging.yaml) | ActiveMQ REST | 3 | Application Developer, Platform Operator |

## Vocabulary

- [Apache ActiveMQ Vocabulary](vocabulary/apache-activemq-vocabulary.yaml) — Unified taxonomy mapping 4 resources, 5 actions, 1 workflow, and 2 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [Apache ActiveMQ Spectral Rules](rules/apache-activemq-spectral-rules.yml) — 19 rules across 7 categories enforcing Apache ActiveMQ API conventions

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
