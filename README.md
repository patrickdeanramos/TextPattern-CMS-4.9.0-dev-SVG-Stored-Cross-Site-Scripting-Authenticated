# TextPattern-CMS-4.9.0-dev-SVG-Stored-Cross-Site-Scripting-Authenticated
TextPattern CMS version 4.9.0 is vulnerable to stored cross-site scripting (XSS) during file uploads involving SVG files. The attack is executed by uploading a specially crafted SVG file containing malicious scripts, which are then rendered by the browser.

<B>Vulnerable URL:</B><br>
http://localhost/textpattern/textpattern/index.php?event=file&step=file_insert<br>

<B>Reproduction:</B>
1. Log in as the root user in Textpattern.<br>
2. Navigate to 'Content > File'.<br>
3. Upload the SVG file containing the malicious XSS code.<br>
4. To trigger the XSS, visit https://<url>/textpattern/files/SVG-XSS.svg.<br>
   ![alt text](https://github.com/patrickdeanramos/TextPattern-CMS-4.9.0-dev-SVG-Stored-Cross-Site-Scripting-Authenticated-/blob/main/SVG-XSS.png?raw=True)

<B>Authors:</B>
Patrick Dean Ramos<br>
Nathu Nandwani<br>
Junnair Manla<br>
Kevin Rosales<br>
Steve Nyan<br>
Shanavas Shakeer<br>
Lani Lambert<br>

