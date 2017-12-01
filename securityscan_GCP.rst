Security Scanning on Google Cloud Platform App Engine services

Operating System and Application Patches
Google Compute Engine and Google Container Engine are powered by virtual machines (VM). If you use these technologies in your projects, it is your responsibility to keep the VM operating system and applications up to date with the latest security patches. Google maintains security and patching of the host OS environments

Google Cloud Security Scanner  - The Google Security Scanning is a separate service named Cloud Security Scanner.

Automated Vulnerability Scanning
Cloud Security Scanner is a web security scanner for common vulnerabilities in Google App Engine applications. It can automatically scan and detect four common vulnerabilities, including cross-site-scripting (XSS), Flash injection, mixed content (HTTP in HTTPS), and outdated/insecure libraries. It enables early identification and delivers very low false positive rates. You can easily setup, run, schedule, and manage security scans and it is free for Google Cloud Platform users.

Find Common Security Vulnerabilities
Detect key vulnerabilities in development prior to production. After you set up a scan, Cloud Security Scanner automatically crawls your application, following all links within the scope of your starting URLs, and attempts to exercise as many user inputs and event handlers as possible.


Focus on Actionable Results
The findings for XSS, Flash injection, mixed content usage, and outdated/insecure libraries all have very low false positive rates. Results are highlighted to enable you to explore and verify in detail and focus on fixes.

Integrates Easily With Your Processes
You can easily setup and run on-demand immediate or scheduled security scans from the Google Cloud Platform Console. Scans should be run from a test environment and test accounts and are enabled for targets only within your App Engine project to preven

How To Guide for Using Cloud Security Scanner - https://cloud.google.com/security-scanner/using-the-scanner

Pricing, costs and traffic - https://cloud.google.com/security-scanner/pricing
There is no charge for using the scanner. However, using the scanner impacts App Engine instance quota limits, bandwidth (traffic) charges, and quotas for API calls to App Engine services, such as mail, search, etc. The actual amount of traffic generated from a scan depends on the application and the number of URLs, event handlers, forms, and parameters.

The scanner is optimized to keep traffic to a minimum. By default, the scan rate is throttled to approximately 15 queries per second (QPS), with slight variations in the rate due to the asynchronous nature of many web applications. Currently, a large scan stops after 100,000 test requests, not including requests related to site crawling. (Site crawling requests are not capped.)
