# Insecure juice shop

# Ojectif
Udajuicer, the largest juice shop in the world was booming until Covid-19 hit. The business team to come up with an online application where customers can place orders for 
delivery/pickup. Someone was able to build them their juice shop application. Unfortunately, the site would constantly go down and they weren’t sure what the issue was. 
To find out why the Juice Shop site keeps going down, SecureCorp, the world well known cybersecurity consulting firm deploys me a security analyst.
As the security analyst, my job will consist of building a threat model for Udajuicer’s website.

# Getting Started
* Download a copy of the juiceshop.ova file from S3. 
* Download & install Oracle VirtualBox software which will be used as our virtualization tool for loading the OVA file downloaded above.
* Download & install a threat modeling tool:
  Example: Microsoft Threat Modeling Tool
* Open up terminal and type the following: bash startup.sh
* Open up a browser in the VM and navigate to localhost:3000

# Section 1: Threat Assessment
## Part 1: Asset Inventory
The first part of our threat model is being able to identify all the assets involved in the target of the assessment. What does Udajuicer have of value? Looking at the architecture 
diagram, identify all the components that make up Udajuicer and document them in the assessment scope of your report. After identifying all the parts, explain the function of each
part and how a request goes from the client to the server. 

## Part 2: Architecture Audit
Now that we’ve identified all the components that makeup Udajuicer, let’s conduct an architecture review with the given diagram. Referencing what we went over secure architecture best 
practices, list out at least 3 flaws. 

## Part 3: Threat Model
Build a Threat Model Diagram showing the flow of data using OWASP Threat Dragon. Identify at least 3 possible threats that would pose a threat to oour web application (Top 10
OWASP).

## Part 4: Threat Analysis
We’ve now identified a few insecurities in Udajuicer’s architecture and want to use this knowledge to help us identify what was causing Udajuicer's website to crash. When in doubt,
investigating logs should point us in the right direction. Analyze the log file on the desktop to identify what type of attack took down the Juice Shop.

## Part 5: Threat Actor Analysis
The final part of our assessment consists of us trying to identify who would possibly want to take down the Juice Shop? 

# Section 2: Vulnerability Analysis
## Task 1: SQL 
The first vulnerability we want to exploit is on the login page of the website

## Task 2: XSS
The second vulnerability we want to exploit is after we’ve logged into the site. We want to exploit an XSS vulnerability in the search bar. Attempt an arbitrary command that will
render an alert with the value “Hacked”. 

# Section 3: Risk Analysis
After notifying Manu of two more vulnerabilities, his technophobia is in full display. You reassure him that these problems can be resolved but the next step is to rank the risks in
order of what should be dealt with first. 
## Task 1: Scoring Risks
Use the matrix in the Threat Model Report to score the risks that we’ve identified so far to the Juice Shop

## Task 2: Risk Rationale

Now that we’ve scored all our risks, explain why you chose to rank the risks in the way you did. This rationale and ranking shows where Udajuicer’s resources should be allocated
first as opposed to trying to tackle everything at once.

# Section 4: Mitigation Plan
## Task 1: Secure Architecture
Use draw.io to design a far more secure architecture for Manu to implement in getting the Juice Shop back up and running,

## Task 2: Mystery Attack Mitigation
Now we want to tackle his most pressing issue and want to implement a solution to mitigate the attack you identified previously.

## Task 3: SQL Injection Mitigation
The next issue we want to fix is the SQL injection vulnerability on his login page.

## Task 4: XSS Mitigation
The last issue we want to fix is the XSS vulnerability.
