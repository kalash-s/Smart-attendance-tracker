# Smart-attendance-tracker

This is a **Machine Learning project** developed during our sophomore year using **Python** and **OpenCV**. It automates the process of recording attendance through face recognition and stores the results in a neatly formatted Excel sheet.

---

## Features

- Face recognition to detect and identify students in real time.
- Automatically logs attendance details into an Excel sheet.
- Outputs include:
  - College name and lecture title (customizable).
  - Number of students **present**, **absent**, and **percentage present**.
  - Names of students **present** along with **timestamps**.
## Inputs Required

1. **Total number of students**
2. **Lecture name**
3. **Facial images** of students attending the lecture

---

### 1. Create Dataset

Run `face_dataset.py` to collect face images of each student.  
Follow this detailed guide:  
https://www.pyimagesearch.com/2018/06/11/how-to-build-a-custom-face-recognition-dataset/

### 2. Generate Face Encodings

Run `face_enc.py` to convert collected face data into encodings used for recognition.

### 3. Run Attendance System

Run `face_recog.py` to:
- Start real-time face recognition
- Match detected faces with the dataset
- Automatically record attendance

Each session generates a **new Excel file** with the attendance details.


## Output

Each time the system is run, an Excel sheet is created containing:
- College and lecture name
- Number of students present
- Number of students absent
- Attendance percentage
- Names of students present with time stamps

---

## Technologies Used

- Python 
- OpenCV 
- Face Recognition Library 
- Pandas 
- Excel File Generation (XLSX) 

---

## Notes

- Make sure all dependencies are installed before running the project.
- Face dataset must be created before running the attendance script.
