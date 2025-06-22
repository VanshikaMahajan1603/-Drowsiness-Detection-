# 🛣️ Real-Time Hypnosis Detection: Video-Based Monitoring for Enhanced Safety

A machine learning-based real-time monitoring system designed to detect signs of driver drowsiness and prevent accidents caused by highway hypnosis.

---

## Project Description

**Situation**
Highway hypnosis, or "Driving Without Attention Mode," is a psychological phenomenon where drivers unknowingly enter a trance-like state during long, monotonous drives—often with fatal consequences. As per government data, over 190 accidents on the Nagpur-Mumbai Samruddhi Expressway between Dec 2022 and July 2023 were linked to driver drowsiness and related factors.

**Task**
To develop a real-time detection system using computer vision and deep learning to identify driver drowsiness, a key symptom of road hypnotism, and issue timely alerts—thereby reducing the risk of accidents and enhancing road safety.

**Action**

* Conducted **exploratory data analysis** on national highway accident trends using data from the Ministry of Road Transport and Highways.
* Used the **NITYMED dataset**, consisting of 53,331 labeled images, to train the model. The dataset included facial recordings of drivers under night-time driving conditions.
* Applied **Convolutional Neural Networks (CNNs)** to extract features related to **eye closure and yawning**, indicative of drowsiness or hypnosis.
* Developed a real-time pipeline involving:

  * **Video frame extraction**
  * **Eye and mouth region detection**
  * **Pattern recognition and alert triggering**
* Used **Python**, **TensorFlow**, **Keras**, **OpenCV**, and **NumPy** to implement the model in **Jupyter Notebook**.
* Deployed the system for **real-time monitoring**, issuing alerts when symptoms like microsleep or yawning were detected.

**Result**

* Achieved an **accuracy of 92.29%** in detecting drowsiness using visual cues.
* The system provides **live analysis and alert notifications**, making it a practical safety tool for long-distance drivers.
* Visual learning curves for accuracy and loss over epochs demonstrated strong model performance and generalization.

---

## Objectives

* Detect driver drowsiness and highway hypnosis symptoms in real time.
* Analyze accident data across road types, open areas, and high-risk states to identify critical safety patterns.
* Minimize the number of accidents due to inattentive driving through proactive alert mechanisms.

---

## Dataset

* **Name**: Night-Time Yawning-Microsleep-Eyeblink-Driver Distraction (NITYMED)
* **Size**: 130 driver recordings (cleaned dataset with 53,331 images)
* **Labels**: Yawning (mouth open ≥ 2.5 cm), Microsleep (eyes closed), Eye blinking removed
* **Diversity**: Includes variations in facial features (beard, glasses, hair color)

---

## Technologies & Tools

| Category   | Tools & Frameworks                                 |
| ---------- | -------------------------------------------------- |
| Language   | Python 3.9.13                                      |
| IDE        | Jupyter Notebook                                   |
| Libraries  | TensorFlow, Keras, OpenCV, NumPy                   |
| Model Type | Convolutional Neural Network (CNN)                 |
| Processing | Image segmentation, binarization, region detection |

---

## System Workflow

1. **Video Monitoring**
2. **Frame Extraction**
3. **Eye and Mouth Region Detection**
4. **Preprocessing (Segmentation & Binarization)**
5. **Feature Extraction (Eye state, Yawning patterns)**
6. **CNN Classification**
7. **Real-Time Alert Generation**

---

## Results

* **Model Accuracy**: 92.29%
* **Metrics Tracked**: Training and validation accuracy/loss over epochs
* **Alerts**: Triggered when eye closure or yawning patterns are detected
* **Application**: Can be integrated into in-car safety systems for commercial drivers or fleet monitoring

---

## Challenges Addressed

* Accurately detecting drowsiness despite subtle facial variations
* Managing real-time video processing with minimal delay
* Handling dataset bias and ensuring generalization for unknown drivers

---

## Future Enhancements

* Integrate **multi-modal data** (e.g., steering angle, heart rate) for higher accuracy.
* Deploy on **embedded devices** like Raspberry Pi for use in actual vehicles.
* Extend to detect **emotional fatigue**, **distraction**, and **stress levels**.
* Build a **mobile or web-based dashboard** for fleet monitoring companies.

---

## References

* Brown, I.D. (1991). *Highway Hypnosis*
* De Waard & Brookhuis (1991). *Driver Status Assessment*
* Pachouly et al. (2020). *Drowsiness Detection Using Visual Behavior*
* George & Routray (2016). *CNN-Based Eye Gaze Classification*
* Ministry of Road Transport and Highways, India

---

