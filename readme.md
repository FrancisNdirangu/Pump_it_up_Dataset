# Tanzanian Water Pump Functionality Prediction

## Project Overview
This project develops a predictive maintenance solution for Tanzania's water infrastructure by identifying pumps at risk of failure. Using machine learning on pump operation data, we classify waterpoints into three critical states: functional, needs repair, or non-functional - enabling proactive maintenance for sustainable water access.

**Key Results**:
- 76% prediction accuracy with Random Forest model
- 78% recall for identifying non-functional pumps

## Business Understanding
Our solution helps:
- **Water Authorities**: Prioritize repair resources
- **NGOs**: Target preventive interventions
- **Maintenance Teams**: Receive actionable alerts
- **Communities**: Maintain reliable water access

## Data Understanding
We analyzed 59,400 water pumps using 40+ features from:
- Tanzanian Ministry of Water
- Taarifa monitoring platform

Key data dimensions:
- Geographic location (GPS, region, basin)
- Technical specifications (pump type, extraction method)
- Infrastructure details (construction year, water quantity)
- Management factors (funding, community engagement)

## Modeling Approach
Tested three classification models:

| Model | Accuracy | Failure Recall |
|-------|----------|----------------|
| Logistic Regression | 61% | 59% |
| Decision Tree | 71% | 77% |
| **Random Forest** | **78%** | **80%** |

The Random Forest model was selected for deployment due to its superior performance in identifying failing pumps.

## Recommendations and Next Steps
1. Model Deployment 
   - Implement Random Forest as the core prediction engine  
   - Prioritize pumps flagged as "non functional" (80% recall)  
   - Generate weekly repair priority lists for maintenance teams  

2. Resource Optimization
   - Allocate 65% of maintenance budget to high-risk regions:  
   - Pumps > 15 years old
   - Shift from reactive to preventive maintenance schedule  

3. Monitoring & Improvement
   - Integrate with Taarifa's mobile platform for real-time reporting  
   - Retrain model quarterly using new repair data  
   - Track "water access days" per community as success metric
   

## How to Use This Project

### Prerequisites
- Python 3.8+
- Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn

