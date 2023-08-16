# deploy-wwt-demo-app

Repository containing playbooks to deploy, remove, and remediate the WWT Demo Application using Ansible and Event-Driven Ansible.

## wwt-demo-app

The WWT Demo Application can be found at <https://github.com/nsthompson/wwt-demo-app>.

## Playbooks

`deploy_app.yml` - Playbook to deploy demo application container using podman.
`remove_app.yml` - Playbook to remove demo application container.
`restart_app_k8s.yml` - Playbook to remediate application failure when deployed on top of Openshift.

## Rulebooks

`rulebooks/bigpanda_recreate.yml` - Ansible Rulebook to act on Big Panda Incident and remediate using the `restart_app_k8s.yml` playbook via Ansible Automation Controller.

## Contributors

Nick Thompson <<https://github.com/nsthompson>>
