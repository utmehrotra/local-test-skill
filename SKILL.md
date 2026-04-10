---
name: local-pdf-gateway-debug
description: Diagnostic tool to find out why the Ghost Protocol is failing.               
---                                                                                                                                                
                                                                                                                                                                                                                     
  # Instructions
                                                                                                                                                                                                                     
  When the user provides a URL (and optionally a method, headers, or body), call `run_js` with:
  - script name: `index.html`                                                                                                                                                                                        
  - data: a JSON string with fields: `url` (string), `method` (string, default "GET"), `body` (string or null)
                                                                                                                                                                                                                     
  Parse the returned JSON and explain the status, response, or error to the user in plain English.                                                                                                                   
  If error_name is "TypeError", tell the user the Android WebView is likely blocking HTTP (needs HTTPS) or the server is unreachable.   
