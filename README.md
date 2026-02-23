# Metal-rods-production-analysis-SQL-project
This project demonstrates the application of Statistical Process Control (SPC) techniques on a manufacturing process producing metal rods.
The goal is to monitor process stability, variation, and defect behavior using industry-standard control charts and present insights through an interactive Power BI dashboard.
The project simulates a real-world quality control scenario commonly used in manufacturing industries.

Objectives :

Analyze process stability over time

Identify special causes of variation

Monitor defect rate and defect counts

Translate statistical results into business-friendly insights

Build a human-readable quality dashboard

Tools & Technologies :

Power BI – Dashboard creation & DAX calculations

SQL Server (SSMS) – Data storage & querying

CSV Dataset – Simulated manufacturing inspection data

SPC Methodology – X̄, R, P, and NP control charts

Control Charts Used & Interpretation :
 X̄ (X-Bar) Chart – Average Rod Diameter Over Time
Purpose:
Monitors whether the average rod diameter remains stable across batches.

R Chart – Variation Within Each Batch
Purpose:
Tracks variation within each batch to ensure consistency.

P Chart – Defect Percentage per Batch
Purpose:
Monitors the percentage of defective rods per batch.

NP Chart – Total Defects per Batch
Purpose:
Tracks the count of defective rods per batch.

Insights:
R CHART – 
The process variation within batches is mostly under statistical control, with a few batches showing unusually high internal variation.


X̄ CHART –
The average diameter is generally stable; however, one batch shows a clear out-of-control signal, indicating a special cause such as incorrect machine setting, calibration
error, or operator mistake.


P CHART –
The defect proportion shows high batch-to-batch variability, with multiple batches exceeding the upper control limit. This indicates the defect generation process is not statistically stable and may be influenced by intermittent assignable causes.
Since X̄ and R charts are mostly stable, defects are not strongly driven by diameter variation alone, suggesting other quality factors (surface finish, cracks, handling damage).


NP CHART – 
The number of defectives per batch frequently exceeds the expected limit, confirming instability observed in the P chart. This reinforces the presence of sporadic quality failures rather than random variation.


MATHEMATICAL Formulas used in charts :

R Chart  :    

R = Xmax - Xmin
UCL(upper control limit) = D4​×Rˉ
LCL(lower control limit) = D3​×Rˉ


X̄ Chart :

Xˉ= ∑X/n​
UCL=Xˉ+A2×Rˉ
LCL=Xˉ−A2×Rˉ


p chart :

p   = Sample Size / Number of Defective Items
pˉ  = Total Units / Total Defects
UCL = p̄ + 3 * √( (p̄ * (1 - p̄)) / n )
LCL = p̄ - 3 * √( (p̄ * (1 - p̄)) / n )

np chart :

np  = n*pˉ
UCL = np + 3​√npˉ(1 - p̄)
LCL = np - 3​√npˉ(1 - p̄)
        ​


	​

	​
​


	​























