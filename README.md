# StreeShield: AI-Powered Deep Fake Detection  

## Overview  

**StreeShield** is an innovative solution designed for **real-time detection of deep fake videos and images**. Utilizing cutting-edge technologies, the project aims to ensure the authenticity of media content, addressing challenges like misinformation and fraud in various domains such as media authentication, social platforms, and law enforcement.  

---

## Problem Statement  
Deep fake media poses significant risks by spreading disinformation and fraud. StreeShield tackles this by leveraging AI to accurately detect deep fakes in real-time, providing a reliable and efficient solution for media verification.  

---

## Features  

### Key Functionalities  
- **AI-Powered Media Detection**: Uses CNN for image detection and 3D CNN for video analysis.  
- **Real-Time Results**: Provides results in under a second for images and under 4 seconds for videos.  
- **Media Type Detection**: Automatically detects whether the uploaded media is an image or video.  
- **Data Augmentation**: Improves model accuracy across varied inputs.  
- **User-Friendly Interface**: Built with ReactJS, the platform offers a seamless experience for media upload and analysis.  
- **Multilingual Support**: Ensures accessibility to a broader audience.  

---

### Backend Features  
- **FastAPI Framework**: Handles communication between the frontend and models.  
- **MongoDB Database**: Efficiently stores user data and model results.  
- **REST APIs**: Enable seamless integration between components.  

---

### Process Flow Architecture  
1. **User Uploads Media**  
2. **Detect Media Type** (Image/Video)  
3. **Preprocess Media** for Analysis  
4. **Run Appropriate Model** (CNN/3D CNN)  
5. **Calculate Confidence Percentages**  
6. **Display Results to the User**  

---

### Technical Feasibility  
- **Models**: CNN and 3D CNN ensure accurate detection.  
- **Scalability**: The solution supports large datasets and higher resolutions.  

---

### Challenges  
- Handling large data volumes for real-time processing, mitigated by optimized algorithms and cloud solutions.  
- Continuous model improvement to minimize potential glitches and enhance accuracy.  

---

### Use Cases  
- **Media Authentication**: Validates the authenticity of news and social media content.  
- **Social Media Platforms**: Detects deep fakes to combat misinformation.  
- **Law Enforcement**: Confirms video evidence for investigations.  

---

## Deployment  

### Prerequisites  
1. **Node.js** for frontend.  
2. **Python 3.8+** for backend.  
3. **MongoDB** for database.  
4. Virtual environment setup for Python.  

---

### Frontend Deployment  

1. Navigate to the frontend folder:  
```bash  
cd frontend
```
2. Install dependencies:
```bash
npm install
```
3. Run the development server:
```bash
npm run dev
``` 
The frontend will be accessible at http://localhost:3000.
---
### Backend Deployment
1. Navigate to the backend folder:
```bash
cd backend
```  
2. Create and activate a virtual environment:
* For Windows:
```bash
python -m venv env  
source env/Scripts/activate
```
* For Linux/Mac:
```bash
python3 -m venv env  
source env/bin/activate
```
3. Install dependencies:
```bash
pip install -r requirements.txt
``` 
4. Run the FastAPI server:
```bash
uvicorn main:app --reload
```

The backend will be accessible at http://127.0.0.1:8000.
---
### Database Setup
1. Ensure MongoDB is installed and running.
2. Configure the database URL in the backend environment file (.env).
---
### Future Enhancements
* Adding detailed confidence levels for applications like forensic investigations.
* Expanding support for high-resolution media and larger datasets.
