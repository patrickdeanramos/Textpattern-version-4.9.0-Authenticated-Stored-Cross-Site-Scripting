# Textpattern-version-4.9.0-Authenticated-Stored-Cross-Site-Scripting
Textpattern version 4.9.0 is vulnerable to a stored cross-site scripting (XSS) attack in the "write Body" parameter. This vulnerability allows attackers to inject and execute malicious scripts in the browsers of unsuspecting users.

Reproduction:
Log in as the root user in Textpattern.
Navigate to 'Content > Write'.
In the body parameter, enter the XSS payload: '<xss onfocus=alert('XSS') autofocus tabindex=1>'. Finally, Click 'Save'.
Verify that the script was triggered by visiting 'My Site'.

Authors:
Patrick Dean Ramos
Nathu Nandwani
Junnair Manla
Kevin Rosales
Steve Nyan
