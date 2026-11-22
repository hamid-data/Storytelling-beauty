# Does the Story Change the Brand? Storytelling in Beauty Advertising

Beauty brands tell very different stories. Nivea talks about what its products *do*. The Body Shop talks about what it *stands for*. This project looks at whether that difference actually changes how young adults in Germany see the brand, and what really drives their feelings and intention to buy.

It's a small online experiment, analysed in SPSS, and written up as a short research report.

## The question

1. Do people respond differently to **product-driven** storytelling (Nivea) than to **purpose-driven** storytelling (The Body Shop)?
2. Which parts of brand perception are affected: performance, imagery, judgments, authenticity, feelings, or purchase intention?
3. Whatever the story, what best predicts purchase intention, brand feelings and brand resonance?

The brand dimensions come from Keller's Customer-Based Brand Equity (CBBE) model, with authenticity added.

## What I did

- **Design:** a between-subjects experiment. Each person was randomly shown one advertisement, either Nivea (product-driven) or The Body Shop (purpose-driven).
- **Participants:** 178 adults aged 18–35 living in Germany, split evenly (89 per condition) after cleaning.
- **Measures:** brand performance, imagery, judgments, authenticity, feelings, purchase intention, and brand resonance (collected for a smaller group only).
- **Checks:** a manipulation check to confirm people recognised the message they saw.
- **Analysis in SPSS:**
  - frequencies and crosstabs (manipulation check, sample)
  - descriptive statistics
  - independent-samples t-tests with Cohen's d
  - Pearson correlations
  - multiple linear regression (three models)

## What I found

- **The story had a small effect.** Only two of six brand measures differed between the two ads.
  - **Brand imagery** was higher after the purpose-driven Body Shop ad (M = 68.6 vs. 63.1, p = .033, d = −0.32).
  - **Purchase intention** was higher after the product-driven Nivea ad (M = 67.1 vs. 58.5, p = .027, d = 0.34).
  - Performance, judgments, authenticity and feelings did not differ between groups.
- **Everything moves together.** The brand measures correlated strongly with each other (r = .51 to .74).
- **Feelings drive buying intention.** Brand feelings were the only significant predictor of purchase intention (β = .63, R² = .64).
- **Performance drives resonance.** Brand performance was by far the strongest predictor of resonance (R² = .76).
- **Authenticity drives feelings.** Authenticity, judgments and performance together explained 62% of the variation in brand feelings, with authenticity the strongest predictor (β = .45).

In short: how the story is told mattered less than whether the brand feels authentic, performs well and creates an emotional connection.

## Repository contents

```
├── README.md
├── report/
│   └── Storytelling_Beauty_Brands_Report.docx   # full write-up (introduction to conclusion)
└── results/
    └── SPSS_Results_Summary.pdf                 # the final tables from SPSS, nothing else
```

The results PDF contains only the tables behind the report: manipulation check, sample, descriptives, t-tests, correlations and the three regression models.

## Data

The survey responses are **not included**. They come from human participants, so I haven't shared them publicly. Everything in the report can be traced to the tables in the results PDF.

## How to reproduce the analysis

If you have a similar dataset in SPSS Statistics:

1. Create a condition variable (1 = Nivea, 2 = The Body Shop) and a manipulation-check variable.
2. Keep only valid, complete cases (here, German respondents aged 18–35 who passed the eligibility checks).
3. Run **Frequencies** and **Crosstabs** for the manipulation check and sample description.
4. Run **Descriptives** for the brand scores.
5. Run **Independent-Samples T Test**, grouped by condition, with effect sizes switched on.
6. Run **Correlate → Bivariate** across the brand measures and shopping-value items.
7. Run **Regression → Linear** (Enter method) for purchase intention, brand resonance and brand feelings.

## Things to keep in mind

- **One ad per brand.** Differences may reflect these two particular advertisements, not product-driven or purpose-driven storytelling in general.
- **Small, single-country sample.** Results describe young adults in Germany.
- **Resonance was only measured for part of the sample** (88 people, all in the Body Shop condition). The models that include it use that group only, and resonance cannot be compared between ads.
- **Six t-tests, no correction.** The two significant results are modest and are not adjusted for multiple comparisons.
- **The manipulation check is built into the design.** It asks about the sustainability message, so a perfect split between groups is expected. It shows people noticed the message, not that the story changed their attitudes.
- **The authenticity pathway (H3) was not tested.** The report did not run a formal mediation analysis.

## Tools

IBM SPSS Statistics for the analysis, and Microsoft Word for the report.

## Contact

Research | Statistical Analysis | SPSS | Data Analytics
GitHub: https://github.com/hamid-data
For research, statistical analysis, and collaboration inquiries, feel free to connect through GitHub.
