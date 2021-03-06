Creating a new app
==================

The following steps will guide you through adding a new app to our system that is built by the CI system and deployed to the live environment.

Prerequisites
-------------

To follow this guide you will need:

* A Github account with access to the ONSdigital organisation

* A login for the concourse CI environment

* [dp-cli](https://github.com/ONSdigital/dp-cli)

* Git:

  ```
  brew install git
  ```

* Terraform >= 0.12:

  ```
  brew install terraform
  ```

* Fly CLI (can be downloaded from the links in the corner of the concourse UI)

Getting started
---------------

These steps will create a new app that is built by CI and deployed to the develop and production environments.  If any of the following Github links 404, likely you need to be added to the ONSdigital organisation.

1. Determine what language and technologies you will use

2. Pick a local dev port for your app and add it to the [local ports list](PORTS.md)

3. Use [`dp-cli` to generate the new repo with boilerplate files](https://github.com/ONSdigital/dp-cli/tree/master/project-generation/COMPLETE_PROJECT_SETUP.md)

4. [Add the new app to the environment](https://github.com/ONSdigital/dp-setup#adding-a-new-app)

5. [Add configurations for your new app](https://github.com/ONSdigital/dp-configs#adding-a-new-app)

6. Check the Concourse UI and/or Nomad UI to ensure your new app has successfully deployed to develop
