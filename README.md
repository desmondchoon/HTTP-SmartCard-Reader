# MyKAD-Reader
Integrates with SmartCard reader to read MyKAD (Malaysian Identity Card) and allow access of service through port 8080

### How it works?
- Download the whole repo, and unzip it.
- Run reader.exe
- Done

### What is this for?
- Integrating SmartCard readers to read MyKAD and to expose the data through HTTP Requests
- Example: Web Applications that needs to integrate with SmartCard readers

### Is this for a specific reader?
- No. It should work with general smart card readers. Try it to know.

### Technical Details
- Runs on port 8080 (Make sure it is free)
- GET http://127.0.0.1:8080 to get the data from reader (poll it ever 1 second or 0.5 second, up to you)
- Data returned: Array (use JavaScript to parse as JSON if you are using web)
- Currently only reads Name, IC, Address, Postcode, State, City. (Image may come soon)
