# Cloud IDE

Deploy your private instance of [Theia](https://theia-ide.org/) in Okteto Cloud

[![Develop on Okteto](https://okteto.com/develop-okteto.svg)](https://cloud.okteto.com/deploy?repo)

This repository launches Theia 1.4.0 configured with Go 1.15. You can deploy it to other frameworks by forking the repo, changing the value of `runtime` in [values-okteto.yaml](values-okteto.yaml) and deploying.

## Identity

During the first deployment, an SSH key will created for your IDE. Use this to be able to clone private repositories, or SSH to other environments. The public key is displayed in the logs, to make it easier to copy/paste. 

## Persistence

Installed plugins, and anything saved under /home/project will be saved to a persistent volume.