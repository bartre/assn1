#DFD dictionary

#Entity
Developer - Employee responsible for submitting code to the license scanner process
Manager - Supervisor to Developer; Requests license information from the database

#Process
Scan Forwarding Software - controls the forwarding of submitted software packages and the scan results
Scan for Licenses - Program responsible for accepting submitted software packages and extracting license information
Request for Software Project License and Vulnerability Information - takes a request from the manager, pulls all stored license and vulnerability information, and sends it to the manager
Policy Document Forwarding Software - takes a request from either the manager or the developer, pulls all stored policy documentation information, and sends it to the requesting entity.
Policy Document Submission Service - Allows the manager to submit either an entirely new or an updated policy document. forwards the new file to the Policy documents database

#Database
Software license and vulnerability database - stores information received from the Scan Forwarding Software, including license and vulnerability information from submitted software packages
NIST vulnerability database - repository of software names and their possible vulnerabilities, run my the US government
Policy documents database - stores documents detailing corporate policy, only managers can update or submit new files

#Data flows
Software package - the package submitted by the developer for license or vulnerability scanning
Software package name - the name of the submitted software package
License scan results - results returned by the Scan for Licenses process
Vulnerability scan results - results returned by the NIST vulnerability database
License and vulnerability scan results - results returned by the NIST vulnerability database or the Scan for Licenses process
Request for software project license and vulnerability information - request from the developer or manager for a selection of license
and vulnerability information from the Software license and vulnerability database
License and vulnerability information - the selection of license and vulnerability information returned by the Software license and
vulnerability database
New policy document - new document constructed by the manager outlining corporate policy
Updated policy document - new version of an existing document constructed by the manager outlining corporate policy
Request for policy documents - request from the developer or manager for a selection of existing policy documents from the Policy
documents database
Policy documentation - the selection of policy documents returned by the Policy documents database
