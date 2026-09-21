# 🌦️ Weather API

A simple **RESTful Weather API built with Python, Flask, and Pandas** that provides historical temperature data from weather stations.

This project was built to understand how APIs work, how Flask handles routes and requests, and how data can be processed and served through API endpoints.

## 🚀 Features

* View available weather stations
* Get temperature data for a specific station and date
* Get all available data for a weather station
* Get weather data for a specific year
* Return data in JSON format
* Display available weather stations through a simple web page

## 🛠️ Technologies Used

* **Python**
* **Flask** – for building the web API
* **Pandas** – for reading and processing weather datasets
* **HTML** – for the basic web interface

## 📁 Project Structure

```text
Weather_API/
│
├── data_small/
│   ├── stations.txt
│   └── TG_STAIDxxxxxx.txt
│
├── templates/
│   └── home.html
│
├── main.py
└── README.md
```

## 🔗 API Endpoints

### 1. Get Available Weather Stations

```text
GET /
```

Displays the available weather stations.

---

### 2. Get Temperature for a Specific Date

```text
GET /api/v1/<station>/<date>
```

Example:

```text
/api/v1/000001/19900101
```

Example response:

```json
{
    "station": "000001",
    "date": "19900101",
    "temperature": 5.2
}
```

---

### 3. Get All Data for a Station

```text
GET /api/v1/<station>
```

Example:

```text
/api/v1/000001
```

Returns the available weather records for the selected station.

---

### 4. Get Data for a Specific Year

```text
GET /api/v1/yearly/<station>/<year>
```

Example:

```text
/api/v1/yearly/000001/1990
```

Returns the weather records available for the selected station during that year.

## ⚙️ How to Run

### 1. Clone the repository

```bash
git clone https://github.com/ayushmohod477/Weather_Api
```

### 2. Navigate to the project folder

```bash
cd Weather_API
```

### 3. Install dependencies

```bash
pip install flask pandas
```

### 4. Run the application

```bash
python main.py
```

The application will start locally.

Open:

```text
http://127.0.0.1:5000/
```

## 📚 What I Learned

Building this project helped me understand:

* How Flask applications work
* How to create API routes
* How URL parameters are used in APIs
* How to read and process datasets using Pandas
* How to filter data based on user requests
* How Python applications return JSON responses
* The basic structure of a REST API

## 🔮 Future Improvements

Some improvements I would like to add in the future:

* Add proper error handling
* Validate station IDs and dates
* Return appropriate HTTP status codes
* Improve API documentation
* Optimize data loading
* Add more weather parameters
* Deploy the API online

## 👨‍💻 Author

**Ayush Mohod**

Built as a learning project to understand Python, Flask, APIs, and data processing.

---

⭐ If you find this project useful, feel free to explore the repository.
