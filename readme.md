# Code-War

Code-War is a platform designed to simulate a competitive coding environment, similar to LeetCode. It provides a user-friendly interface where users can submit their code, track their progress, and interact with other users. The platform supports multiple programming languages and includes features like sorting questions based on difficulty, a leaderboard, and code submissions tracking.

## Features

- **User Authentication**: Users can create accounts and log in to submit their solutions.
- **Question Sorting**: Questions are sorted by difficulty level and by whether they are solved or not.
- **Leaderboard**: Displays the ranking of users based on the number of problems solved and their performance.
- **Question Description**: Each question includes a description and an integrated code editor.
- **Code Editor & Compiler**: Users can submit their code through an inbuilt code editor that supports multiple languages.
- **Concurrent Submission Handling**: Uses RedisQueue to manage multiple simultaneous code submissions.
- **Container Isolation**: Each user's code submission runs in isolated containers, ensuring security and isolation.
  
## Technologies Used

- **Backend**: Node.js (Express)
- **Frontend**: React.js
- **Database**: MongoDB
- **Containerization**: Docker
- **Queue Management**: RedisQueue
- **Compiler**: Docker containers for code execution
- **Authentication**: JWT (JSON Web Tokens)
- **Deployment**: AWS EC2 (for deployment) & Docker

## Getting Started

To run this project locally, follow these steps:

### Prerequisites

- [Node.js](https://nodejs.org/en/) - JavaScript runtime
- [Docker](https://www.docker.com/) - For containerization
- [Redis](https://redis.io/) - For managing job queues
- [MongoDB](https://www.mongodb.com/) - For storing data

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Devang2304/code-war.git
   cd code-war
2. Install the dependencies for the backend and frontend:
   ```bash
   npm install
    cd client && npm install
3. Set up your environment variables:
   - DATABASE_URI - Your MongoDB URI
   - REDIS_URI - Your Redis URI
   - JWT_SECRET - Secret key for JWT authentication
4. Run the backend and frontend
   
# Running Docker Containers for Code Execution

Each user's code is run in an isolated Docker container for security and isolation. This ensures that malicious code won't affect other users. To set up the Docker environment:

- Ensure Docker is installed and running.
- Build and run the Docker containers

## Acknowledgements

- Thanks to LeetCode for the inspiration.
- Docker for containerization.
- Redis for managing the queue system.

