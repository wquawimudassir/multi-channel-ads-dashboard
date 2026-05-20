# Multi-Channel Ads Performance Dashboard

## Project Summary

This project is an interactive **multi-channel advertising performance dashboard** built for a analysis. It combines January 2024 paid media data from **Facebook, Google, and TikTok** into a single unified data model and presents the results through a clean, browser-based dashboard.

The main purpose of the dashboard is to make cross-channel performance easier to understand at a glance. Instead of reviewing separate platform exports, the dashboard brings the key metrics together in one place so that marketing, analytics, and business teams can compare spend, traffic, conversions, and efficiency across platforms.

## Business Objective

Paid media data is often fragmented because every ad platform exports data in a different format. Facebook, Google, and TikTok each use different naming conventions and slightly different structures for campaign, ad group, cost, and performance metrics.

The objective of this project was to:

- Standardize the data from all three platforms
- Create one unified dataset for analysis
- Build a dashboard that supports both executive-level and campaign-level review
- Highlight platform performance, spend allocation, conversion volume, and cost efficiency
- Make the dashboard easy to open and review without any backend setup

## Platforms Analyzed

The dashboard includes data from the following advertising platforms:

- Facebook Ads
- Google Ads
- TikTok Ads

The analysis covers the period from **January 1, 2024 to January 30, 2024**.

## Data Model

The source data from each platform had different field names and structures. To make the dashboard work consistently, the data was normalized into one unified table.

### Common Unified Fields

| Field | Description |
|---|---|
| `date` | Reporting date |
| `platform` | Advertising platform name |
| `campaign_id` | Unique campaign identifier |
| `campaign_name` | Campaign name |
| `ad_group_id` | Ad group or ad set identifier |
| `ad_group_name` | Ad group or ad set name |
| `impressions` | Number of times ads were shown |
| `clicks` | Number of ad clicks |
| `spend` | Advertising spend |
| `conversions` | Number of conversions |
| `video_views` | Video views, where available |
| `ctr` | Click-through rate |
| `cpc` | Cost per click |
| `cpm` | Cost per thousand impressions |
| `cpa` | Cost per acquisition |
| `conversion_value` | Conversion value, where available |
| `engagement_rate` | Engagement rate, where available |
| `likes` | TikTok engagement metric |
| `shares` | TikTok engagement metric |
| `comments` | TikTok engagement metric |
| `video_completion_rate` | Video completion rate, where available |

## Metric Definitions

| Metric | Formula | Meaning |
|---|---|---|
| Spend | Sum of media cost | Total amount spent on advertising |
| Impressions | Sum of impressions | Total ad views |
| Clicks | Sum of clicks | Total user clicks |
| Conversions | Sum of conversions | Total conversion actions |
| CTR | Clicks / Impressions | Measures click engagement |
| CPC | Spend / Clicks | Average cost per click |
| CPM | Spend / Impressions × 1,000 | Cost to reach 1,000 impressions |
| CPA | Spend / Conversions | Average cost per conversion |

## Dashboard Features

The dashboard was designed to answer practical marketing performance questions quickly.

### 1. KPI Scorecards

The top section contains five scorecards:

- Total Spend
- Impressions
- Clicks
- Conversions
- Average CPA

These were selected because they answer the most common executive-level questions:

- How much did we spend?
- How many people did we reach?
- How much traffic did we drive?
- How many conversions did we generate?
- How efficient was the spend?

### 2. Platform Filter

The platform filter allows the user to switch between:

- All platforms combined
- Facebook only
- Google only
- TikTok only

When a filter is selected, the KPI cards, charts, and campaign table update dynamically.

### 3. Platform Performance Cards

The platform cards show a side-by-side comparison of Facebook, Google, and TikTok. These cards make it easy to compare spend, impressions, clicks, conversions, CTR, CPA, and CPM by platform.

### 4. Spend Distribution Donut Chart

The donut chart shows how the total budget was distributed across platforms.

This helps answer:

- Which platform received the most budget?
- Is spend concentrated in one channel?
- Does the budget allocation match platform performance?

### 5. Daily Trend Chart

The daily trend chart allows users to switch between:

- Spend
- Clicks
- Impressions
- Conversions

This is useful because total monthly numbers do not show day-by-day movement. Trend analysis helps identify pacing changes, performance spikes, drops, or potential campaign schedule effects.

### 6. Campaign Conversion Chart

The campaign conversion chart ranks campaigns by conversion volume. A horizontal bar chart was used because campaign names are longer and easier to read in this format.

### 7. CPA vs CPM Efficiency Chart

The efficiency chart compares:

- CPA: cost efficiency per conversion
- CPM: cost efficiency per reach/impression volume

This is useful because different campaigns may have different goals. A campaign with a low CPM may be strong for awareness, while a campaign with a low CPA may be stronger for direct response.

### 8. Campaign Performance Table

The campaign table provides a detailed campaign-level breakdown with:

- Platform
- Campaign name
- Spend
- Impressions
- Clicks
- CTR
- Conversions
- CPA
- CPM
- Spend heatmap indicator

The table is useful for deeper analysis after reviewing the high-level charts.

## Overall Performance Summary

| Metric | Total |
|---|---:|
| Total Spend | `$130,244.90` |
| Total Impressions | `40,473,185` |
| Total Clicks | `688,333` |
| Total Conversions | `13,363` |
| Average CTR | `1.70%` |
| Average CPA | `$9.75` |

## Platform Performance Summary

| Platform | Spend | Impressions | Clicks | Conversions | CTR | CPA | CPM | Spend Share |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Facebook | `$18,292.00` | `4,541,474` | `88,899` | `2,395` | `1.96%` | `$7.64` | `$4.03` | `14%` |
| Google | `$37,686.20` | `7,223,544` | `137,590` | `4,218` | `1.90%` | `$8.93` | `$5.22` | `29%` |
| TikTok | `$74,266.70` | `28,708,167` | `461,844` | `6,750` | `1.61%` | `$11.00` | `$2.59` | `57%` |

## Key Analysis Insights

### 1. TikTok drove the highest conversion volume

TikTok generated the highest number of conversions with **6,750 conversions**, which was higher than both Google and Facebook. It also received the largest share of spend at approximately **57% of total spend**.

This suggests TikTok was the strongest platform for scale and volume during the reporting period.

### 2. Facebook was the most cost-efficient platform

Facebook had the lowest average CPA at **$7.64**, despite having the lowest total spend. This means Facebook generated conversions more efficiently than the other two platforms.

From a performance marketing perspective, Facebook appears to be the strongest platform for cost efficiency.

### 3. Google showed strong intent-driven performance

Google had a strong CTR of **1.90%**, which was higher than TikTok. This makes sense because Google Search campaigns often capture users who already have active intent.

Google performed especially well in brand and shopping campaigns, where user intent is typically stronger.

### 4. TikTok had the lowest CPM

TikTok had the lowest CPM at **$2.59**, making it the most efficient platform for reach and impression volume. This supports TikTok as a strong discovery and awareness channel.

However, TikTok also had the highest CPA at **$11.00**, which means it was less efficient for direct conversion compared with Facebook and Google.

### 5. Platform performance depends on the business goal

There is no single best platform across every metric.

- For conversion volume: TikTok performed best
- For cost efficiency: Facebook performed best
- For high-intent clicks: Google performed best
- For low-cost reach: TikTok performed best

This is why the dashboard separates volume metrics and efficiency metrics.

## Campaign-Level Insights

### Top Campaigns by Conversion Volume

| Rank | Platform | Campaign | Conversions |
|---:|---|---|---:|
| 1 | TikTok | `Influencer_Collab` | `2,653` |
| 2 | TikTok | `Conversion_Focus` | `2,061` |
| 3 | Google | `Shopping_All_Products` | `1,801` |
| 4 | Google | `Search_Brand_Terms` | `1,445` |
| 5 | TikTok | `Awareness_GenZ` | `1,203` |

### Most Efficient Campaigns by CPA

| Rank | Platform | Campaign | CPA |
|---:|---|---|---:|
| 1 | Google | `Search_Brand_Terms` | `$5.10` |
| 2 | Facebook | `Conversions_Retargeting` | `$5.95` |
| 3 | Google | `Shopping_All_Products` | `$6.34` |
| 4 | Facebook | `Traffic_Drive_Jan` | `$7.52` |
| 5 | Facebook | `Brand_Awareness_Q1` | `$9.44` |

### Campaign Observations

- `Influencer_Collab` was the highest conversion campaign overall.
- `Conversion_Focus` on TikTok also generated strong conversion volume.
- `Search_Brand_Terms` had the best CPA, showing the value of high-intent branded search.
- `Conversions_Retargeting` on Facebook performed well with a low CPA, suggesting retargeting was effective.
- `Search_Generic_Terms` had a much higher CPA, indicating it may need optimization in keywords, bids, targeting, or landing page experience.
- `Video_Views_Campaign` had a high CPA, so it should likely be evaluated as an awareness campaign rather than a direct conversion campaign.

## Business Recommendations

Based on the dashboard analysis, the following recommendations can be considered:

### 1. Continue investing in TikTok for scale

TikTok is driving the largest conversion volume and the lowest CPM. It is useful for reach, discovery, and top-of-funnel scale.

### 2. Protect and optimize Facebook retargeting

Facebook has the strongest CPA efficiency, especially through retargeting. This channel should be protected because it appears to generate efficient conversions at a lower cost.

### 3. Prioritize high-intent Google campaigns

Google Brand Search and Shopping campaigns are performing well. These campaigns should remain active because they capture users who are already closer to conversion.

### 4. Review high-CPA campaigns

Campaigns with high CPA should be reviewed for:

- Audience targeting
- Creative quality
- Keyword relevance
- Landing page experience
- Bidding strategy
- Budget allocation

### 5. Add ROAS when revenue data is available

The current dashboard focuses on conversions and cost efficiency. If revenue or conversion value is available across all platforms, ROAS should be added as a future metric.

## How to Open the Dashboard

This dashboard does not require a backend server.

Steps:

1. Download or clone the repository.
2. Open the project folder.
3. Double-click the dashboard HTML file.
4. The dashboard will open directly in your browser.

If the dashboard file is renamed to `index.html`, it can also be published easily using GitHub Pages.


## Dashboard Walkthrough Summary

This dashboard was designed to support a simple five-minute walkthrough:

1. Introduce the project and objective
2. Explain the unified data model
3. Review the KPI scorecards
4. Compare platform-level performance
5. Explain spend distribution and daily trends
6. Review campaign-level conversion and efficiency charts
7. Walk through the campaign performance table
8. Close with recommendations and possible future enhancements


## Final Summary

This project demonstrates how raw advertising exports from multiple platforms can be cleaned, standardized, and converted into a meaningful performance dashboard. The dashboard makes it easier to compare platforms, evaluate campaign performance, understand budget allocation, and identify optimization opportunities.

The most important takeaway is that each platform plays a different role:

- TikTok is strongest for scale and reach
- Facebook is strongest for CPA efficiency
- Google is strongest for intent-driven performance

Together, the unified view provides a clearer understanding of overall paid media performance than reviewing each platform separately.
