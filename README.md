# Cross-Site WebSocket Hijacking (CSWH) Tester

This is a simple web page to test for Cross-Site WebSocket Hijacking (CSWH) vulnerabilities.

## What is CSWH?

Cross-Site WebSocket Hijacking is a vulnerability where a malicious website can open a WebSocket connection to a vulnerable server application. If the WebSocket handshake relies solely on HTTP cookies for session handling and doesn't have other forms of protection (like tokens), the browser will automatically send the cookies, potentially allowing the malicious site to impersonate the user.

## How to Use

1.  Open the `CSWH-test.html` file in your web browser.
2.  Enter the WebSocket URL of the application you want to test in the "WebSocket URL" input field (e.g., `wss://yourapp.com/socket`).
3.  Click the "Connect" button.
4.  Observe the log output.
    *   A **"SUCCESS: Connection established!"** message indicates that your application might be vulnerable to CSWH.
    *   An **"ERROR"** message suggests the connection failed, which could be for various reasons (CORS, network issues, etc.), but it doesn't necessarily mean you are safe.
5.  If the connection is successful, you can use the "Send Data" section to send messages to the WebSocket server to further test the vulnerability.

## Disclaimer

This tool is for educational and testing purposes only. Do not use it on systems you do not have permission to test.