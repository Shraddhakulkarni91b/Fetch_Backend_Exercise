# Exercise

# Receipt Processor

A simple web service to process receipts and calculate reward points based on predefined rules.

## Features
- Submit a receipt to calculate reward points.
- Retrieve points for a submitted receipt using a unique ID.

## Technologies Used
- Go (Golang) for backend development.
- Docker for containerization.

### Run Locally
1. Clone the repository:

2. Navigate to the project directory:
    cd cmd/

3. Install dependencies and run the app:<br>
    go mod tidy <br>
    go run main.go

### Run with Docker
1. Build the Docker image:
    docker build -t receipt-processor .

2. Run the Docker container:
    docker run -p 8080:8080 receipt-processor

### API Endpoints
1. Submit a Receipt
    Endpoint: POST /receipts/process
    URL - http://localhost:8080/receipts/process

2. Get Points for a Receipt
    Endpoint: GET /receipts/{id}/points
    URL - http://localhost:8080/receipts/{id}/points
