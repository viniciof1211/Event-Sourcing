# Event Sourcing Enterprise Integration Pattern
Event Sourcing is a powerful architectural pattern where the state of an application is determined by a sequence of events. Instead of storing the current state of an object, the system stores a log of all events that have occurred, enabling features like auditability, temporal queries, and scalability

# Event-Sourcing in Python

[![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

This repository demonstrates the implementation of the **Event Sourcing** design pattern in Python. Event Sourcing is a powerful architectural pattern where the state of an application is determined by a sequence of events. Instead of storing the current state of an object, the system stores a log of all events that have occurred, enabling features like auditability, temporal queries, and scalability.

---

## Features

- **Event Store (Hub)**: A centralized log where all events are stored.
- **Microservices**: Example microservices that source events to the hub.
- **OOP Principles**: Reusable and extensible code following polymorphism, interfaces, and inheritance.
- **Example Use Case**: Create and replay events to reconstruct the state of an aggregate.

---

## Getting Started

### Prerequisites

- Python 3.8 or higher.

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/viniciof1211/Event-Sourcing.git
   cd event-sourcing-python
