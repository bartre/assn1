DFD dictionary

Entity
Developer - Employee responsible for submitting code to the license scanner process
Manager - Supervisor to Developer; Requests license information from the database

Process
Scan Forwarding Software - controls the forwarding of submitted code and the scan results
Scan for Licenses - Program responsible for accepting submitted code and extracting license information
Request for all License and Vulnerability Information - takes a request from the manager, pulls all stored license and vulnerability information, and sends it to the manager
Policy Document Forwarding Software - takes a request from either the manager or the developer, pulls all stored policy documentation information, and sends it to the requesting entity.
Policy Document Submission Service - Allows the manager to submit either an entirely new or an updated policy document. forwards the new file to the Policy documents database

Database
Software license and vulnerability database
NIST vulnerability database
Policy documents database

