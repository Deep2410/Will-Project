### 1. Initialization
 - Develop a SubterraneanHazardDetection system.
 - Initialize the database and reports list.
### 2. Start Detection:
  - Display “Detection process started”.
  - Call receive_input.
### 3. Receive Input:
  - Get user Input (Latitude and Longitude).
  - Validate the input (formatting):
    - If input is valid, go to check data existence.
    - If input is invalid, request the correct input and retry.
### 4. Check Data Existence:
  - If the data exists, send the existing result to the frontend.
  - If the data doesn’t exist, Initiate the backend process.
### 5. Initiate Backend Processing:
  - Set up an HTTP client to request external API.
### 6. Query External APIs:
  - Retrieve required geological data (Type of soil, soil bearing capacity, rock type, seismic hazard data, Groundwater table level, slope stability, contamination level, climate data) from external APIs
  - Integrate the data obtained from API with our database.
### 7. Run Analytics:
  - Analyze the combined data to detect hazards:
    - If hazards are detected, generate a report.
      - Create a report with the detected hazards and timestamps.
      - Call send_report.
    - If no hazards are found, notify the user.
### 8. Send Report:
  - Send the Analytics results to the user.
### 9. End Process:
  - Display "Process completed successfully."
