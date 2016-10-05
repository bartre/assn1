COMMENT: This is not rendering on the screen well. It is showing as one big sentence. Please format a bit more and I'll provide comments. 


DFD dictionary

Entity
Developer - Employee responsible for submitting code to the license scanner process
Manager - Supervisor to Developer; Requests license information from the database

Process
Scan Forwarding Software - controls the forwarding of submitted software packages and the scan results
Scan for Licenses - Program responsible for accepting submitted software packages and extracting license information
Request for all License and Vulnerability Information - takes a request from the manager, pulls all stored license and vulnerability information, and sends it to the manager
Policy Document Forwarding Software - takes a request from either the manager or the developer, pulls all stored policy documentation information, and sends it to the requesting entity.
Policy Document Submission Service - Allows the manager to submit either an entirely new or an updated policy document. forwards the new file to the Policy documents database

Database
Software license and vulnerability database - stores information received from the Scan Forwarding Software, including license and vulnerability information from submitted software packages
NIST vulnerability database - repository of software names and their possible vulnerabilities, run my the US government
Policy documents database - stores documents detailing corporate policy, only managers can update or submit new files

