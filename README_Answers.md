# FreshKart Unit 4 — PPT 3 and PPT 4 Answer Pack

This folder contains completed versions of the two supplied activity notebooks and the four supplied CSV datasets.

## Files
- `Unit4_ppt3activity.ipynb` — Can We Trust the AI Analyst? (orders and business insights)
- `Unit4_ppt4activity.ipynb` — Should We Trust the Alarm? (cold-chain anomaly detection)
- `freshkart_orders.csv`
- `freshkart_eta_predictions.csv`
- `freshkart_coldchain.csv`
- `freshkart_paylater.csv`

## How to run
1. Keep the notebooks and CSV files together in this folder.
2. Open the folder in Jupyter Notebook, JupyterLab, or VS Code.
3. Open each notebook and select a Python 3 kernel.
4. Run all cells from top to bottom. The notebooks use relative CSV paths.

## Key verified findings

### PPT 3 — Orders and AI-generated business insights
- The supplied orders file has 13,987 rows and 70 fully duplicated rows; after removing duplicates, 13,917 rows remain.
- Missing ratings are about 27.6% overall, with the highest missingness in Hyderabad (45.0%).
- Mean order value is about ₹464.73, while the median is ₹358; the distribution is strongly right-skewed.
- Bengaluru orders increase overall from January to September, with a fitted slope of about 56.2 orders per month, although the series is not strictly increasing.
- Hyderabad orders decrease about 28.4% from August to September. H2 has missing weekly data; the on-time rate changes by only about −0.3 percentage points.
- Pune's total orders rise about 117% from Q2 to Q3, partly because P3 and P4 are new stores. P1 and P2 show about 7.6% like-for-like growth.
- Partner comparisons are confounded by zone mix. Within both Urban and Suburban zones, Partner A has the higher on-time rate (a Simpson's paradox example).

### PPT 4 — Cold-chain anomaly detection
- There are 8,064 readings, 46 confirmed fault hours (about 0.57%), and 159 ColdSense alerts.
- At the default threshold, precision is about 10.1% and recall about 34.8%; accuracy alone is misleading because faults are rare.
- All 143 false alarms occur at 02:00, during the normal nightly defrost period.
- ColdSense catches all 10 compressor trips, catches 6 of 11 defrost-heater-stuck fault hours, and misses all 25 sensor-frozen fault hours.
- The lowest cost in the tested threshold grid is at 0.30, but changing the threshold does not solve the missed sensor-frozen pattern.
- A flat run of readings on FZ-H2 is a collective anomaly and needs sequence-aware review.

## Submission note
These are completed answer copies of the supplied activity notebooks. Review the written reflection responses and adjust them to accurately represent your own learning and experience before submitting.
