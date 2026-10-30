# Predicting soil degradation with machine learning

**Concept proposal** for a machine learning model that estimates the risk of soil degradation, so that governments and organizations can act before fertility and biodiversity are lost. This is a project design, not an implemented model.

Project completed during the *Data Science, Analytics and AI Agents* program at [start2impact](https://www.start2impact.it/). The full presentation is in Italian.

## The problem

According to the UN SOFI report, about 1.7 billion people live in areas where crop yields are 10% lower because of human-induced soil degradation. Reversing just 10% of that degradation on existing farmland could lift around 154 million people out of undernourishment every year. The project relates to **UN Sustainable Development Goal 2, Zero Hunger** (target 2.4).

## Proposed approach

- **Data:** soil degradation indicators from ISPRA (the Italian Institute for Environmental Protection and Research): land cover change, productivity loss, organic carbon loss, habitat quality loss, soil erosion, artificial land cover and burned areas.
- **Training and validation:** train on Italian data, then validate on international data.
- **Output:** a continuous risk index from 0 to 100, where values above 50 indicate high risk of degradation, shown on a color-graded map for non-technical users. The model does not measure species directly, but the environmental impacts that reduce biodiversity and fertility.

## How success would be measured

- **MAE (mean absolute error)** between predicted and observed degradation, with a target of 8%. The literature commonly reports errors between 10% and 15%, so 8% is ambitious but realistic with good-quality data. The model would be trained on data up to 2018 and tested on later periods, to check that it really anticipates future degradation without using information that would not be available at prediction time. MAE was chosen because it reads directly as "off by X percentage points".
- **Estimated ROI** over 5 years: estimated net economic benefits divided by the costs of the project and of soil restoration. A ROI above 1 indicates economic sustainability.

## Expected benefits (estimates)

- Acting early on just 20% of at-risk areas, with an average 5% yield recovery, would raise overall productivity by about 1% at territorial level.
- With an average gross saleable production of €3,800 per hectare, a 5% yield increase is worth about €190 per hectare per year, around **€1.9 million on 10,000 hectares**.
- A 30% reduction in chemical inputs (estimated at €200 per hectare) would save about **€600,000 on 10,000 hectares**.

## Who would use it

National and regional governments, international organizations such as FAO and UN, research institutes and environmental NGOs, to identify high-risk areas, prioritize interventions and allocate resources more efficiently.

## Repository contents

```
.
├── README.md
└── predicting-soil-degradation-with-machine-learning.pdf    # full proposal (in Italian)
```

## Author

**Danilo Manzo**, junior Data Analyst (Excel, SQL, Python)<br>
[Portfolio](https://danilomanzo.eu) · [LinkedIn](https://www.linkedin.com/in/danilomanzo) · [Email](mailto:manzodanilo1@gmail.com)
