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

