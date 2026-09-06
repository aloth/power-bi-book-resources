# Teach Yourself VISUALLY Power BI - Supplementary Material

[![CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](LICENSE)
[![Companion Website](https://img.shields.io/badge/Companion%20Site-alexloth.com-blue)](https://alexloth.com/power-bi-book/)
[![Follow on X](https://img.shields.io/twitter/follow/VisAnalyticsNYC?style=social)](https://x.com/VisAnalyticsNYC)
[![Data Modeling & Star Schema](https://img.shields.io/badge/Data_Modeling_%26_Star_Schema-Chapter_4-F2C811)](Chapter%204)

> Official companion repository for **_Teach Yourself VISUALLY Power BI_** by **Alexander Loth** (Wiley).  
> Use these sample datasets and `.pbix` files to follow along, experiment, and adapt the book’s examples to your own data.

<p align="center">
  <img src="https://alexloth.com/wp-content/uploads/2023/04/Teach-Yourself-VISUALLY-Power-BI-book-cover-1024x944.png" alt="Teach Yourself VISUALLY Power BI book cover" width="420" />
</p>

**Buy the book:** [alexloth.com/power-bi-book](https://alexloth.com/power-bi-book/) · also at [Wiley](https://www.wiley.com/en-us/Teach+Yourself+VISUALLY+Power+BI-p-9781119903772) and [Amazon](https://www.amazon.com/Teach-Yourself-VISUALLY-Power-Tech/dp/1119903777)

---

## Who this is for

* **Visual learners** who prefer step-by-step screenshots over dense prose.
* **Business users & analysts** building their first reports and dashboards in Power BI.
* **Excel users** moving to Power BI and looking for a guided path.
* **Anyone** starting out with Power BI - no DAX, modeling or coding experience required.

---

## Table of Contents
- [Who this is for](#who-this-is-for)
- [What’s Included](#whats-included)
- [Quick Start](#quick-start)
- [Prerequisites](#prerequisites)
- [Repository Structure](#repository-structure)
- [Chapter & File Index](#chapter--file-index)
- [Compatibility Notes](#compatibility-notes)
- [Troubleshooting / FAQ](#troubleshooting--faq)
- [About the Author](#about-the-author)
- [How to Cite](#how-to-cite)
- [Contributing & Issues](#contributing--issues)
- [License](#license)

---

## What’s Included

- **Power BI project files (`.pbix`)** — ready-to-open reports that match specific tasks in the book.
- **Sample datasets (`.xlsx`, `.csv`)** — source files used throughout the chapters to practice end-to-end.

---

## Quick Start

**Option A — Download ZIP (recommended):**
1. Click the green **`<> Code`** button.
2. Choose **Download ZIP**, then unzip locally and open the `.pbix` files in their chapter folders.

**Option B — Git users:**
```bash
git clone https://github.com/aloth/power-bi-book-resources.git
````

---

## Prerequisites

* **Microsoft Power BI Desktop (Windows, free):** [https://powerbi.microsoft.com/desktop/](https://powerbi.microsoft.com/desktop/)
  Installation is covered in Chapter 1 of the book.

---

## Repository Structure

```
power-bi-book-resources/
├─ Data Sets/
│  ├─ Financial Sample.xlsx
│  └─ Retail Analysis Sample.pbix
├─ Chapter 1/
├─ Chapter 2/
├─ Chapter 3/
├─ Chapter 4/
├─ Chapter 5/
├─ Chapter 6/
├─ Chapter 7/
├─ Chapter 8/
├─ Chapter 9/
├─ Chapter 10/
└─ Chapter 11/
```

---

## Chapter & File Index

<details>
<summary><strong>Click to expand the full mapping</strong></summary>

| Chapter | Key Task / Section                               | Corresponding File(s)                                                              |
| :------ | :----------------------------------------------- | :--------------------------------------------------------------------------------- |
| 📂 [Data](./Data%20Sets/) | General data sets used across multiple chapters  | `Data Sets/Financial Sample.xlsx`<br>`Data Sets/Retail Analysis Sample.pbix`      |
| 📖 [1](./Chapter%201/) | *Deeper Concepts: Licenses & Storage* | `Chapter 1/README.md`                                                              |
| 🔌 [2](./Chapter%202/) | *Connecting Power BI to Your Data* | Uses `Financial Sample.xlsx` (no specific start `.pbix`)                           |
| 🧹 [3](./Chapter%203/) | *Remove Duplicate Values* | `Chapter 3 - Remove Duplicates.pbix`                                               |
|         | *Replace Values in a Column* | `Chapter 3 - Replace Values.pbix`                                                  |
|         | *Split a Column Using a Delimiter* | `Chapter 3 - Split Column.pbix`                                                    |
|         | *Group Data* | `Chapter 3 - Group Data.pbix`                                                      |
|         | *Add a Calculated Column* | `Chapter 3 - Calculated Column.pbix`                                               |
|         | *Add an Index Column* | `Chapter 3 - Index Column.pbix`                                                    |
| 🏗️ [4](./Chapter%204/) | *Create Dimension Tables* | `Chapter 4 - Dimension Tables.pbix`                                                |
|         | *Create a Hierarchical Schema* | `Chapter 4 - Hierarchical Schema.pbix`                                             |
| 📊 [5](./Chapter%205/) | *Create a Bar Chart* | `Chapter 5 - Bar Chart.pbix`                                                       |
|         | *Apply Filters to Visuals* | `Chapter 5 - Apply Filters.pbix`                                                   |
|         | *Format the Y-Axis of a Bar Chart* | `Chapter 5 - Format Y-Axis.pbix`                                                   |
|         | *Format the X-Axis of a Bar Chart* | `Chapter 5 - Format X-Axis.pbix`                                                   |
|         | *Add and Format the Data Category* | `Chapter 5 - Data Category.pbix`                                                   |
|         | *Move a Bar Chart's Legend* | `Chapter 5 - Bar Legend.pbix`                                                      |
|         | *Add a Zoom Slider and Update Bar Colors* | `Chapter 5 - Zoom Colors.pbix`                                                     |
|         | *Add Data Labels to a Bar Chart* | `Chapter 5 - Data Labels.pbix`                                                     |
|         | *Add an Image to the Plot Area* | `Chapter 5 - Plot Image.pbix`                                                      |
|         | *Create a Line or Area Chart* | `Chapter 5 - Area Chart.pbix`                                                      |
|         | *Format the Axes of a Line/Area Chart* | `Chapter 5 - Area Axes.pbix`                                                       |
|         | *Add a Legend to a Line/Area Chart* | `Chapter 5 - Area Legend.pbix`                                                     |
|         | *Move Legend and Add Gridlines* | `Chapter 5 - Area Gridlines.pbix`                                                  |
|         | *Add Zoom Slider and Steps* | `Chapter 5 - Area Zoom.pbix`                                                       |
|         | *Add Data Markers and Labels* | `Chapter 5 - Area Markers.pbix`                                                    |
|         | *Format Data Labels of a Line/Area Chart* | `Chapter 5 - Area Labels.pbix`                                                     |
| 📐 [6](./Chapter%206/) | *Create and Format a Gauge Chart* | `Chapter 6 - Gauge.pbix`                                                           |
|         | *Create and Format a KPI Visual* | `Chapter 6 - KPI.pbix`                                                             |
|         | *Create a Matrix Visual* | `Chapter 6 - Matrix.pbix`                                                          |
|         | *Format a Matrix Visual* | `Chapter 6 - Matrix Format.pbix`                                                   |
|         | *Format Values and Column Headers* | `Chapter 6 - Matrix Values.pbix`                                                   |
|         | *Format Row Headers* | `Chapter 6 - Matrix Rows.pbix`                                                     |
|         | *Format Subtotals and Grand Totals* | `Chapter 6 - Matrix Totals.pbix`                                                   |
|         | *Format Specific Column and Cell Elements* | `Chapter 6 - Matrix Elements.pbix`                                                 |
|         | *Create a Waterfall Chart* | `Chapter 6 - Waterfall.pbix`                                                       |
|         | *Format a Waterfall Chart* | `Chapter 6 - Waterfall Format.pbix`                                                |
|         | *Format X-Axis and Legend* | `Chapter 6 - Waterfall Legend.pbix`                                                |
|         | *Add and Format Breakdowns* | `Chapter 6 - Waterfall Breakdown.pbix`                                             |
|         | *Create, Format, and Label a Funnel Chart* | `Chapter 6 - Funnel.pbix`                                                          |
|         | *Create a Pie or Donut Chart* | `Chapter 6 - Pie.pbix`                                                             |
|         | *Format a Pie or Donut Chart* | `Chapter 6 - Pie Format.pbix`                                                      |
|         | *Create a Treemap Chart* | `Chapter 6 - Treemap.pbix`                                                         |
|         | *Format a Treemap Chart* | `Chapter 6 - Treemap Format.pbix`                                                  |
| 🗺️ [7](./Chapter%207/) | *Create a Proportional Symbol Map* | `Chapter 7 - Proportional.pbix`                                                    |
|         | *Create a Choropleth Map* | `Chapter 7 - Choropleth.pbix`                                                      |
|         | *Create an Isarithmic Map* | `Chapter 7 - Isarithmic.pbix`                                                      |
|         | *Create a Skyscraper Map* | `Chapter 7 - Skyscraper.pbix`                                                      |
| 🧮 [8](./Chapter%208/) | *Advanced DAX Concepts Guide* | `Chapter 8/README.md`                                                              |
|         | *SUM* | `Chapter 8 - Add.pbix`                                                             |
|         | *DIVIDE* | `Chapter 8 - Division.pbix`                                                        |
|         | *IF* | `Chapter 8 - Condition.pbix`                                                       |
|         | *COUNT* | `Chapter 8 - Count.pbix`                                                           |
|         | *AVERAGE* | `Chapter 8 - Average.pbix`                                                         |
|         | *CONCATENATE* | `Chapter 8 - Concatenate.pbix`                                                     |
|         | *Apply Conditional Formatting* | `Chapter 8 - Format.pbix`                                                          |
| 🔬 [9](./Chapter%209/) | *Identify Outliers* | `Chapter 9 - Outliers.pbix`                                                        |
|         | *Find Groups by Clustering* | `Chapter 9 - Clustering.pbix`                                                      |
| 📑 [10](./Chapter%2010/) | *Start a Report and Add a Title* | `Chapter 10 - Start Report.pbix`                                                   |
|         | *Add Visuals to a Report* | `Chapter 10 - Report Visuals.pbix`                                                 |
|         | *Add Slicers to a Report* | `Chapter 10 - Slicers.pbix`                                                        |
|         | *Control Visual Interactions* | `Chapter 10 - Interact.pbix`                                                       |
|         | *Enable Drill-Through Actions* | `Chapter 10 - Drill-Through.pbix`                                                  |
|         | *Split a Page into Sections* | `Chapter 10 - Sections.pbix`                                                       |
|         | *Add Bookmarks and Navigation* | `Chapter 10 - Bookmarks.pbix`                                                      |
| 🔒 [11](./Chapter%2011/) | *Advanced Sharing & Security Guide* | `Chapter 11/README.md`                                                             |
|         | *Ask Questions About the Data (Q&A)* | `Chapter 11 - Ask Questions.pbix`                                                  |
|         | *Publish a Report* | `Chapter 11 - Publish.pbix`                                                        |
|         | *Set Up Row-Level Security* | `Chapter 11 - Security.pbix`                                                       |

</details>

---

## Compatibility Notes

* Use the **current monthly version** of Power BI Desktop for best results.
* If a file prompts to **upgrade** when opened, choose **Yes**. After saving, the file may not open in older versions.
* Some visuals (e.g., maps) require setting **Data category** (Country/Region, State/Province, etc.) for fields to geocode correctly.

---

## Troubleshooting / FAQ

* **Numbers import as text or wrong decimal**
  Check **File > Options and settings > Options > Regional Settings**. Ensure the model or your OS locale matches the dataset’s decimal separator.

* **Privacy level prompts / blocked merges**
  Go to **File > Options and settings > Data Source Settings**. Set appropriate **Privacy levels** (e.g., Private/Organizational) to enable transformations.

* **Map visuals not plotting**
  Assign **Data category** to location fields (e.g., Country/Region, City). If needed, provide **Latitude/Longitude** columns.

* **Row-Level Security testing**
  After defining roles, use **Modeling > View as** to validate filters before publishing.

---

## About the Author

**Alexander Loth** is a Data Scientist and Digital Strategist with over 15 years of experience in AI, Data & Cloud.  
His career began at CERN and includes leadership roles at Microsoft, Tableau, and SAP. Today, he advises companies and organizations on their digital transformation journeys and is the author of several bestselling books.

[![Website](https://img.shields.io/badge/Website-alexloth.com-blue?style=flat-square)](https://alexloth.com/)
[![ORCID](https://img.shields.io/badge/ORCID-0009--0003--9327--6865-green?style=flat-square&logo=orcid)](https://orcid.org/0009-0003-9327-6865)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-aloth-blue?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/aloth/)
[![X (Twitter)](https://img.shields.io/badge/Follow-@xlth-black?style=flat-square&logo=x)](https://x.com/xlth)

---

## How to Cite

If you reference the book or materials, please use the following BibTeX entry to cite the book:

```bibtex
@book{loth2023visually,
  title      = {Teach Yourself {VISUALLY} {Power BI}},
  shorttitle = {VISUALLY Power BI},
  author     = {Loth, Alexander},
  year       = {2023},
  publisher  = {Wiley},
  address    = {Hoboken, NJ, USA},
  isbn       = {978-1-119-90377-2},
  url        = {https://alexloth.com/power-bi-book/},
  urldate    = {2026-08-25}
}
```

You can also link the companion site: [https://alexloth.com/power-bi-book/](https://alexloth.com/power-bi-book/).

GitHub also reads `CITATION.cff` in this repository, so the **Cite this repository** button in the sidebar produces the same reference with the author ORCID attached.

---

## Contributing & Issues

This repository serves as a learning resource for the book.

Found a problem or have a question? Use our issue templates:

* 📖 **[Report an Erratum](https://github.com/aloth/power-bi-book-resources/issues/new?template=erratum.yml)** — errors in the book
* ❓ **[Ask a Question](https://github.com/aloth/power-bi-book-resources/issues/new?template=question.yml)** — questions about chapters or examples
* 💻 **[Report a Code Issue](https://github.com/aloth/power-bi-book-resources/issues/new?template=code-issue.yml)** — problems with companion files

---

## 📚 More books by the author

Companion repositories for the other books:

| Book | Publisher |
|:---|:---|
| [Content Creation mit generativer KI](https://github.com/aloth/Generative-KI-Buch-Begleitmaterialien) | mitp 2026 |
| [KI für Content Creation](https://github.com/aloth/KI-Buch-Begleitmaterialien) | mitp 2024 |
| [Microsoft Power BI: Das Praxisbuch](https://github.com/aloth/Power-BI-Fabric-Copilot-Buch-Begleitmaterialien) | mitp 2026 |
| [Datenvisualisierung mit Power BI](https://github.com/aloth/Power-BI-Buch-Begleitmaterialien) | mitp 2022 |
| [Datenvisualisierung mit Tableau](https://github.com/aloth/Tableau-Buch-Begleitmaterialien) | mitp 2021 |
| [Visual Analytics with Tableau](https://github.com/aloth/tableau-book-resources) | Wiley 2019 |
| [Decisively Digital](https://github.com/aloth/decisively-digital-book-resources) | Wiley 2021 |

**Note:** [Microsoft Power BI: Das Praxisbuch](https://github.com/aloth/Power-BI-Fabric-Copilot-Buch-Begleitmaterialien) is the German-language Power BI book.

## License

This work is licensed under a [Creative Commons Attribution 4.0 International License](LICENSE).

[![CC BY 4.0](https://licensebuttons.net/l/by/4.0/88x31.png)](LICENSE).

---

## Acknowledgments

Thanks to **John Wiley & Sons** and to the Power BI community for continued inspiration and contributions.

---

> ⭐ If these resources help you, consider **starring** the repo and following the social links above to get updates and share your work!
> 
