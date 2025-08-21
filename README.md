README - FPGA-Based Defibrillator Pulse Simulation Using ECG Signal Detection


📌 Project Overview:
This project focuses on designing and simulating a defibrillator pulse generator on FPGA that can identify abnormal cardiac rhythms (arrhythmias) from real-time ECG signals. It integrates ECG acquisition, digital signal processing, and pulse generation modules entirely on FPGA, ensuring low-latency, real-time detection and simulation of corrective pulses.
Unlike real defibrillators, this project simulates defibrillator pulses for safe educational, research, and prototype development purposes.


🎯 Objectives:
⦁	Detect abnormal cardiac rhythms such as Ventricular Tachycardia (VT) and Ventricular Fibrillation (VF).
⦁	Implement Verilog-based FSM (Finite State Machine) for rhythm analysis.
⦁	Generate simulated defibrillator pulses (biphasic waveform) upon detecting abnormal ECG activity.
⦁	Validate results using ECG datasets and MATLAB-based visualization.


⚡ Why FPGA?:
⦁	Real-time & parallel processing (essential for life-critical ECG detection).
⦁	Low latency compared to microcontrollers/software-based methods.
⦁	Reconfigurability for different ECG conditions and future improvements.
⦁	Low power, portable design suitable for healthcare applications.


🛠️ Methodology:
1.	Load ECG Data – ECG samples (360 Hz) imported from CSV datasets.
2.	Filter Signal – 0.5–40 Hz Butterworth filter applied to remove noise.
3.	R-Peak Detection – Threshold-based peak detection algorithm.
4.	RR Interval Calculation – Time difference between consecutive R-peaks.
5.	Arrhythmia Detection: Short RR (<0.6s) → Tachycardia | Long RR (>1.2s) → Bradycardia.
6.	Defibrillator Pulse Simulation – Abnormal rhythms trigger simulated pulse output & console warnings.
7.	Visualization – ECG plots with R-peak markers and abnormal event highlights.


📂 Repository Contents: 
https://github.com/Pranayreddykankanala/FPGA-based-defibrillators-using-ECG-signal-detection/blob/main/Presentation%2028.pptx ---> Detailed project documentation, literature review, applications, and future scope.
https://github.com/Pranayreddykankanala/FPGA-based-defibrillators-using-ECG-signal-detection/blob/main/PBL%20Review-2%20Documetation%20Format.docx ---> Slide deck summarizing objectives, methodology, and results.


📊 Applications:
⦁	Medical Training & Education – Safe ECG-based defibrillator training without real shocks.
⦁	Smart Ambulances – Embedded detection and alerts for paramedics.
⦁	Remote Patient Monitoring – Real-time ECG detection via telemedicine.
⦁	Wearable Devices – Portable arrhythmia detection in smartwatches/fitness trackers.
⦁	Defibrillator Testing – Simulation-based validation of AED logic.


🔬 Tools & Technologies
⦁	Hardware: FPGA (Verilog/VHDL implementation)
⦁	Software: MATLAB (signal visualization), Xilinx/Intel FPGA toolchain
⦁	Algorithms: R-Peak Detection, FSM for arrhythmia detection, PWM-based waveform generation

👩‍💻 Team Members:
M. Lakshmi Sravya, 
T. Tejaswini Reddy, 
K. Pranay Reddy,
S. Bala Sai Ram.

Guided by: Dr. N. Phalguni Singh & Dr. Vijay Rao Kumbhare


✅ Conclusion:
Real-time ECG monitoring & arrhythmia detection successfully implemented on FPGA. FSM-based detection ensures reliable recognition of abnormal rhythms. A simulated biphasic defibrillator pulse is generated for abnormal ECG patterns. Design is low-power, accurate, and portable, making it suitable for healthcare applications.
📌 This repository is intended for academic and research purposes only. The project simulates defibrillator behavior and does not deliver real medical shocks.
