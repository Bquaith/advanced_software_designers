#### Topic - Application continuity management service

# AppShield

## Summary

An application continuity service dynamically backs up and restores the state of applications running within the framework on K8s. The service shall use the DSL of the framework to determine the relevant application state and its backup policies. Developers of an application should be able to backup and restore a specific version from images and relevant state from the service. The application state shall be stored externally on the given S3-compatible object storage.

### Stakeholder

* DevOps
* System administrators
* Developers
* Information Security
* Product manager

### Functional requirements

* Monitoring the status of applications: Monitors the status of applications and can perform automatic actions

* Restore application status: Ability to select and restore a specific application version and its state.

* Flexible configuration of backup policies: Define a backup policy based on application type, data criticality, and other parameters.

* (?) Supports hot backup: Ability to create backups without stopping the application. Minimize downtime and impact on uptime.

* Management via API and CLI: Full-featured REST API and CLI for integration with other DevOps tools. Ability to create backups and restore via commands in the terminal.

* Control via web interface: Web interface for simplified interaction and status tracking

--------------

* Dynamic creation of backups and restoration of state
  * Service shall be able to backup the state of applications running within the framework on K8s
  * Service shall be able to restore the state of applications backed up by service

* Usage of DSL framework
  * The service shall use the DSL of the framework to determine the relevant application state and its backup policies

* Possibility of creating backups when the developer desires to
  *  Developers of an application should be able to backup
  *  Developers of an application should be able to restore a specific version from images and relevant state

* External storage of state backups
  * The application state shall be stored externally on the given S3-compatible object storage
 
### Constrains

## Team name: ASDs

### Students

* Gorelyi Mikhail
* Lukashin Daniil
* Derezovskiy Ilya
* Sigal Lev 
