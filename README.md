# Wikipedia Research Assistant

A **Model Context Protocol (MCP)**-powered research assistant that enables natural language interaction with Wikipedia. This Python-based agent processes free-form questions, queries Wikipedia's Python package, and returns relevant, summarized results through an MCP-compatible interface.

## Features

* **MCP Agent Integration** – Leverages the Model Context Protocol to support tool-based interaction.
* **Natural Language Interface** – Accepts free-text queries and interprets user intent.
* **Wikipedia Content Retrieval** – Uses the Wikipedia Python package to fetch article content.
* **Summarization Support** – Processes and condenses information for easier consumption.

## Getting Started

### Prerequisites

* Python 3.11

### Clone the Repository

```bash
git clone https://github.com/Palwisha-18/wikipedia_research_assistant.git
cd wikipedia_research_assistant
```

### Set Up a Virtual Environment

```bash
python3.11 -m venv venv
```

Activate the environment:
* On macOS/Linux:

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

### Configure Environment Variables

Create a `.env` file in the project root directory:

```bash
touch .env
```

Example content for `.env`:

```env
BASE_URL=
API_KEY=
```

### Run the MCP Client

To start the assistant:

```bash
python mcp_client.py
```

Example interaction:

```text
You: Tell me about photosynthesis.
Processing request of type CallToolRequest
AI: Photosynthesis is a system of biological processes by which photosynthetic organisms, such as most plants, algae, and cyanobacteria, convert light energy, typically from sunlight, into the chemical energy necessary to fuel their metabolism. Photosynthesis usually refers to oxygenic photosynthesis, a process that produces oxygen. Photosynthetic organisms store the chemical energy so produced within intracellular organic compounds (compounds containing carbon) like sugars, glycogen, cellulose and starches. To use this stored chemical energy, an organism's cells metabolize the organic compounds through cellular respiration. Photosynthesis plays a critical role in producing and maintaining the oxygen content of the Earth's atmosphere, and it supplies most of the biological energy necessary for complex life on Earth.

Some bacteria also perform anoxygenic photosynthesis, which uses bacteriochlorophyll to split hydrogen sulfide as a reductant instead of water, producing sulfur instead of oxygen. Archaea such as Halobacterium also perform a type of non-carbon-fixing anoxygenic photosynthesis, where the simpler photopigment retinal and its microbial rhodopsin derivatives are used to absorb green light and power proton pumps to directly synthesize adenosine triphosphate (ATP), the "energy currency" of cells.

In plants, algae, and cyanobacteria, sugars are synthesized by a subsequent sequence of light-independent reactions called the Calvin cycle. In this process, atmospheric carbon dioxide is incorporated into already existing organic compounds, such as ribulose bisphosphate (RuBP). Using the ATP and NADPH produced by the light-dependent reactions, the resulting compounds are then reduced and removed to form further carbohydrates, such as glucose.
```
