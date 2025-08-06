#Task 2: Analyze a Phishing Email Sample

## Objective

The purpose of this task was to analyze a phishing email sample to identify common indicators of phishing attacks. This exercise helps in understanding how phishing attempts are structured and how to detect them in real‑world scenarios.

## Tools Used

* **Email Sample Source:** phishing.org (phishing examples)
* **Header Analysis Tool:** MXToolbox Email Header Analyzer
* **Operating System:** Kali Linux

## Steps Performed

### Step 1: Collected Sample Email

* Downloaded a phishing email example from **phishing.org**.
* Saved a screenshot of the phishing email for analysis.

**Figure 1: Phishing Email Example**
*(Insert phishing\_example.png here)*

### Step 2: Checked Sender Information

* Observed the sender’s email address: `phishing@fakebank.com`.
* The domain did not match the official domain of the bank, indicating a spoofed sender.

### Step 3: Analyzed Email Header

* Since phishing.org does not provide a raw header, a simulated phishing email header was created.
* The header was analyzed using **MXToolbox Email Header Analyzer**.
* The analysis revealed:

  * **SPF:** Fail
  * **DKIM:** Fail
  * **DMARC:** Fail
  * **Originating IP:** 203.0.113.25 (not authorized for fakebank.com)

**Figure 2: Header Analysis Result**
*(Insert header\_analysis.png here)*

### Step 4: Examined Email Content

* The subject line used urgent language: *“Verify your account immediately to avoid suspension.”*
* Detected a suspicious link:

  * Displayed: `https://secure-bank.com`
  * Actual: `http://malicious-site.com`
* Found grammar issues such as missing punctuation and inconsistent capitalization.

## Results

The email was confirmed to be a phishing attempt based on:

* Spoofed sender domain
* Failed authentication checks (SPF, DKIM, DMARC)
* Mismatched and malicious URL
* Use of urgent and threatening language
* Spelling and grammar errors

## Outcome

By completing this task, I gained:

* The ability to identify phishing indicators in suspicious emails
* Practical experience using header analysis tools like MXToolbox
* A better understanding of common phishing techniques used by attackers

Do you want me to also make a **cover page** for your document (with task title, your name, and date) so it looks more official when you submit?
