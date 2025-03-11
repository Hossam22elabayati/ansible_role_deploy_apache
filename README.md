Ansible Role: Apache Deployment
------------------------------------------
This Ansible role automates the deployment of the Apache web server with customizable configuration files. It includes templates for configuring whitelist IPs, server name, and document rules, as well as a handler to restart Apache whenever the configuration changes.

Table of Contents
----------------------------
- Requirements
- Role Variables
- Dependencies
- Example Playbook
- Handler
- License
- Author Information

Requirements
----------------------------------
Before using this role, ensure you have the following:

Ansible installed on the control machine.

Python installed on the target hosts.

Root or sudo access on the target hosts to install packages and modify configurations.

Role Variables
----------------------------------------------------
This role allows you to customize the following settings:

Apache Server Name: The domain name or IP address for the Apache server.

Document Root: The directory where the website files are stored.

Whitelist IPs: A list of IP addresses allowed to access specific directories.

Document Rules: Configuration for directory indexing, access controls, and overrides.

You can override these variables in your playbook or inventory.

Dependencies
---------------------------------------------------------
This role does not depend on any other roles from Ansible Galaxy. However, it assumes the target hosts are running a supported Linux distribution (e.g., Ubuntu, CentOS).

Example Playbook
To use this role, create an inventory file listing your target hosts and a playbook to apply the role. Pass the necessary variables to customize the Apache configuration.

Run the playbook using the ansible-playbook command, specifying the inventory file and playbook.

Handler
------------------------------------------------------
This role includes a handler to restart Apache whenever the configuration file changes. This ensures that any updates to the configuration take effect immediately.

License
---------------------------------------------------
This project is licensed under the BSD License. See the LICENSE file for details.

Author Information
This role was created by [Hossam Mahmoud].

GitHub: Hossam22elabayati

Email: hossamelabayati@gmail.com
