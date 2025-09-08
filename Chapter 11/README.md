# Chapter 11: Advanced Concepts for Sharing and Securing Analytics

After learning the basic mechanics of publishing and sharing your analyses in the book, this document delves into two crucial aspects for professional use in organizations: strategically choosing the right sharing method and securing your data through proper data governance.

---

### Data Governance with Sensitivity Labels

The ease of sharing reports is a strength of Power BI, but it also introduces risks. Not all data is meant for every audience. Therefore, a robust governance strategy is essential. Power BI seamlessly integrates with Microsoft Purview, the central platform for compliance and data security, to address this.

The core of this integration is **Sensitivity Labels**.

**What are Sensitivity Labels?**

These are centrally defined digital tags (e.g., "Public," "Internal," "Highly Confidential") that are applied to Power BI artifacts (reports, datasets, etc.). However, they are more than just labels—they enforce active security policies.

**Key Mechanisms:**

1.  **Centralized Definition:** The labels and their associated rules (e.g., "Block export") are not configured in Power BI but are defined centrally by administrators in the Microsoft Purview compliance portal.
2.  **Application and Inheritance:** As a creator, you apply these labels in Power BI Desktop or the Power BI service. A dataset marked as "Confidential" will automatically pass this label down to all reports built on top of it, ensuring protection is consistent.
3.  **Protection Beyond Power BI:** This is the most critical feature. When a user exports data from a protected report to Excel, the resulting Excel file automatically inherits the same label and its protection policies (e.g., encryption). The data remains secure even after it leaves Power BI.

Using sensitivity labels is the step that transforms an unregulated self-service BI environment into a managed and secure analytics ecosystem that meets corporate compliance requirements.

---

### Strategic Sharing: The Right Method for Every Use Case

Power BI offers several ways to share content. Choosing the right method is critical for a good user experience and clean administration.

| Method | Ideal For... | Key Characteristics |
| :--- | :--- | :--- |
| **Direct Sharing** (Share) | Ad-hoc sharing with individuals or small, defined groups. Quick, informal collaboration. | - **Granular:** You share a single report or dashboard. <br> - **Unstructured:** No bundling of multiple content items. <br> - **Notification:** Recipients get an email with a link. |
| **Workspace** | **Collaboration among developers and analysts.** This is the "engine room" or the "workshop." | - **Collaborative:** All members have editing rights (depending on their role). <br> - **Cluttered for end-users:** Shows all related assets (datasets, dataflows, etc.), which can be confusing for consumers. |
| **Power BI App** | The **formal distribution of finished reports** to a broad audience of end-users. This is the "showroom." | - **Bundled:** Combines multiple reports and dashboards into one professional application. <br> - **Clean Interface:** Consumers only see the reports relevant to them, not the underlying datasets. <br> - **Custom Navigation:** Allows you to create a curated navigation and structure for your content. |

**Conclusion:** Workspaces are for **creation**; Power BI Apps are for **consumption**. Direct sharing should only be used for exceptional cases.
