# Chapter 1: Deeper Concepts

This document provides additional details on core concepts introduced in Chapter 1 to build a strong foundation for your Power BI journey.

## Understanding Power BI & Fabric Licenses

Choosing the right license is one of the most common practical hurdles for new users. The introduction of Microsoft Fabric has expanded the options. This table provides a clear overview to help you navigate them.

| License / SKU         | Type                | Target Audience                                  | Core Functionality & Key Differentiators                                                                                                      |
| --------------------- | ------------------- | ------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------- |
| **Power BI Free** | User-based          | Individual users, learners                       | Create reports for personal use in "My Workspace." **Cannot share or consume content shared by others.** |
| **Power BI Pro** | User-based          | Business users, small & medium teams             | The standard license for collaboration. Allows publishing, sharing, and consuming reports in app workspaces.                                  |
| **Power BI PPU** | User-based          | Power users, analysts in larger organizations    | Provides **all Premium features** (e.g., large data models, paginated reports, deployment pipelines) on a per-user basis.                       |
| **Power BI Premium** | Capacity-based      | Large enterprises, enterprise-wide BI            | Dedicated computing power (P-SKU) for high performance and large user counts. Allows Free users to consume content hosted on this capacity.   |
| **Fabric Capacity** | Capacity-based      | Organizations utilizing the entire Fabric platform | Unified computing power (F-SKU) for **all Fabric workloads** (Power BI, Data Factory, Synapse, etc.). **Important:** Developers still need a **Power BI Pro license** to publish and share Power BI content. |
| **Fabric Trial** | User-based          | Individuals, learners (in Fabric context)        | Allows trying out **all Fabric features**, including Power BI. Content can only be saved within one's personal "OneLake."                     |

**Conclusion:** For collaborating on Power BI reports, the **Pro license** remains the standard for every developer and consumer (who isn't reading from a Premium capacity). Fabric capacities can replace the need for Power BI Premium capacities and extend them with additional data services.

---

## The Three Power BI Storage Modes

In Chapter 1, you load your first data into Power BI. Behind the scenes, Power BI used **Import mode**. This section introduces the three different ways Power BI can access data.

### 1. Import (Default & Most Common Mode)

-   **What happens?** Data is copied from the source, compressed, and stored within the `.pbix` file using the VertiPaq engine.
-   **Pros:** Delivers maximum performance because all calculations run in Power BI's fast in-memory engine. Full DAX and Power Query functionality is available.
-   **Cons:** Data is only as current as the last refresh. The dataset size is limited by available memory.

### 2. DirectQuery

-   **What happens?** Power BI stores only the metadata (table and column names). Every interaction in the report (e.g., clicking a slicer) generates a live query to the source database.
-   **Pros:** Data is always real-time. Ideal for very large data models (big data) that cannot be imported.
-   **Cons:** Performance is entirely dependent on the speed of the source database. Not all DAX and Power Query functions are supported.

### 3. Direct Lake (The New Mode with Microsoft Fabric)

-   **What happens?** A revolutionary hybrid approach. Power BI reads Parquet files directly from Microsoft Fabric OneLake without importing or duplicating data.
-   **Pros:** Combines the performance of Import mode with the real-time capabilities of DirectQuery for data stored in Fabric.
-   **Cons:** Only works for data located in Fabric OneLake.

Understanding these modes will help you design the right architecture for your future projects.
