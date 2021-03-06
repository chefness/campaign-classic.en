---
solution: Campaign Classic
product: campaign
title: Configure FDA connectors
description: Learn configuration steps for FDA
audience: platform
content-type: reference
topic-tags: connectors
---

# Configuring FDA connectors {#specific-configurations-by-database-type}

Depending on the external databases that you want to be able to access from Adobe Campaign, you will need to carry out certain specific configurations. These configurations essentially involve installing drivers and declaring environment variables that belong to each RDBMS on the Adobe Campaign server.

As a general rule, you need to install the corresponding client layer on the external database on the Adobe Campaign server.

>[!NOTE]
>
>Compatible versions are listed in [Campaign Compatibility Matrix](../../rn/using/compatibility-matrix.md#FederatedDataAccessFDA).
>

## Configuration steps {#fda-configuration-steps}

To set up access to an external database with FDA, configuration steps are:

1. Install the drivers that correspond to your database on the Adobe Campaign server. Drivers are listed in the database-specific pages [listed below](#fda-specific-configuration). 
1. [Create and configure an external account](../../installation/using/connecting-to-database.md) that allows you to establish the connection between Adobe Campaign and the external database. For more information on external accounts in Campaign, refer to [this page](../../installation/using/external-accounts.md).
1. [Create the schema](../../installation/using/creating-data-schema.md) of the external database in Adobe Campaign. This allows you to recognize the data structure of the external database.
1. If needed, [create a new target mapping](../../installation/using/defining-data-mapping.md) from the previously created schema. This is required if the recipients of your deliveries come from the external database. This implementation comes with limitations related to message personalization.

Once the data schema is created, data can be processed in Adobe Campaign workflows. For more on this, refer to [this section](../../workflow/using/accessing-an-external-database--fda-.md).

## Database specific configuration {#fda-specific-configuration}

Depending on the external databases that you want to be able to access from Adobe Campaign, you will need to carry out certain specific configurations. These configurations essentially involve installing drivers and declaring environment variables that belong to each RDBMS on the Adobe Campaign server.

Follow the links below to learn more:

* [Azure Synapse](../../installation/using/configure-fda-synapse.md)

* [Snowflake](../../installation/using/configure-fda-snowflake.md)

* [Hadoop](../../installation/using/configure-fda-hadoop.md)

* [Oracle](../../installation/using/configure-fda-oracle.md)

* [Netezza](../../installation/using/configure-fda-netezza.md)

* [Sybase IQ](../../installation/using/configure-fda-sybase.md)

* [Teradata](../../installation/using/configure-fda-teradata.md)

* [SAP HANA](../../installation/using/configure-fda-sap-hana.md)
