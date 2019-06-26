# Azure VDC Documentation

## [Understanding the concepts](understand/readme.md)

These articles will help you understand how the Azure Virtual Datacenter Automation Toolkit works and what it is intended to do.

  - [Prerequisite Azure knowledge](understand/azure.md) - Resources for understanding the Azure services that the toolkit utilizes.
  - [Understanding the Automation Toolkit](understand/toolkit.md) - Explains the important concepts in the toolkit.
  - [Understanding environment types](understand/environment-types.md) - Describes the built-in environment types that the toolkit can deploy.
  - [Common workflow](understand/workflow.md) - Covers the typical usage pattern for the tools in the toolkit.
  - [Roles and permissions](understand/roles.md) - Lists the custom roles that are provided by default in the toolkit.
  - [Modules](understand/modules.adoc) - Explains the modules included in the toolkit.

## [Setting up the toolkit](setup/readme.md)

We recommend using the Docker image provided in this GitHub repository to run the toolkit. However, you can run the toolkit locally if you choose. After getting the toolkit setup, you'll be ready to make your first deployment with the toolkit.

  - [Run the Docker image](setup/setup-docker.md) *(Recommended)* - How to setup the toolkit using Docker.
  - [Run on your local machine](setup/setup-local.md) - How to setup the toolkit natively.

## [Usage patterns for the toolkit](use/readme.md)

This section provides more detail on *deploying* archetypes and modules with the toolkit.

  - [Your first deployment](use/your-first-deployment.md) - Quick start tutorial for deploying the _simulated on-premises archetype_.
  - [General considerations](use/general-considerations.md) - Items to evaluate before deploying any archetype.
  - [Creating archetype configuration files](use/configuration-files.adoc) - How to prepare an `archetype.json` file.
    - [Common parameters](use/common-parameters.adoc) - Parameters used in all archetype configuration files.
    - [Common workload parameters](use/common-workload-config.adoc) - Parameters used by workload archetype configuration files.
  - [Archetype deployment considerations](use/archetype-deployment-considerations.md) - Items to evaluate that are specific to _shared-services_ and _workload_ environments.
  - [Validating deployments](use/deployment-validation.adoc) - How to validate an archetype configuration.

## [Extending the toolkit](extend/readme.md)

The real power of the toolkit is the ability to create new archetypes and modules to meet your specific needs.

  - [Creating new modules](extend/creating-new-modules.adoc) - How to create a new module.
  - [Creating new archetypes](extend/creating-new-archetypes.adoc) - How to create a new archetype.
  - [Using the integration tests](extend/integration-testing.adoc) - How to run and add new integration tests.

## [Script Reference](reference/readme.md)

There are four Python scripts provided by the toolkit.

  - [policy-assignment.py](reference/script-policy-assignment.adoc) Update subscription policy post-deployment
  - [role-creation.py](reference/script-role-creation.adoc) Create subscription roles
  - [subscription.py](reference/script-subscription.adoc) Create management groups and subscriptions
  - [vdc.py](reference/script-vdc.adoc) Deploy archetypes and modules

## [Archetypes](archetypes/readme.md)

Be sure to understand the different [environment types](../understand/environment-types.md) for archetypes.

  - [Simulated on-premises environment](archetypes/on-premises/overview.adoc)
  - [Shared services](archetypes/shared-services/overview.adoc)
  - [IaaS N-tier architecture](archetypes/ntier-iaas/overview.adoc)
  - [App Service Environment + SQL Database](archetypes/paas/overview.adoc)
  - [SAP HANA](archetypes/sap-hana/overview.adoc)
  - [Cloudbreak](archetypes/cloudbreak/overview.adoc)

> NOTE: If you are interested in [contributing](/#contributing), please note that some of the docs are [authored in AsciiDoc](adoc-file-format.adoc) (.adoc) and others are Markdown (.md).