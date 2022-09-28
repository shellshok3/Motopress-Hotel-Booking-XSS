# Exploit Title: WordPress Plugin Motopress Hotel Booking Lite 4.4.2 - Stored Cross-Site Scripting (XSS)

Date: 2022-09-28

Exploit Author: Ali Alipour

Vendor Homepage: https://motopress.com/

Software Link: https://wordpress.org/plugins/motopress-hotel-booking-lite/

Version: 4.4.2

Tested on: Windows 10 Pro x64 - XAMPP Server

CVE : N/A

------------------------------------------------

PoC:

1: Install Latest WordPress

2: Install and activate Latest Motopress Hotel Booking Lite (4.4.2).

3: Navigate to Accommodation >> Services.

4: Click on "Add New" button And Enter the JavaScript Payload in the Title Field : ( "><script>alert("XSS")</script> )

5:Click on the publish button.

6. Visit http://localhost/wp/services/

7. XSS payload execute.
