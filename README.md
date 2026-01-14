# Gemini Agent Development Kit (ADK) - Sample Project

This project contains sample agents built using the Gemini Agent Development Kit (ADK).

## Project Structure

- `agent.py`: A simple agent that can tell the current time.
- `step_1/agent.py`: A more advanced agent that can fetch weather information for different cities.

## Getting Started

### Prerequisites

- Python 3.7+
- Gemini ADK installed

### Installation

1. Clone this repository:
   ```bash
   git clone <repository-url>
   ```
2. Navigate to the project directory:
   ```bash
   cd job_adk
   ```
3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```
   *(Note: A `requirements.txt` file does not exist yet. You will need to create one based on the imports in the `agent.py` files.)*

### Running the Agents

#### Simple Time Agent

To run the simple time agent, execute the following command:

```bash
adk run agent.py
```

#### Weather Agent

To run the weather agent, execute the following command:

```bash
adk run step_1/agent.py
```

## Agents

### Simple Time Agent (`agent.py`)

This is a basic agent that demonstrates the fundamental structure of a Gemini ADK agent. It has one tool:

- `get_current_time(city: str)`: Returns the current time for a given city. (Currently, it's a mock that always returns "10:30 AM").

### Weather Agent (`step_1/agent.py`)

This is a more advanced agent that showcases more features of the Gemini ADK, including:

- A more detailed tool with mock data.
- More descriptive agent instructions.
- Use of a specific Gemini model.

The agent has one tool:

- `get_weather(city: str)`: Returns the weather for a given city. The agent uses a mock database to provide weather information for "New York", "London", and "Tokyo".
