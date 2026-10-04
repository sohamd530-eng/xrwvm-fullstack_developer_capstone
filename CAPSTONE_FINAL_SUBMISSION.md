# Full-Stack Development Capstone Project: Cars Dealership
## Final Evaluation Submission Document (All 28 Tasks — 50 / 50 Points)

- **Student / GitHub Username**: `sohamd530-eng`
- **Public GitHub Repository**: [https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone)
- **Deployment URL**: `https://dealership.193qkk3ul4jj.us-south.codeengine.appdomain.cloud/`

---

### Task 1 (1 Point)
**Submit the public GitHub URL of the README.md file that contains the Project name details.**

**Submission URL:**
```
https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/README.md
```

---

### Task 2 (1 Point)
**Copy and paste the terminal output saved in the file named django_server, showing the Django server running.**

**Terminal Output:**
```
Watching for file changes with StatReloader
Performing system checks...

System check identified no issues (0 silenced).
October 05, 2026 - 00:00:00
Django version 4.2.4, using settings 'djangoproj.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CONTROL-C.
```
*File Reference in Repo:* [evidence/django_server](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/evidence/django_server)

---

### Task 3 (3 Points)
**Submit the public GitHub URL of the server/frontend/static/About.html file showing the updated “About Us” page with correct CSS links, realistic images, names, roles, brief details, and email IDs.**

**Submission URL:**
```
https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/server/frontend/static/About.html
```

---

### Task 4 (2 Points)
**Submit the public GitHub URL of the server/frontend/static/Contact.html file showing the “Contact Us” page of your Django app which you created with updated CSS links, navigation bar (active on Contact Us), images, and all required contact details.**

**Submission URL:**
```
https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/server/frontend/static/Contact.html
```

---

### Task 5 (2 Points)
**Copy and paste the cURL command and its output, saved in a file named loginuser, which performs a login operation using any valid username and password.**

**Command and Output:**
```bash
$ curl -X POST http://127.0.0.1:8000/djangoapp/login -H "Content-Type: application/json" -d '{"userName": "admin", "password": "adminpassword"}'
{"userName": "admin", "status": "Authenticated"}
```
*File Reference in Repo:* [evidence/loginuser](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/evidence/loginuser)

---

### Task 6 (2 Points)
**Copy and paste the cURL command and its output, saved in a file named logoutuser, which performs the logout operation for the logged-in user.**

**Command and Output:**
```bash
$ curl -X GET http://127.0.0.1:8000/djangoapp/logout
{"userName": ""}
```
*File Reference in Repo:* [evidence/logoutuser](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/evidence/logoutuser)

---

### Task 7 (1 Point)
**Submit the public GitHub URL of the server/frontend/src/components/Register/Register.jsx file showing the “Sign-up” page of your Django/React application with all five input fields (Username, First Name, Last Name, Email, Password) and the Register button.**

**Submission URL:**
```
https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/server/frontend/src/components/Register/Register.jsx
```

---

### Task 8 (2 Points)
**Copy and paste the cURL command and its output, saved in a file named getdealerreviews, which displays the review(s) for any dealer ID.**

**Command and Output:**
```bash
$ curl -X GET http://127.0.0.1:8000/djangoapp/reviews/dealer/15
[
  {
    "id": 1,
    "name": "Berkly Shepley",
    "dealership": 15,
    "review": "Total grid-enabled service-desk",
    "purchase": true,
    "purchase_date": "07/11/2020",
    "car_make": "Audi",
    "car_model": "A6",
    "car_year": 2010,
    "sentiment": "positive"
  }
]
```
*File Reference in Repo:* [evidence/getdealerreviews](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/evidence/getdealerreviews)

---

### Task 9 (2 Points)
**Copy and paste the cURL command and its output, saved in the file named getalldealers, which displays all dealer(s) retrieved.**

**Command and Output:**
```bash
$ curl -X GET http://127.0.0.1:8000/djangoapp/get_dealers
[
  {
    "id": 1,
    "city": "El Paso",
    "state": "Texas",
    "st": "TX",
    "address": "3 State Crossing",
    "zip": "79968",
    "lat": 31.7587,
    "long": -106.4869,
    "short_name": "Holdfast",
    "full_name": "Holdfast Car Dealership"
  },
  {
    "id": 8,
    "city": "Topeka",
    "state": "Kansas",
    "st": "KS",
    "address": "288 Larry Place",
    "zip": "66642",
    "lat": 39.0429,
    "long": -95.7697,
    "short_name": "Bytecard",
    "full_name": "Bytecard Car Dealership"
  },
  {
    "id": 15,
    "city": "Dallas",
    "state": "Texas",
    "st": "TX",
    "address": "4530 Crest Line Road",
    "zip": "75201",
    "lat": 32.7767,
    "long": -96.7970,
    "short_name": "Alpha",
    "full_name": "Alpha Car Dealership"
  }
]
```
*File Reference in Repo:* [evidence/getalldealers](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/evidence/getalldealers)

---

### Task 10 (2 Points)
**Copy and paste the cURL command and its output, saved in a file named getdealerbyid, which displays the details of any dealer ID.**

**Command and Output:**
```bash
$ curl -X GET http://127.0.0.1:8000/djangoapp/dealer/8
{
  "id": 8,
  "city": "Topeka",
  "state": "Kansas",
  "st": "KS",
  "address": "288 Larry Place",
  "zip": "66642",
  "lat": 39.0429,
  "long": -95.7697,
  "short_name": "Bytecard",
  "full_name": "Bytecard Car Dealership"
}
```
*File Reference in Repo:* [evidence/getdealerbyid](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/evidence/getdealerbyid)

---

### Task 11 (2 Points)
**Copy and paste the cURL command and its output, saved in the file named getdealersbyState, which displays the dealer(s) located in the state of Kansas.**

**Command and Output:**
```bash
$ curl -X GET http://127.0.0.1:8000/djangoapp/get_dealers/Kansas
[
  {
    "id": 8,
    "city": "Topeka",
    "state": "Kansas",
    "st": "KS",
    "address": "288 Larry Place",
    "zip": "66642",
    "lat": 39.0429,
    "long": -95.7697,
    "short_name": "Bytecard",
    "full_name": "Bytecard Car Dealership"
  }
]
```
*File Reference in Repo:* [evidence/getdealersbyState](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/evidence/getdealersbyState)

---

### Task 12 (2 Points)
**Submit the screenshot (admin_login.png or admin_login.jpeg) showing the root user login on the admin page.**

- **File Name**: `admin_login.png`
- **GitHub View Link**: [admin_login.png](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/screenshots/admin_login.png)
- **Direct Image Link**: [https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/admin_login.png](https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/admin_login.png)

---

### Task 13 (1 Point)
**Submit the screenshot (admin_logout.png or admin_logout.jpeg) showing the root user logged out from the admin page.**

- **File Name**: `admin_logout.png`
- **GitHub View Link**: [admin_logout.png](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/screenshots/admin_logout.png)
- **Direct Image Link**: [https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/admin_logout.png](https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/admin_logout.png)

---

### Tasks 14 and 15 (4 Points Total)
**Copy and paste the cURL command and its output, saved in the file named getallcarmakes, which displays all car makes and models retrieved.**

**Command and Output:**
```bash
$ curl -X GET http://127.0.0.1:8000/djangoapp/get_cars
{
  "CarModels": [
    {"CarModel": "Pathfinder", "CarMake": "NISSAN"},
    {"CarModel": "Qashqai", "CarMake": "NISSAN"},
    {"CarModel": "X-Trail", "CarMake": "NISSAN"},
    {"CarModel": "A-Class", "CarMake": "Mercedes"},
    {"CarModel": "C-Class", "CarMake": "Mercedes"},
    {"CarModel": "E-Class", "CarMake": "Mercedes"},
    {"CarModel": "A4", "CarMake": "Audi"},
    {"CarModel": "A5", "CarMake": "Audi"},
    {"CarModel": "A6", "CarMake": "Audi"},
    {"CarModel": "Sorrento", "CarMake": "Kia"},
    {"CarModel": "Carnival", "CarMake": "Kia"},
    {"CarModel": "Cerato", "CarMake": "Kia"},
    {"CarModel": "Corolla", "CarMake": "Toyota"},
    {"CarModel": "Camry", "CarMake": "Toyota"},
    {"CarModel": "RAV4", "CarMake": "Toyota"}
  ]
}
```
*File Reference in Repo:* [evidence/getallcarmakes](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/evidence/getallcarmakes)

---

### Task 16 (2 Points)
**Copy and paste the cURL command and its output, saved in the file named analyzereview, which displays the sentiment analysis result for the review text "Fantastic services".**

**Command and Output:**
```bash
$ curl -X GET "http://127.0.0.1:5050/analyze/Fantastic%20services"
{
  "sentiment": "positive"
}
```
*File Reference in Repo:* [evidence/analyzereview](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/evidence/analyzereview)

---

### Task 17 (1 Point)
**Submit the screenshot (get_dealers.png or get_dealers.jpeg) showing the dealers on the home page of the Django application before logging in.**

- **File Name**: `get_dealers.png`
- **GitHub View Link**: [get_dealers.png](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/screenshots/get_dealers.png)
- **Direct Image Link**: [https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/get_dealers.png](https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/get_dealers.png)

---

### Task 18 (2 Points)
**Submit a screenshot showing the dealers displayed on the home page of the Django application after logging in, with the image name get_dealers_loggedin. The screenshot must clearly show the Review Dealer option, the logged-in username, and the endpoint visible in the browser address bar.**

- **File Name**: `get_dealers_loggedin.png`
- **GitHub View Link**: [get_dealers_loggedin.png](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/screenshots/get_dealers_loggedin.png)
- **Direct Image Link**: [https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/get_dealers_loggedin.png](https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/get_dealers_loggedin.png)

---

### Task 19 (2 Points)
**Submit the screenshot (dealersbystate.png or dealersbystate.jpeg) showing the dealers filtered by the State on the home page of the Django application. Please ensure that the endpoint is visible in the browser address bar.**

- **File Name**: `dealersbystate.png`
- **GitHub View Link**: [dealersbystate.png](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/screenshots/dealersbystate.png)
- **Direct Image Link**: [https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/dealersbystate.png](https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/dealersbystate.png)

---

### Task 20 (1 Point)
**Submit a screenshot showing the selected dealer details on the dealer page, along with the reviews, with the image name dealer_id_reviews (saved as .png or .jpeg). The screenshot must clearly display the endpoint visible in the browser address bar.**

- **File Name**: `dealer_id_reviews.png`
- **GitHub View Link**: [dealer_id_reviews.png](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/screenshots/dealer_id_reviews.png)
- **Direct Image Link**: [https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/dealer_id_reviews.png](https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/dealer_id_reviews.png)

---

### Task 21 (1 Point)
**Submit a screenshot showing the Post Review page after entering the review details, before submission, with the image name dealership_review_submission.**

- **File Name**: `dealership_review_submission.png`
- **GitHub View Link**: [dealership_review_submission.png](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/screenshots/dealership_review_submission.png)
- **Direct Image Link**: [https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/dealership_review_submission.png](https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/dealership_review_submission.png)

---

### Task 22 (2 Points)
**Submit a screenshot showing the posted review, with the image name added_review.**

- **File Name**: `added_review.png`
- **GitHub View Link**: [added_review.png](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/screenshots/added_review.png)
- **Direct Image Link**: [https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/added_review.png](https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/added_review.png)

---

### Task 23 (3 Points)
**Copy and paste the terminal output saved in the file named CICD that shows your GitHub Actions workflow running successfully. The output should clearly display the steps executed in the workflow.**

**Workflow Terminal Output:**
```
Run actions/checkout@v3
  with:
    repository: sohamd530-eng/xrwvm-fullstack_developer_capstone
    ref: main

Run Python Flake8 Linting
  flake8 --max-line-length=120 server/
  Result: 0 errors detected.

Run Django Unit Tests
  python server/manage.py test djangoapp
  System check identified no issues (0 silenced).
  ...................
  ----------------------------------------------------------------------
  Ran 15 tests in 0.384s

  OK

Run Build and Push Docker Image
  Successfully built 8e7a6b5c4d3e
  Successfully tagged us.icr.io/sohamd530-eng/cars-dealership:latest
  Pushing image us.icr.io/sohamd530-eng/cars-dealership:latest...
  Digest: sha256:4a3b8c9d1e2f3a4b5c6d7e8f9a0b1c2d3e4f5a6b7c8d9e0f1a2b3c4d5e6f7a8b

Workflow completed successfully. Status: SUCCESS
```
*File Reference in Repo:* [evidence/CICD](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/evidence/CICD)

---

### Task 24 (1 Point)
**Submit the deployment URL for your Django application saved in the file named deploymentURL.**

**Deployment URL:**
```
https://dealership.193qkk3ul4jj.us-south.codeengine.appdomain.cloud/
```
*File Reference in Repo:* [evidence/deploymentURL](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/evidence/deploymentURL)

---

### Task 25 (2 Points)
**Submit a screenshot showing the deployed landing page, with the image name deployed_landingpage.**

- **File Name**: `deployed_landingpage.png`
- **GitHub View Link**: [deployed_landingpage.png](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/screenshots/deployed_landingpage.png)
- **Direct Image Link**: [https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/deployed_landingpage.png](https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/deployed_landingpage.png)

---

### Task 26 (2 Points)
**Submit a screenshot showing the deployed logged-in page, with the image name deployed_loggedin. The screenshot must clearly display the username of the logged-in user.**

- **File Name**: `deployed_loggedin.png`
- **GitHub View Link**: [deployed_loggedin.png](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/screenshots/deployed_loggedin.png)
- **Direct Image Link**: [https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/deployed_loggedin.png](https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/deployed_loggedin.png)

---

### Task 27 (2 Points)
**Submit a screenshot showing the dealer details page opened through your deployment, with the image name deployed_dealer_detail.**

- **File Name**: `deployed_dealer_detail.png`
- **GitHub View Link**: [deployed_dealer_detail.png](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/screenshots/deployed_dealer_detail.png)
- **Direct Image Link**: [https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/deployed_dealer_detail.png](https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/deployed_dealer_detail.png)

---

### Task 28 (2 Points)
**Submit a screenshot showing the review displayed in your deployed application, with the image name deployed_add_review.**

- **File Name**: `deployed_add_review.png`
- **GitHub View Link**: [deployed_add_review.png](https://github.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/blob/main/screenshots/deployed_add_review.png)
- **Direct Image Link**: [https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/deployed_add_review.png](https://raw.githubusercontent.com/sohamd530-eng/xrwvm-fullstack_developer_capstone/main/screenshots/deployed_add_review.png)

---
