---
title: Staging activities during a migration
description: Use the Cloud Adoption Framework for Azure to understand staging activities and associated deliverables needed during a migration.
author: martinekuan
ms.author: martinek
ms.date: 04/04/2019
ms.topic: conceptual
ms.service: cloud-adoption-framework
ms.subservice: migrate
ms.custom: internal
---

# Understand staging activities during a migration

As described in the article on promotion models, *staging* is the point at which assets have been migrated to the cloud. However, they're not ready to be promoted to production yet. This is often the last step in the migrate process of a migration. After staging, the workload is managed by an IT operations or cloud operations team to prepare it for production usage.

## Deliverables

Staged assets may not be ready for use in production. There are several production readiness checks that should be finalized before this stage is considered complete. The following is a list of deliverables often associated with completion of asset staging.

- **Automated testing.** Any automated tests available to validate workload performance should be run before concluding the staging process. After the asset leaves staging, synchronization with the original source system is terminated. As such, it is harder to redeploy the replicated assets, after the assets are staged for optimization.
- **Migration documentation.** Most migration tools can produce an automated report of the assets being migrated. Before concluding the staging activity, all migrated assets should be documented for clarity.
- **Configuration documentation.** Any changes made to an asset (during remediation, replication, or staging) should be documented for operational readiness.
- **Backlog documentation.** The migration backlog should be updated to reflect the workload and assets staged.

## Next steps

After staged assets are tested and documented, you can proceed to optimization activities.

> [!div class="nextstepaction"]
> [Optimize migrated workloads](../optimize/index.md)
