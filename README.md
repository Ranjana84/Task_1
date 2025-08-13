# Medical Appointment No Shows – Data Cleaning Task

## Objective
Clean and preprocess the raw dataset to make it ready for analysis.

## Dataset Used
[Medical Appointment No Shows](https://www.kaggle.com/datasets/joniarroba/noshowappointments) – Kaggle

## Steps Taken for Data Cleaning
1. **Load Dataset**  
   - Loaded the dataset using Pandas and inspected the first few rows.

2. **Handle Missing Values**  
   - Checked for null/missing values using `.isnull()`.  
   - Dropped rows with missing data (if any).

3. **Remove Duplicate Rows**  
   - Removed duplicate rows using `.drop_duplicates()` to ensure no repeated records.

4. **Standardize Text Columns**  
   - `Gender` → converted to uppercase (M / F).  
   - `Neighbourhood` → capitalized each word.  
   - `No-show` → converted to uppercase (YES / NO).

5. **Convert Date Columns**  
   - `ScheduledDay` and `AppointmentDay` converted to a consistent format (`dd-mm-yyyy`) using Pandas datetime functions.

6. **Rename Columns**  
   - Renamed columns to lowercase with underscores for consistency.

7. **Fix Data Types**  
   - Numeric columns (`age`, `scholarship`, `hipertension`, `diabetes`, `alcoholism`, `handcap`, `sms_received`) converted to integers.

8. **Save Cleaned Dataset**  
   - Saved as `Medical_Appointment_No_Shows_Cleaned.csv` for further analysis.

## Outcome
- Dataset is clean, structured, and consistent.  
- Ready for data analysis, visualization, or modeling.  
- All numeric and date columns are in correct format.  
- No duplicates or missing values remain.

## Files in this Repository
- `Medical_Appointment_No_Shows.csv` – Original dataset  
- `Medical_Appointment_No_Shows_Cleaned.csv` – Cleaned dataset  
- `data_cleaning_script.py` – Python script used for cleaning  
- `Medical_Appointment_No_Shows_Cleaning_Professional.pdf` – Summary PDF of the cleaning process
