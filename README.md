# geospatial-panel-modeling
**The Problem:** Urban heat and air pollution are typically tackled as entirely separate issues, but they actually compound one another. The goal of this research was to test the "thermal blanket effect", where daytime smog traps heat and prevents nighttime cooling, and to determine if it disproportionately burdens informal settlements in New Delhi.

**The Methodology:** I constructed a high-resolution spatial dataset tracking three pre-monsoon summers (April to June, 2022–2024). After merging satellite temperature and pollution data with official settlement coordinates, I used a Two-Way Fixed Effects regression to isolate the exact relationship between smog and trapped heat.

**The Impact:** The model revealed a clear disparity: Informal settlements suffer an additional 0.2°C thermal penalty during high-pollution events compared to formally developed areas. These quantitative insights provide a scalable, data-driven framework for targeted infrastructure investments, proving that generalized, city-wide mandates are an inefficient way to solve complex challenges.

## Future Roadmap:
This V1 TWFE regression model proves the historical relationship between pollution and urban heat. To scale this into a production-ready B2B or B2G asset, the following iterations are proposed:

*   **V2 (Real-Time API):** Transition from static CSVs to a live data pipeline integrating real-time MODIS and Sentinel-5P API feeds, allowing dynamic daily heat-penalty scoring.
*   **V3 (Predictive Alerting System):** Implement forecasting models to trigger automated alerts for logistics, real-estate developers, or local infrastructure teams when severe thermal blanket events are imminent.
*   **V4 (Geographic Expansion):** Standardize the data ingestion pipeline to easily deploy the 3.5 km x 5.5 km grid analysis to other major metropolitan areas facing similar industrial and infrastructure challenges.
