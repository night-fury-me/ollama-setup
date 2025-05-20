## ollama-setup

### Introduction

This project aims to set up and configure Ollama, a tool for managing and deploying machine learning models.

### Prerequisites

-   Docker
-   Docker Compose
-   Git

### Installation

Clone the repository:

```bash
git clone https://github.com/night-fury-me/ollama-setup.git
cd ollama-setup
```

### Docker Setup

To set up the Docker containers for Ollama and Open WebUI, use the provided `docker-compose.yml` file.

### Starting the Containers

To start the Docker containers, run the following command in the root directory of the project:

```bash
docker-compose up -d
```

### Stopping the Containers

To stop the Docker containers, run:

```bash
docker-compose down
```

### Pulling and Running Models

To pull and run models from Ollama, you can use the following command. For example, to pull the `deepseek-r1` 671b quantized model, use:

```bash
docker exec -it ollama ollama pull secfa/DeepSeek-R1-UD-Q2_K_XL
```

### Access the Open WebUI

```bash
http://localhost:3000/
```

visite the above link to Access Ollama and its installed model with GUI.

**Note:** For linux the connection needs to be updated with: `http://ollama:11434` instead of `http://host.docker.internal:11434`

-   Open Open WebUI at http://localhost:3000
-   Go to Settings → Connections → Ollama API
-   Click ✏️ to edit the connection
-   Replace `http://host.docker.internal:11434` with `http://ollama:11434`

### License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

### Contact

For any questions or suggestions, please open an issue or contact the project maintainer at karim.redwanul@outlook.com
