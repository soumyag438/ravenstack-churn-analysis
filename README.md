📊 RavenStack SaaS — Churn Analysis (Excel)
> A complete churn analysis project for a fictional B2B SaaS company, built entirely in Microsoft Excel.
> Covers data cleaning, KPI calculation, pivot-style breakdowns, charting, and strategic recommendations.
---
🗂️ Project Overview
RavenStack is a fictional SaaS company. This project analyses why customers are churning and what actions the business should take to improve retention.
The analysis is powered by 5 raw datasets spanning 500 accounts, 5,000 subscriptions, 600 churn events, 2,000 support tickets, and 25,000 feature usage logs.
Metric	Value
Total Accounts	500
Churn Rate	22.0%
Active MRR	$10,159,608
MRR Lost to Churn	$1,179,139
Avg Customer Lifetime	~3 months
Reactivation Opportunities	61 accounts
---
📁 Files in This Repository
```
ravenstack-churn-analysis/
│
├── RavenStack_Churn_Analysis.xlsx     ← Main Excel workbook (10 sheets)
│
├── data/
│   ├── ravenstack_accounts.csv        ← 500 customer accounts
│   ├── ravenstack_subscriptions.csv   ← 5,000 subscription records
│   ├── ravenstack_churn_events.csv    ← 600 churn events with reasons
│   ├── ravenstack_support_tickets.csv ← 2,000 support tickets
│   └── ravenstack_feature_usage.csv   ← 25,000 feature usage logs
│
└── README.md
```
---
📋 Workbook Structure (10 Sheets)
Sheet	Description
💡 Insights & Recommendations	Executive summary, key findings, and a 30/60/90-day action plan
📊 Dashboard	KPI cards, churn-by-plan table, reason breakdown, and 2 charts
📁 Accounts	All 500 accounts — churned rows highlighted in red
💳 Subscriptions	5,000 subscription records with MRR/ARR amounts
🚨 Churn Events	600 churn events with reason codes and refund data
🎫 Support Tickets	2,000 tickets colour-coded by priority
📉 Churn Analysis	Pivot-style breakdowns by plan, industry, country, referral source, reason, and month
💰 MRR Analysis	Active MRR vs MRR lost, customer lifetime by plan, bar chart
🎯 Support Analysis	Ticket metrics compared across active vs churned customers
⚡ Feature Usage	Top 40 features by usage volume and error rate
---
🔍 Key Findings
1. 🔴 Missing Features is the #1 Churn Reason
114 events (19%) of churns are driven by missing features — more than any other reason. This points to a product gap that needs roadmap prioritisation, not a pricing or support fix.
2. 🔴 Post-Upgrade Churn is a Silent Killer
20.5% of churns (123 accounts) happened immediately after an upgrade. These customers raised their expectations by upgrading and then felt let down. An upgrade onboarding sequence would directly address this.
3. 🔴 Churn is Flat Across All Plan Tiers (~22% each)
Basic, Pro, and Enterprise all churn at exactly the same rate. This rules out pricing as a root cause — the problem is the core product value proposition, not the plan structure.
4. 🟠 DevTools is the Highest-Churn Industry Segment
DevTools customers churn at 31% — nearly double the Cybersecurity segment (16%). The product may lack DevTools-specific integrations (e.g. GitHub, CI/CD pipelines).
5. 🟠 Partner Channel Produces 2x Better Retention
Partner-referred customers churn at only 14.6% vs 30.2% for event-sourced leads. Event channel CAC is likely being wasted on poorly-fitted customers.
6. 🟠 Support Resolution Averages 35+ Hours
With 'support' as the joint #2 churn reason, a 35+ hour average resolution time is a direct driver of churn. Tiered SLAs need to be implemented urgently.
7. 🟡 Trial Accounts Churn ~22% More Than Paid
Trial churn is 25.8% vs 21.1% for paid accounts. Trials are failing to convert customers into long-term users. Onboarding improvements should focus on faster time-to-value.
---
🎯 Top Recommendations
Priority	Action	Expected Outcome
🔴 Critical	Implement a mandatory exit survey at cancellation	Eliminate the 15.8% "unknown" churn reason gap
🔴 Critical	Fix the 4 most error-prone features (feature_4, 26, 9, 2)	Reduce product-quality churn
🔴 Critical	Build an upgrade onboarding email sequence	Rescue post-upgrade churns (20.5% of all churn)
🟠 High	Set support SLA targets by priority tier	Address the #2 churn driver
🟠 High	Trigger downgrade early-warning alerts	Intercept the downgrade → churn pipeline
🟠 High	Win-back campaign for 61 flagged accounts	Low-cost MRR recovery
🟡 Medium	Revamp trial onboarding with day-3 and day-10 check-ins	Improve 25.8% trial churn
🟢 Quick Win	Expand the partner referral programme	Scale the lowest-churn acquisition channel
---
🛠️ Tools Used
Microsoft Excel — data cleaning, analysis, charts, and dashboard
Python + pandas — data preparation and workbook generation (openpyxl)
---
📬 About
Built as a portfolio data analysis project demonstrating end-to-end SaaS churn analysis using Excel as the primary analytical and presentation tool.
Feel free to fork, adapt, or use this as a template for your own SaaS analysis projects.
