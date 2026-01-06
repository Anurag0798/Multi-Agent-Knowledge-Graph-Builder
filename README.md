# Multi-Agent Knowledge Graph Builder

Welcome to the Multi-Agent Knowledge Graph Builder! This project is designed to create a roadmap generator for any given topic (e.g., machine learning, data science, DevOps), presenting the roadmap in a graph format. With an advanced multi-agent framework leveraging the Lang ecosystem, this project simplifies creating complex knowledge graphs for effective learning and understanding.

## Project Overview

The goal of this project is to generate a roadmap for any specified topic, represented in a graph format. It utilizes agents, which are autonomous entities performing specific tasks, similar to roles in a company. These agents leverage Large Language Models (LLMs) to automate tasks and generate insights.

## Lang Ecosystem

The project introduces the Lang ecosystem, including:

- **LangChain**: A framework for building logic and creating chains of agents to perform tasks in sequence, ideal for Retrieval Augmented Generation (RAG) applications.
- **LangSmith**: A tool for debugging, monitoring, and visualizing LangChain applications, akin to TensorBoard.
- **LangGraph**: Supports multi-agent workflows, enabling stateful conversations between agents for collaborative interactions.
- **LangServe**: Facilitates the deployment of LangChain applications and agents as APIs.

## Project Architecture

The architecture involves a user interface (built with Streamlit) where users input a topic. This input is processed by a LangGraph workflow consisting of three agents:

1. **Research Agent**: Utilizes the Serper API to search the internet for information related to the input topic.
2. **Synthesizer Agent**: Employs a URI AI LLM to summarize the information gathered.
3. **Mapper Agent**: Creates a graph data structure from the summarized information, generating a visual roadmap using the Graphviz library.

## Practical Implementation

The project implementation includes:

1. Setting up the project folder structure.
2. Creating a new Conda environment and installing packages from `requirements.txt`.
3. Three agents (research, synthesizer, and mapper) with their specific functions.
4. Utilize LangGraph to define the workflow and connect the agents.
5. Generate the visual roadmap with Graphviz.
6. Streamlit app for the user interface.

## Contributing

Contributions are welcome! If you have ideas for enhancements or additional features, feel free to fork the project and submit a pull request.

## License

This project is open-source and available under the MIT License. See the `LICENSE` file for more details.