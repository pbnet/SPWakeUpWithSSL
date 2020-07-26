# SPWakeUpWithSSL

This is a SharePoint warm-up app for SharePoint 2019.


                SPWakeup2019 for SharePoint 2019 with SSL Support
              
                
The app will open every site on the local server's Sharepoint farm.
You can vary this behaviour by using the run time options listed below.
These options are not case sensitive.

Available run-time options are: 
-Exclude: Excludes the listed Site Collection URL from being woken.
Can be used more than once. Example:
spwakeup2019SSL.exe -Exclude:http(s)://badsite.com -Exclude:http(s)://badsite2.com
-Email: An email address that should be sent a log of the results.
Example: spwakeup6.exe -Email:\"andrei@server.local\"
-UserName: Name of the account that should be used to browse the sites.
If no user name is set, sites are accessed under the current account.
-Domain: The domain of the account specified above.
-Password: The password that should be used to browse the sites.
You only need to set this option if you are also specifying an account.
-Authentication: The type of authentication used to browse the sites.
By default NTLM authentication is used.
-Verbose If this flag is set, every site is listed by URL.
By default only the Total number of sites is listed.
[Warning] If you use the Email option in conjunction with Verbose mode, the
resulting email may be cut-off after 2048 characters.
-Help Shows this help screen.
