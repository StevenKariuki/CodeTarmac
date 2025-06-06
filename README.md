# 🕳️ Pothole Spotter

Pothole Spotter is an AI-powered web app that detects, classifies, and visualizes potholes on Kenyan roads. Users upload road images with geo-coordinates, and the system identifies potholes using Azure Custom Vision, displaying results on an interactive map.

---

## 🚀 Features

- Upload road images with GPS data
- AI-based classification using Azure Custom Vision
- Visualize potholes on a Leaflet map with severity markers
- View details on marker click (image, status, timestamp)
- Define road stretches and analyze multiple images

---

## 🧑‍💻 Tech Stack

- **Frontend**: React, Leaflet, TailwindCSS
- **Backend**: Node.js, Express.js
- **AI/ML**: Azure Custom Vision (image classification)
- **Database**: MySQL (smartroads > detections table)
- **Storage**: Static file server / cloud for image uploads

---

## 📂 Project Structure

```bash
pothole-spotter/
├── client/              # React frontend
│   └── src/
├── server/              # Express backend
│   └── uploads/         # Uploaded image storage
├── database/            # SQL scripts / schema
├── .env                 # Environment variables
├── README.md            # You’re here 😎
```

---

## 🛠️ Setup & Run

## 🧠 Local Setup Instructions

1. **Clone the repo**
   ```bash
   https://github.com/PotholePatrol/pothole-spotter.git
   From the branch called Vi_brants_fix
   ```

2. **Create environment file**
   - Copy `.env.example` to `.env` and fill in your details.

3. **Set up MySQL Database**
   - Make sure MySQL is running.
   - Run this command to create the `smartroads` database and `detections` table:
     ```bash
     mysql -u root -p < smartroads_schema.sql
     ```

4. **Install dependencies**
   ```bash
   npm install
   ```

5. **Run the server**
   ```bash
   npm start
   

### Prerequisites:
- Node.js
- MySQL
- Azure Custom Vision account

### Backend:
```bash
cd server
npm install
node index.js
```

### Frontend:
```bash
cd client
npm install
npm start
```

# Setting up Environment

1. Duplicate `.env.example` and rename it to `.env`
2. Fill in your actual keys and DB credentials
3. Do NOT commit the real `.env` file


### Env Config (.env example):
```env
AZURE_ENDPOINT=https://<your-endpoint>.cognitiveservices.azure.com/
AZURE_PREDICTION_KEY=<your-key>
PORT=5000
```

---

## 🧠 Future Features
- Admin dashboard for stats and management
- Export detection data (CSV/PDF)
- User authentication (optional)
- Mobile-first UI revamp

---

## 📸 Sample of the page Preview

![image](https://github.com/user-attachments/assets/0ad1e31a-23ac-409b-b674-debedf55b23a)

![Screenshot 2025-06-03 155719](https://github.com/user-attachments/assets/0a65969a-6161-420d-b282-15d9b882359d)
![Screenshot 2025-06-03 155803](https://github.com/user-attachments/assets/0b901392-31fa-4b40-b7c8-3b575893ee20)

![Screenshot 2025-06-03 155746](https://github.com/user-attachments/assets/41597540-39dc-4f2b-b3c2-1becd117123d)



---

## 🤝 Contributing

PRs are welcome! If you're vibing with the vision, fork the repo, make changes, and drop that pull request 🔥

---

## 🧾 License

MIT License © 2025 Steven Muiruri
