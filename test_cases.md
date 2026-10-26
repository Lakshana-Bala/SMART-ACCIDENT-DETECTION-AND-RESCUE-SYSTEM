# Test cases

Run these checks in a modern browser and record actual results before reporting them as passed.

| ID | Action | Expected result |
|---|---|---|
| TC01 | Open `index.html` | Dashboard loads in the browser without installing Python |
| TC02 | Select a JPG or PNG file | Image preview appears; no AI analysis is claimed |
| TC03 | Select “Possible accident detected” and run | Simulated alert appears and a row is added to the table |
| TC04 | Select “No accident detected” and run | A no-alert message appears and no new record is added |
| TC05 | Enter latitude 100 and run | Input is rejected as invalid |
| TC06 | Click the OpenStreetMap link | Browser opens a map location (internet required) |
| TC07 | Download CSV | CSV file downloads containing the alert records |
| TC08 | Clear demo records | Table returns to the empty state |
