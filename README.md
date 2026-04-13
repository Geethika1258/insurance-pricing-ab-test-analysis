# insurance-pricing-ab-test-analysis
A/B testing analysis of flat-rate vs risk-based insurance pricing strategies using Python and Power BI

## Business Problem
An insurance company is testin two premium pricing strategies.
Which strategy retains more customers and generates higher revenue?

- **Strategy A** - Traditional flat-rate pricing
- **Strategy B** - Risk-based dynamic pricing

## Data Set
- 5,000 simulated policyholders
- 14 features-age,occupation,region,policy type,premium,lapse status
- Simulated using acturial assumptions based on real industry lapse patterns

 ## Approach
 1. Datasete simulation using Python (Numpy,Pandas)
 2. A/B test statistical analysis - two-sample t-test
 3. Customer segmentation by age group,region,policy type
 4. Interactive Power BI dashboard with slicers and KPIs

## Key Findings
1. Strategy B reduces lapses rate by **3.9 percentage points** (28.4% --> 24.6% )
2. Strategy B generates **₹1.93M more revenue** than Strategy A
3. Biggest retention improvement in **41-50 age segment** (27.5% --> 21.0%)
4. Both findings are statistically significant (p = 0.0019)

## Statistical Test Results
| Test | H0 | Result | P-Value |
|------|----|--------|---------|
| Two-sample t-test | Same lapse rste | Reject H0 | 0.0019 |
| Two-sample t -test | Same revenue | Reject H0 | 0.0000 |

## Model Performance
| Metric | Strategy A | Strategy B |
|--------|------------|------------|
| Customers | 2,440 | 2,560 |
| Lapse Rate | 28.4% | 24.6% |
| Avg Premium | ₹3,015 | ₹3,629 |
| Total Revenue | ₹7.36M | ₹9.29M |

## Business Recommendation 
Risk-based dynamic pricing (Strategy B) should be rolled out 
prioritising the 41-50 age segment where retention improvement is highest. Full rollout projected to generate ₹1.93M additional annual revenue across 5,000 policyholders.

## Dashboard 
https://github.com/Geethika1258/insurance-pricing-ab-test-analysis/blob/main/Insurance%20Pricing%20AB%20test%20Dashboard.pdf

## Tools
Pyhton | Pandas | Numpy | Scipy | Matplotlib | seaborn | Power BI 

## Files 
- `ab_test_insurance.csv` - simulateed dataset
- `ab_test_powerbi.csv` - enriched dataset for dashboard
- Jupyter notebook - full analysis with hypothesis tests
- Power BI dashboard Screenshot

## Related Projects 
- [Motor Insurance Claims Analysis] (https://github.com/Geethika1258/motor-insurance-claims-analysis/tree/main)
