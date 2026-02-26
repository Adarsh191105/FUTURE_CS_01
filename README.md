# FUTURE_CS_01
Web Application Security Assessment: KitCoek.<br>
This repository summarizes the findings from the Web Application Security Assessment conducted on the target website, https://kitcoek.in/. The assessment was performed to identify security gaps in HTTP headers, cross-domain configurations, and server responses.<br>

Project Overview:<br>
Target: https://kitcoek.in/<br> 
Date of Assessment: 10 February 2026 <br>
Prepared By: Adarsh Dipak Gurav (Pentester) <br>
Prepared For: Future Interns <br>
Project ID: PEN-2026-001 <br>

Methodology:<br>
The security assessment followed the OWASP Top 10 standard for web application security testing.<br>
Scanning Mode: The assessment utilized automated and passive scanning modes.<br>
Tools Used:<br>
Nmap (Network Mapper) <br>
OWASP ZAP (Zed Attack Proxy)<br>

Key Findings Summary:<br>
The assessment generated 14 alerts and identified four primary security flaws, ranging from High to Informational severity.<br>

IDVulnerability:<br>
 NameSeverityRecommendation1Vulnerable JS Library (Next.js) High Upgrade library to latest version 2Cross-Domain Misconfiguration (CORS) Medium Restrict Access-Control-Allow-Origin 3Missing Security Headers Low Implement X-Content-Type-Options & CSP 4User Controllable HTML Attribute Info Validate/Sanitize input parameters<br>

Conclusion & Recommendations<br>
The most critical discovery is the application's use of an antiquated Next.js library (v12.0.8), which exposes the program to known CVEs and needs immediate patching. Additionally, the application suffers from permissive CORS policies and missing HTTP security headers, which raise the risk of cross-site scripting (XSS) and data theft.<br>
It is highly advised to update the framework to the most recent stable version and enforce more stringent server configurations. Immediate attention to these problems will greatly improve the application's resistance to possible exploitation.<br>

Disclaimer: A penetration test is considered a snapshot in time. The findings and recommendations reflect the information gathered during the assessment (10-02-2026) and not any changes made outside of that period. This document contains proprietary and confidential information<br>

INTERN: ADARSH_GURAV.<br>
DATE: 27-FEB-2026
