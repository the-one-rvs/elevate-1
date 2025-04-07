# Express Docker Application

A simple Express.js application containerized with Docker and featuring automated security scanning via GitHub Actions.

## 🚀 Features

- Express.js web server
- Docker containerization
- GitHub Actions pipeline
- Trivy security scanning
- Environment variable support

## 🛠️ Tech Stack

- Node.js with Express.js
- Docker
- GitHub Actions
- Trivy Scanner

## 📦 Installation

1. Clone the repository:
```sh
git clone <your-repo-url>
cd app
```

2. Install dependencies:
```sh
npm install
```

3. Start the application:
```sh
npm start
```

## 🐳 Docker Usage

Build the image:
```sh
docker build -t myapp .
```

Run the container:
```sh
docker run -p 3000:3000 myapp
```

## 🌐 API Endpoints

- `GET /`: Returns "Hello World"
- `GET /go`: Returns "Let's go"

## 🔒 Security

This project uses Trivy for vulnerability scanning through GitHub Actions. Scan results are automatically uploaded as artifacts in the pipeline.

## 📝 Environment Variables

- `PORT`: Server port (default: 3000)

## 🔄 CI/CD Pipeline

The GitHub Actions pipeline ([.github/workflows/pipeline.yaml](.github/workflows/pipeline.yaml)) includes:

1. Docker image building
2. Security scanning with Trivy
3. Scan results archival

## 📄 License

ISC