# CHANGELOG

## [Commit: [165dee4](https://github.com/byFrederick/ansible-gbh-apps/commit/165dee4356794e73535a226ceeaf8eb3557ccc38)] - 2025-05-27

- Updated app_deployment role to just clone apps repo and install dependencies.
- Added api_deployment role which creates the systemd unit and start the services to run the demo-api app.
- Added webapp_deployment role that builds webapp, installs nginx, and configures nginx to serve the app.

### Sources

- https://dev.to/dpuig/creating-an-ansible-playbook-to-install-and-configure-nginx-for-hosting-static-websites-3n6j

---

## [Commit: [165dee4](https://github.com/byFrederick/ansible-gbh-apps/commit/165dee4356794e73535a226ceeaf8eb3557ccc38)] - 2025-05-27

- Added app_deployment role which clone repos, generate .env, install node dependencies, created a systemd unit and starts the service.

### Sources

- https://docs.ansible.com/ansible/latest/collections/ansible/builtin/git_module.html
- https://stackoverflow.com/questions/4018154/how-do-i-run-a-node-js-app-as-a-background-service
- https://docs.redhat.com/en/documentation/red_hat_enterprise_linux/9/html/using_systemd_unit_files_to_customize_and_optimize_your_system/assembly_working-with-systemd-unit-files_working-with-systemd

---

## [Commit: [24db9be](https://github.com/byFrederick/ansible-gbh-apps/commit/24db9be781baffdb13a6b37d2a5b687625601a30)] - 2025-05-27

- Added common role that installs needed packages, user, group and app directory where the apps will be place.

---

## [Commit: [fa87554](https://github.com/byFrederick/ansible-gbh-apps/commit/fa87554acc13478857c67c039ab9bb02ac31e75d)] - 2025-05-27

- Added config, group_vars, hosts and main playbook files

### Sources

- https://docs.ansible.com/ansible/2.8/user_guide/playbooks_best_practices.html

---

## [Commit: [b297010](https://github.com/byFrederick/ansible-gbh-apps/commit/b2970108450f69763775586c628bf79aebfbf462)] - 2025-05-27

- Initialize folder structure