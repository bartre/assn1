#Executive Summary

####Motivation
For assignment 1, I designed a system to do two key things: work with software package vulnerabilities and licenses, 
and handle corporate policy updates.  The system aims to make developers and managers in the company aware of potential 
vulnerabilities and licenses held in incoming software packages and allow managers to create new policies or update current 
policies to prevent damage to the company.  Open source software can have one or many licenses associated with it, restricting
its use and distribution.  Violating any of these licenses can cause a number of problems, like product recalls and lawsuits.
In addition to the licenses, vulnerabilities can have much the same effect.  If there is a problem with the software,
such as a security hole, this can cause incorrect data, or even leave the company and its customers as potential victims
to hackers.  Managing these risks via corporate policy and software updates are key to maintaining a healthy modern business.

####System Information
The system has two types of users, the manager and the developer, each with unique roles. The developer has three abilities: 
submitting a software package, requesting the stored software package license and vulnerability information, and requesting
the preexisting policy documents.  When the developer submits a new software package, it is sent through the scan forwarding 
software, which sends the package name to the NIST Vulnerability database, and the package itself to the license scanning 
software.  Once both of these processes are complete, the information is returned to the scan forwarding software.  The scan 
forwarding software sends the new information to the software license and vulnerability database and to the developer.  Next,
the developer can request the stored software packages license and vulnerability information.  The end result is the same as 
if the developer submitted a new package, but the information is already on the database, so the request goes to the request
for software license and vulnerability information process, which forwards the request to the database.  Once the database 
has  received the request, the information is sent back to the process, which sends the information back to the developer.
Finally, the developer can request the preexisting policy documents.  This request goes to the policy document forwarding 
software process, which sends the request to the policy documents database.  Once ready, the request is sent to the policy
document forwarding process, and back to the developer.

The Manager has four abilities: requesting the stored software package license and vulnerability informaion, requesting 
preexisting policy documents, submitting new policy documents, and updating existing policy documents.  Requesting the stored 
software package license and vulnerability information and requesting the preexisting policy documents are both identical to 
how they were performed for the developer.  Submitting new policy documents and updating the existing policy documents are
done in an identical way.  The manager submits the file, preexisting or not, to the policy document submission service, which
forwards the file to the policy documents database.
