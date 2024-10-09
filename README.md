# Call Center Optimization and Self-Service IVR Project

## Project Introduction
This project centers on enhancing the operational capabilities of United Airlines' call center by analyzing critical performance metrics such as Average Handle Time (AHT) and Average Speed to Answer (AST). The objective is to implement an Interactive Voice Response (IVR) system to handle self-resolvable customer inquiries, thereby improving efficiency, decreasing the agent load, and fostering higher customer satisfaction through strategic automation.

## Challenges Identified
The call center faces a significant influx of calls due to frequent, straightforward customer queries (like booking modifications, upgrades, and seating arrangements). These issues often escalate to agents, which burdens their workload and extends response times. The project intends to:
- Examine call patterns and metrics such as AHT, AST, and customer sentiment to extract insights.
- Propose enhancements to the IVR system to automate responses to common inquiries and minimize agent intervention.
- Assess the potential efficiency improvements that could result from these changes.

## Project Goals
1. Decrease Average Handle Time (AHT) through the automation of calls that can be managed via self-service.
2. Improve the customer experience by providing self-service functionalities within the IVR system.
3. Streamline operational workflows by identifying common call reasons and enhancing agent processes.

---

## Data Utilized
This analysis incorporates various datasets essential for deriving insights:
- **calls.csv**: Details regarding call durations, transcripts, and agent interactions.
- **reason.csv**: Primary reasons associated with each customer call.
- **sentiment_statistics.csv**: Information on customer and agent sentiment, average sentiment scores, and silence durations.
- **customers.csv**: Customer profiles, including loyalty status and unique identifiers.

### Sample Data Fields:
- `call_id`, `customer_id`, `agent_id`, `primary_call_reason`
- `average_sentiment`, `silence_percent_average`, `call_start_datetime`

---

## Methodological Approach

### 1. Data Preparation
   - Combine datasets using `call_id` as the linkage.
   - Clean data to handle missing values, remove duplicates, and ensure consistent formats.

### 2. Exploratory Analysis
   - Trend Analysis: Determine the frequency of various call reasons.
   - Timing Evaluation: Assess the AHT and AST associated with different call types.
   - Sentiment Analysis: Investigate customer-agent interactions to identify emotional patterns.

### 3. Impact of IVR Automation
   - Evaluate the potential decrease in handle time from automating calls that can be resolved without agent assistance (representing 17.82% of total call volume).
   - Analyze call patterns to predict operational gains after implementing automation.

### 4. Visualization Techniques
   - Use bar graphs, heat maps, and scatter plots to depict call frequency, AHT, AST, sentiment distributions, and estimated efficiency improvements from automation.

### 5. Clustering for Customer Insights
   - Implement K-means clustering based on sentiment and silence metrics to discover behavioral trends among customers, guiding the automation strategies.

---

## Visual Representations
- Primary Call Reasons: A bar graph illustrating the most frequent customer inquiries.
- AHT and AST Metrics: Graphical representations showing these metrics by call reason to highlight areas needing improvement.
- Customer Sentiment Clusters: Analysis of sentiment scores and silence percentages, showcasing different customer interaction behaviors.

---

## Tools and Technologies Employed

- Python: For data analysis and processing.
- Pandas: For managing and merging datasets.
- Matplotlib & Seaborn: Libraries for creating visual representations of data.
- Scikit-learn: For implementing clustering algorithms (K-means).
- NumPy: For numerical computations.
- Jupyter Notebook: For interactive analysis structuring.

---

## Insights and Recommendations

- Automating 17.82% of calls related to easily solvable issues (such as booking and seating requests) will alleviate agent workloads and boost customer satisfaction.
- The Average Handle Time (AHT) for issues like IRROPS (Irregular Operations) is significantly higher than for other call categories, indicating areas for potential automation.
- Sentiment analysis reveals that the emotional tone during calls influences both AHT and AST, highlighting the importance of effective agent training in managing customer frustrations.
- Recommended IVR improvements to empower customers to independently resolve common queries, thereby significantly reducing the need for escalations.

---

## Future Steps

- Implement the proposed IVR improvements targeting self-service options.
- Evaluate the financial and operational impacts post-implementation to measure reductions in AHT and AST.
- Expand sentiment analysis to refine training programs for agents aimed at enhancing customer satisfaction.
- Extend the solution across different service channels, including web and mobile, to ensure a seamless customer experience.

---

## How to Execute the Project

1. Clone the repository:
    ```bash
    git clone https://github.com/adi00700/United-CX-CallEfficiency
    ```
2. Install necessary dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Conduct the analysis:
    - Open the Jupyter Notebook `call_center_analysis.ipynb`.
    - Execute the cells sequentially to review the data preparation, analysis, and visualizations.

---

## Contributions
We welcome contributions through:
- Reporting bugs or issues.
- Suggesting new features or enhancements.
- Submitting pull requests for improvements.

---

## License Information
This project is licensed under the MIT License - refer to the LICENSE file for specifics.

---

