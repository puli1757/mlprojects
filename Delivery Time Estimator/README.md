# Delivery Time Estimator 🚚📦

This project predicts delivery times based on historical data, using a containerized Python application. It is designed for logistics platforms such as DoorDash, Swiggy, or Uber Eats to optimize delivery efficiency.

---

## 📁 Folder Structure

```
.
├── data/                        # Input datasets and data description
├── example_solution/           # Dockerized ML pipeline and prediction logic
│   ├── app/                    # Core ML application code
│   ├── docker-compose.yml      # Orchestrates app containers
│   └── DoorDash Summary.docx   # Report on problem statement & solution
```

---

## 📊 Data Description

- `historical_data.csv`: Contains features like order time, delivery time, distance, traffic conditions, etc.
- `data_to_predict.json`: New orders needing delivery time prediction
- `data_description.txt`: Explanation of dataset fields

---

## 🚀 How to Run

### 1. Build Docker Image
```bash
docker-compose build
```

### 2. Run the App
```bash
docker-compose up
```

### 3. Predict Delivery Time
Send a POST request to the running container with JSON data.

---

## 🧪 Testing

Tests are located in:
```
app/tests/
```
Run tests using:
```bash
docker-compose -f docker-compose.yml run app pytest
```

---

## 🧰 Tech Stack

- Python
- Scikit-learn or similar ML framework
- Docker
- JSON for input/output
- Pytest for testing

---

## 📄 License

This project is provided for educational purposes.

---

## ✍️ Author

Yeswanth Puli
