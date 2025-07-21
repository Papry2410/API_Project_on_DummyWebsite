### **API_Project_on_DummyWebsite**
Tested the APIs of a dummy website, covering POST, GET, PUT, PATCH and DELETE operations.





## **API Testing Project: Reqres Dummy Website**

* **API Operations Covered:** Thoroughly tested `GET`, `POST`, `PUT`, `PATCH`, and `DELETE` requests.
* **Tools Utilized:** Postman for request creation and organization, and Newman for command-line execution.
* **Setup:**
    * Developed a Postman Collection to organize all API requests.
    * Created a Postman Environment to manage the website URL, ensuring easy recall and flexibility.
    * Established a connection between the Collection and Environment for streamlined testing.
* **Validation & Testing Methodology:**
    * Implemented Post-request scripts within Postman to perform data validation after each API call.
    * Intentionally introduced invalid data in some scripts to test error handling and system robustness.
    * Executed all requests for 10 iterations with a 5-millisecond delay between each iteration to simulate load.
* **Reporting:** Utilized Node.js to run Newman and generate detailed test reports.

* Here's how to properly write down those Newman commands, providing context and clarity for each step:

-----

**Newman Installation and Execution Commands**

To get started with Newman for Postman Collection execution and report generation, follow these steps:

**Step 1: Install Newman Globally** 

This command installs the Newman CLI (Command Line Interface) tool on your system, allowing you to run Postman collections from your terminal.

```bash
npm install -g newman
```

**Step 2: Install the HTML Extra Reporter (Optional, but Recommended)**

This command installs a powerful reporter that generates detailed and user-friendly HTML reports of your test runs.

```bash
npm install -g newman-reporter-htmlextra
```

-----

**Executing Postman Collections with Newman**

Once Newman and the HTML Extra Reporter are installed, you can run your Postman Collections using the following commands:

**1. Running for a Single Iteration:** 

```bash
newman run collectionname.json -e environmentname.json -r cli,htmlextra
```

  * Replace `collectionname.json` with the actual name of your Postman Collection JSON file.
  * Replace `environmentname.json` with the actual name of your Postman Environment JSON file.

**2. Running for Multiple Iterations (e.g., 10 Iterations):**

```bash
newman run collectionname.json -e environmentname.json -n 10 -r cli,htmlextra
```

  * The `-n 10` flag specifies that the collection should be run 10 times. You can change `10` to any desired number of iterations.
  * Remember to replace `collectionname.json` and `environmentname.json` with your actual file names.

-----
### *** Newman Report Summary: ***
<img width="1824" height="874" alt="Screenshot 2025-07-22 021144" src="https://github.com/user-attachments/assets/7e31f80c-5b88-49ba-bf19-5859fe72943b" />
<img width="1783" height="873" alt="Screenshot 2025-07-22 021223" src="https://github.com/user-attachments/assets/ace5981a-bd89-4125-a612-fe0c78b67811" />


