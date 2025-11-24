Stress Level Prediction System

This project implements a simple, interpretable stress-level prediction model using basic personal lifestyle features. The goal is to demonstrate clean OOP design, lightweight data processing and a small linear prediction formula in Python.

📌 Overview

The system takes the following inputs for each person:

Average Heart Rate (BPM)

Average Daily Sleep Hours

Average Weekly Work Hours

Using these values, it produces:

Stress Score (0–100)

Risk Category: Low, Moderate, or High

The model is intentionally simple and explainable, designed for academic demonstrations and practice.

📁 Project Structure stress_predictor/ │ ├── stress_predictor.py # Main program ├── README.md # Documentation └── sample_data.csv # Example CSV (optional)

🧠 How the Model Works

The model uses a linear formula:

score = 0.8 * (heart_rate / 80)

(-1.5) * sleep_hours
1.0 * (work_hours / 50)
20
Then it clamps the output to a 0–100 range.

Risk Levels Score Range Risk Level 0–40 Low 41–70 Moderate 71–100 High ▶️ Running the Program

Make sure you have Python 3.8+ installed.

Run normally python stress_predictor.py

When running, you can:

Use sample data,

Add people manually,

Or load a CSV file.

The program will display a clean table with predictions.

📥 CSV Format (Optional)

If you want to load people from a CSV file, use this header:

name,heart_rate_bpm,sleep_hours_per_day,work_hours_per_week Alice,75,8,40 Bob,92.5,5.5,65

📤 Exporting Results

After running predictions, you can export the results to CSV:

results.csv

This file will contain:

name

heart_rate_bpm

sleep_hours_per_day

work_hours_per_week

score

risk

📌 Notes

This is not a medical tool.

It is meant only for educational and demonstration purposes.

The weights and baseline values are easy to adjust if you want to experiment.

📜 License

This project can be used for educational and academic purposes. Feel free to modify and extend it as needed.

<img width="849" height="949" alt="Screenshot 2025-11-25 000025" src="https://github.com/user-attachments/assets/86399eef-93e4-4158-a9e3-632e8dca4e84" />
<img width="1014" height="951" alt="Screenshot 2025-11-25 000038" src="https://github.com/user-attachments/assets/ade2997c-1829-4091-9184-4fb8c62dbf91" />
<img width="1229" height="1019" alt="Screenshot 2025-11-25 000050" src="https://github.com/user-attachments/assets/ab2d4cc1-65f0-4cd7-9496-7fc4ee545b8d" />
<img width="1217" height="942" alt="Screenshot 2025-11-25 000059" src="https://github.com/user-attachments/assets/a526a55e-715a-4d02-888c-a345dbb332e5" />
![Uploading Screenshot 2025-11-25 000128.png…]()




