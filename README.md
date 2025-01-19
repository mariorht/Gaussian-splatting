# FastAPI Project Template

![example workflow](https://github.com/mariorht/Gaussian-splatting/actions/workflows/run-tests.yml/badge.svg)


**Gaussian Splatting Project** is a base structure for experimenting with Gaussian splatting techniques. Currently, the most relevant component of the project is located in [notebooks/gaussian_splatting.ipynb](notebooks/gaussian_splatting.ipynb), where interactive experimentation with Gaussian splatting is demonstrated. The rest of the code, intended to implement these features in a web application, is not functional yet.
---

## Setup

### Running in a Virtual Environment (Without Docker)

1. **Prerequisites:**
   - Ensure **Python 3.9** or higher is installed.

2. **Use the `start_venv.sh` Script:**

   From the project's root directory, execute:

   ```bash
   ./setup_venv.sh
   ```

   This script:
   - Creates and activates a virtual environment.
   - Installs dependencies from `src/requirements.txt`.
   - Starts the FastAPI server at `http://127.0.0.1:8001`.

3. **Access the Application:**

   - Open your browser at `http://127.0.0.1:8001` to see the homepage (`index.html`).
   - Navigate to `/hello` to view the basic "Hello" example.

4. **Stop the Server:**

   Press `Ctrl + C` in the terminal to stop the server.

---

### Running with Docker

1. **Prerequisites:**
   - Ensure **Docker** and **Docker Compose** are installed.

2. **Use the `start_docker.sh` Script:**

   From the project's root directory, execute:

   ```bash
   ./start_docker.sh
   ```

   This script automates the steps above:
   - Builds the Docker image.
   - Starts the container using `docker-compose`.

4. **Access the Application:**

   Open your browser at `http://localhost:8001`.

5. **Stop the Project:**

   To stop and remove containers, you can either:
   - Run the command:
     ```bash
     docker-compose down
     ```
   - Or stop the Docker Compose process started by `start_docker.sh` by pressing `Ctrl + C` in the terminal.

---

## Running Tests

To run the tests, you can use the provided script:

```bash
./run_tests.sh
```


