# Textpattern-version-4.9.0-Authenticated-Stored-Cross-Site-Scripting
Textpattern version 4.9.0 is vulnerable to a stored cross-site scripting (XSS) attack in the "write Body" parameter. This vulnerability allows attackers to inject and execute malicious scripts in the browsers of unsuspecting users.

Reproduction:<br>
1. Log in as the root user in Textpattern.<br>
2. Navigate to 'Content > Write'.<br>
3. In the body parameter, enter the XSS payload: '<xss onfocus=alert('XSS') autofocus tabindex=1>'. Finally, Click 'Save'.<br>
4. Verify that the script was triggered by visiting 'My Site'.<br>

Authors:<br>
Patrick Dean Ramos<br>
Nathu Nandwani<br>
Junnair Manla<br>
Kevin Rosales<br>
Steve Nyan<br>
Shanavas Shakeer<br>
Lani Lambert<br>
