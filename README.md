

 Z_SFLIGHT_EXERCICIO3: Detailed Flight ALV Report
 ✈️ Project Overview

This project is an advanced **ABAP report** that utilizes the **ALV Grid Display** (`REUSE_ALV_GRID_DISPLAY`) to provide a detailed analysis of flights. It combines core flight data (`SFLIGHT`) with route information (`SPFLI`) and performs essential business calculations.

The goal is to offer a professional, interactive tool for querying flights based on comprehensive selection criteria and visualizing key metrics like occupancy and estimated revenue.

## ⚙️ Key Features

* **Data Integration (INNER JOIN):** Joins data from the `SFLIGHT` and `SPFLI` tables to include route details (Country, City, and Airport for Origin/Destination) in the result set.
* **Flexible Selection:** The selection screen is structured into blocks, allowing for mandatory and optional filters:
    * **Airline ID** (Mandatory) and **Flight Date Range**.
    * Optional filters for **Origin Route** (Country, City, Airport).
    * Optional filters for **Destination Route** (Country, City, Airport).
* **Runtime Calculations:** Calculates and displays the following metrics in the report:
    * **Free Seats** (`free_seats`).
    * **Occupancy Rate (%)** (`occup_rate`).
    * **Estimated Revenue** (`estimated_revenue`).
* **ALV Output:** Presents the results in the standard SAP **ALV Grid** format, which offers native SAP features like sorting, filtering, subtotals, and data export.
* **Portuguese UI:** The labels on the selection screen and the ALV column headers are defined in **Portuguese**.

## 🛠️ Technical Details

* **Technology:** ABAP (Advanced Business Application Programming).
* **Tables Used:**
    * `SFLIGHT`: Flight Information.
    * `SPFLI`: Flight Route/Connection.
* **Key Function Module:**
    * `REUSE_ALV_GRID_DISPLAY`: Used for displaying the interactive report.

## 🖥️ How to Use (For ABAP Developers)

1.  Create a new ABAP program (Type 1 - Executable) in the SAP development environment (transaction SE38) named `Z_SFLIGHT_EXERCICIO3`.
2.  Copy and paste the complete source code.
3.  Create the following selection texts (via `GOTO -> Text Elements -> Selection Texts`):
    * `TEXT-001`: Parâmetros Essenciais (Essential Parameters)
    * `TEXT-002`: Filtros de Rota (Origem) (Route Filters - Origin)
    * `TEXT-003`: Filtros de Rota (Destino) (Route Filters - Destination)
4.  Execute the program (F8) and enter the desired selection criteria.
5.  The report will be displayed in the ALV format.

## 📝 Author

Vitor Panciarelli/vitordev25

