# Heartbeat Abnormality Classification Challenge

## Company Introduction
Welcome to the Heartbeat Abnormality Classification Challenge! This competition, organized by Ostrich AI in collaboration with a leading healthcare technology company, aims to advance the detection and classification of heartbeat abnormalities using real patient data. Join us in this mission to improve cardiac healthcare by developing state-of-the-art machine learning models.

## Problem Statement
Cardiovascular diseases are a leading cause of mortality worldwide. Early detection of heartbeat abnormalities can significantly improve patient outcomes. In this competition, your task is to classify between noise and 24 types of heartbeat abnormalities from 10-second ECG data vectors.

Your objective is to build a machine learning model that can accurately classify the following heartbeat abnormalities:

||||
|--------|---------|---------|
| 1. VPB | 2. Afib | 3. PSVT |
| 4. PVC | 5. SVPB | 6. VT   |
| 7. Arrhythmia | 8. PAC | 9. Atrial Pair |
| 10. Atrial Run | 11. Sinus Pause | 12. Second Degree AV Block Type I |
| 13. Second Degree AV Block Type II | 14. Atrial Triplet | 15. First Degree AV Block |
| 16. VT Couplet | 17. VE Triplet | 18. AF |
| 19. VE Couplet | 20. Bigeminy | 21. Trigeminy |
| 22. Paced Rhythm | 23. Triplet | 24. Others |

## Dataset Description
The dataset provided for this competition contains ECG signal data along with corresponding metadata. Each row in the dataset represents an ECG recording for a particular patient and includes the following columns:
- **HR**: Heart Rate
- **ECG VALUE**: A comma-separated list of ECG signal values
- **Created**: The timestamp when the ECG data was recorded
- **StartTime**: The start time of the ECG recording
- **EndTime**: The end time of the ECG recording
- **DoctorId**: The ID of the doctor who recorded the ECG
- **PatientId**: The ID of the patient
- **AbSubType**: The type of abnormality detected in the ECG (e.g., Vpb, N, etc.)

Below is a sample of the dataset:

| HR | ECG VALUE | Created | StartTime | EndTime | DoctorId | PatientId | AbSubType |
|----|-----------|---------|-----------|---------|----------|-----------|-----------|
| 84 | 471,472,473,...,506 | 00:27.0 | 00:17.0 | 00:27.0 | 7 | 193 | Vpb |
| ... | ... | ... | ... | ... | ... | ... | ... |

## Data Files
- **train.csv**: Training data with 10-second ECG vectors and corresponding labels.
- **test.csv**: Testing data with 10-second ECG vectors for which you need to predict the labels.
- **sample_submission.csv**: A sample submission file in the correct format.

## Evaluation
Submissions are evaluated based on the F1 score. The F1 score is the harmonic mean of precision and recall, providing a balance between the two metrics. This is crucial for this task as both false positives and false negatives can have significant impacts on patient outcomes.

## Submission
Your submission file should be a CSV with the following columns:
- **id**: The unique identifier for each sample.
- **label**: The predicted type of heartbeat abnormality.

**Example:**

| id | label |
|----|-------|
| 1 | Afib |
| 2 | Bigeminy |
| ... | ... |

## Getting Started
To help you get started, we've provided a [baseline notebook](https://github.com/Mihir-Ai-lab/Heartbeat-Classification/blob/main/baseline.ipynb) that demonstrates how to load the data, preprocess it, and build a simple model using a convolutional neural network (CNN). Feel free to build on this or use your own approach.

## Prizes
- **1st Place**: ₹35,000
- **2nd Place**: ₹20,000
- **3rd Place**: ₹15,000

## Timeline (Tentative)
- **Competition Launch**: July 20th
- **Data Exploration and Preprocessing**: July 20th - July 23rd
- **Model Development**: July 23rd - July 30th
- **Final Submission**: August 4th
- **Result Announcement**: August 6th

## Support

If you have any questions or need assistance, please post in the competition forum or contact our support team at support@ostrich-ai.com.

Further details regaridng the exact competition dates & how to participate will be shared on the [community](https://nas.io/ostrich-ai)

We look forward to your innovative solutions and wish you the best of luck!
