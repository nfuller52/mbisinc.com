# McGrew Behavior Services Server Setup
This repository houses the development environment setup as well as the staging
and production server provisioning and deploying.

We use vagrant to provision a virtual machine that very closely represents the production
and staging environments. Development specific WordPress settings, such as `WP_DEBUG` and
`SAVEQUERIES` may be setup and configured in `site\config\environments\development.php`.

Please review the [MBIS Theme]() repository for making theme changes.

## Updating WordPress
Although you can update WordPress via the user interface, in order to keep everyone
on the same page it should be done through this repository.

**DO NOT UPDATE WORDPRESS FROM THE USER INTERFACE**

Instead, simply update the version number in the `site\composer.json` file.

## Development Environment
This site is based on the roots.io development ideology. Information for resources
may be found at [roots.io](https://roots.io/).

Tools utilized:

1. Trellis
2. Bedrock
3. Sage (for the main theme, which is in its own repository)

### Requirements
Please reference the [Trellis](https://roots.io/trellis/docs/installing-trellis/)
documentation for instructions on setting up the virtual machine.

1. ansible ~ 2.7.13
2. vagrant >= 1.9.7
3. virtualbox >= 5.*
4. composer >= 1.5

### Setup

#### Virtual Machine (Web Server, Database and WordPress)
1. Clone this repository
2. Move into the `trellis` directory
3. Start the vagrant box `vagrant up`

* The default IP is set to **192.168.50.50**
* Trellis should automatically update your hosts file to match mbisinc.dev, but,
I suggest you verify it in your local hosts file.

#### Database and Assets
TODO

## Staging Environment
TODO

## Production Environment
TODO

## Development/Git Workflow
TODO

## Deploy Process
TODO
