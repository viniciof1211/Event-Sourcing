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

2. (Optional) Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate

3. Install dependencies:
   ```bash
   pip install -r requirements.txt

---

### Usage
#### Running the Example

1. Navigate to the project directory:
      ```bash
      cd src

2. Run the example script:
   ```bash
   python main.py

This will:

- Create a new user by sourcing a UserCreatedEvent to the event store.
- Replay events to reconstruct the state of the user.

#### Example Output
   ```plaintext
   User: john_doe, Email: john@example.com

### Code Structure
   ```plaintext
   event-sourcing-python/
      ├── src/
      │   ├── __init__.py
      │   ├── events.py          # Event base class and concrete events
      │   ├── event_store.py     # Event Store (Hub) implementation
      │   ├── aggregates.py      # Aggregate implementation
      │   ├── services.py        # Microservices implementation
      │   └── main.py            # Example usage
      ├── tests/                 # Unit tests (optional)
      ├── requirements.txt       # Dependencies
      └── README.md              # This file

---

## Extending the Project

- **Add New Events**: Create new event classes by subclassing the `Event` base class.
- **Add New Aggregates**: Implement new aggregates that can apply events and reconstruct their state.
- **Add New Microservices**: Create additional microservices to handle different types of events.

---

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- Inspired by Martin Fowler's [Event Sourcing](https://martinfowler.com/eaaDev/EventSourcing.html) pattern.
- Built with Python's OOP capabilities.

---

## Contact

For questions or feedback, please open an issue or contact [Vinicio S. Flores](mailto:vfloreshdz@gmail.com).
