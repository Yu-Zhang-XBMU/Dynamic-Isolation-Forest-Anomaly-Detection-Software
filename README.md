This application is designed for Dynamic Isolation Forest anomaly detection, accompanying the manuscript submitted to JACC.

Users are advised to download the compressed package, extract its contents, and locate the software named app.exe within the dist folder. Double-click to open the software. Please note that the startup process might be slow, so patience is appreciated.

Software Usage Requirements:

File Format Support:

The software currently supports only .xlsx or .xls format files.
The file must contain at least three columns, named Patient ID, Project, and Hospitalization Days.
Patient ID: Can be anonymized as needed to protect patient privacy.
Project: Refers to the actual laboratory test items.
Hospitalization Days: Represents the sequence of hospitalization days for the patient.
File Format Requirements: The first column must be Patient ID, the second to the penultimate columns should be the actual test items, and the last column must be Hospitalization Days.
Data Consistency:

All patients included in anomaly detection must have the same number of Hospitalization Days (e.g., all patients must have data for 3 or 5 days).
No missing data is allowed. If up to 30% of data is missing for a patient, users should use tools like R or Python to fill the gaps using KNN imputation before proceeding.
Normalization:

After completing the data imputation, normalize all laboratory test columns to eliminate unit discrepancies between test items.
Data Format:

Ensure that all cells contain only numeric values. Do not include reference ranges or other annotations.
Future Updates:

Future versions may include additional features, such as missing data detection, automated KNN imputation, and automated normalization.
Visualization Options:

Future updates may also provide options for result output, such as heatmaps and Nightingale rose charts. Currently, only tabular outputs are supported.
If you encounter any issues during the use of this software, please contact the author via email at 01585@xbmu.edu.cn.
