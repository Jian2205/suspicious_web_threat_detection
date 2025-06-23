# Cybersecurity Project: Suspicious Web Threat Interactions

## Objective
To detect and analyze suspicious web traffic using unsupervised machine learning (Isolation Forest) based on AWS CloudWatch logs from a production web server.

## Dataset
- Web traffic logs including features like:
  - Bytes In/Out
  - Protocol
  - Source IP & Country
  - Ports, Timestamps

## Tools & Libraries
- Python (Pandas, NumPy, Seaborn, Matplotlib)
- Scikit-learn (`IsolationForest`)
- Jupyter Notebook

## Key Features Engineered
- `session_duration`: Time difference between start and end of session
- `avg_packet_size`: Total bytes transferred per second
## ML Approach
- **Unsupervised Anomaly Detection** using Isolation Forest
- `contamination=0.05` to identify top 5% outlier sessions

## Visualization & Insights
- EDA on protocols, response codes, IP origins
- Scatter plots highlighting anomalous sessions

## Result
- Detected several anomalous sessions aligned with known suspicious flags
- Exported results for further threat investigation

## Files
- `notebook.ipynb` — main analysis
- `suspicious_sessions.csv` — anomaly output
- `report.pdf` — summary of findings
- `presentation.pptx` — project slide deck

## Conclusion
This project shows that unsupervised ML can be a practical, lightweight solution for anomaly-based intrusion detection without relying on labeled data.
