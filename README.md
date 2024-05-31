# Red Hat Ansible Automation Hub configuration as code (CaC)

**Red Hat Ansible Automation Hub Configuration Collection**
- [infra.ah_configruation Documentation]( https://console.redhat.com/ansible/automation-hub/repo/validated/infra/ah_configuration/docs/ "infra.ah_configruation Documentation")

**You will need the infrastructure as code to use this experimental feature**
- [Using postinstall feature of containerized Ansible Automation Platform]( https://access.redhat.com/documentation/en-us/red_hat_ansible_automation_platform/2.4/html/containerized_ansible_automation_platform_installation_guide/aap-containerized-installation#using-postinstall_aap-containerized-installation "Using postinstall feature of containerized Ansible Automation Platform")
- [aws_ansible_deployment_containerized gitrepo]( https://github.com/ericcames/aws_ansible_deployment_containerized "aws_ansible_deployment_containerized gitrepo")

**Ansible Automation Platform configuration as code (CaC)**
- [aap.controller.config CaC]( https://github.com/ericcames/aap.controller.config "aap.controller.config CaC")

Example excerpt from inventory file:
===========
```
# AAP Automation Hub - optional
# -----------------------------
# To use the postinstall feature you need to set these variables
hub_postinstall=true
hub_postinstall_dir=/home/ansible-svc/git-repos
# When using config-as-code in a git repository
hub_postinstall_repo_url={{ hub_postinstall_repo_url }}
hub_postinstall_repo_ref=main
```