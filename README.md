# KrishiAI (PlantCare AI)

KrishiAI is an integrated agricultural assistant encompassing a machine learning-powered backend for plant disease detection and a responsive frontend for farmers to interact with the system.

## Project Structure

This repository is split into two main components:
*   **`frontend/`**: The web application built with React and Vite.
*   **`backend/`**: The FastAPI server that handles ML inference (using TensorFlow) and serves the API.

---

## 🚀 Getting Started

To run the full KrishiAI application locally, you will need to start both the backend and frontend servers. Each directory has its own setup and run scripts.

### 1. Backend Setup and Run

The backend is a Python-based FastAPI application using TensorFlow for machine learning models.

**Prerequisites**: Python 3.11 (recommended for TensorFlow compatibility on macOS ARM64).

```bash
cd backend

# Setup the virtual environment and install dependencies
bash local_setup.sh

# Start the FastAPI server (runs on port 5001)
bash local_run.sh
```
*Note: The backend runs on `http://localhost:5001/`.*

### 2. Frontend Setup and Run

The frontend is built with React, Vite, and TailwindCSS.

**Prerequisites**: Node.js and npm.

```bash
cd frontend

# Install the necessary dependencies (using legacy-peer-deps to avoid conflicts)
npm install --legacy-peer-deps

# Start the Vite development server
npm run dev
```
*Note: The frontend will typically run on `http://localhost:5174/` or `http://localhost:5173/` depending on port availability.*

---

## Features

*   **Plant Disease Detection**: Upload or capture images of plant leaves to identify potential diseases using our MobileNetV2-based model.
*   **Real-time AI Chatbot**: Get quick answers to agricultural queries.
*   **Responsive Dashboard**: An easy-to-use interface tailored for ease of access.

## License

This project is licensed under the MIT License.
