 health-checks
 ================
This Ansible playbook creates a bunch of health checks and generates periodic reports.

It checks the memory, disk, cpu and applications urls on different servers and notify the users with e-mails.

## How does it work?

* The Ansible server acts as a centralized server for all metrices logs, so after applying the healtchecks on each server the Ansible server fetches all these logs
* After that it creates the periodic summary and sends an e-mail with this summary 
* Also it creates a final summary of the day summarizing all the errors occurred


## How to use? 
* Adjust Ansible Hosts file and health check variables according to your need.
* Adjust the smtp and add the e-mails that will receive the summary.

