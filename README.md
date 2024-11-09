# IS 362 - Project 3: Chinook Database Analysis  

### By: Kathleen Molina  

## Overview  
This project involves analyzing data from the Chinook database using SQL and Python. The goal is to combine data from multiple tables to display customer purchases, including customer names, track names, and album titles. The results are presented in a Pandas DataFrame and saved as a CSV file.

---

## Objective  
1. Combine information from the following Chinook database tables:  
   - `Customer`
   - `Invoice`
   - `InvoiceLine`
   - `Track`
   - `Album`
2. Query and display the following details:
   - Customer's last name and first name.
   - Purchased track names.
   - Corresponding album titles.
3. Sort the data by:
   - Customer's last name, then first name.
4. Save the results to a CSV file (`customer_purchases.csv`).

---

## Project Workflow  

### 1. **Database Connection**  
- Connected to the Chinook SQLite database (`Chinook.sqlite`) using Python's `sqlite3` library.  
- Verified database content by listing all available tables.

### 2. **Data Creation (if needed)**  
- Added tables (`Customer`, `Invoice`, `InvoiceLine`, `Track`, and `Album`) and inserted sample data to ensure the database has sufficient content for analysis.

### 3. **SQL Query**  
- Combined data from multiple tables using SQL `JOIN` operations.  
- Retrieved the following columns:
  - `LastName` (Customer's last name),
  - `FirstName` (Customer's first name),
  - `TrackName` (Name of purchased track),
  - `AlbumTitle` (Title of the corresponding album).  
- Sorted the data by `LastName` and `FirstName`.

### 4. **DataFrame and CSV Export**  
- Loaded the query results into a Pandas DataFrame.  
- Saved the DataFrame to a CSV file (`customer_purchases.csv`) for easy access and submission.

### 5. **Visualization (Optional)**  
- Created a bar chart to display the number of tracks purchased by each customer using `matplotlib`.

---

## Results  

### Example Output (First 5 Rows):  
| LastName | FirstName | TrackName           | AlbumTitle     |  
|----------|-----------|---------------------|----------------|  
| Almeida  | Roberto   | Right Next Door...  | Sex Machine    |  
| Almeida  | Roberto   | In The Evening      | Maquinorama    |  
| Almeida  | Roberto   | In The Evening      | O Samba Pocone |  
| Almeida  | Roberto   | Fool In The Rain    | Maquinorama    |  
| Almeida  | Roberto   | Fool In The Rain    | O Samba Pocone |  

### CSV File:  
The results are saved in the file `customer_purchases.csv`.  

---

## How to Run  

### Prerequisites:  
1. Python 3 installed on your system.  
2. Required Python libraries:  
   - `sqlite3`
   - `pandas`
   - `matplotlib`

3. Chinook SQLite database file (`Chinook.sqlite`) in the working directory.  

### Steps:  
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/<YourGitHubUsername>/IS362-Project3.git
