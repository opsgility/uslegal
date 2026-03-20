---
lab:
  title: 'Exercise 3: Excel — Sales Intelligence & Account Health Analysis'
  description: 'Use Copilot in Excel Online to uncover revenue trends, identify at-risk accounts, spot cross-sell opportunities, and build a data-driven territory action plan.'
  duration: 55 minutes
  level: 100
  islab: true
  primarytopics:
    - Microsoft 365 Copilot
    - Excel Online
    - Sales Intelligence
    - Account Health
    - Territory Management
---

# Exercise 3: Excel — Sales Intelligence & Account Health Analysis (55 min)
---

Your CRM and internal reporting systems generate a wealth of data about your territory every month — but raw spreadsheets don't tell you where to focus. In this exercise, you use Copilot in Excel Online to transform five real operational reports into a clear picture of your territory's health: which accounts are growing, which are slipping, where to cross-sell, and what leading indicators signal about the months ahead.

By the end of this exercise, you will have used Copilot to surface insights that would take hours to find manually — and you'll have a prioritized action plan built directly from the data.

### Before You Begin

Copilot in Excel Online works directly with data in the open workbook. For Copilot to analyze your data:

- Data must be formatted as an **Excel Table** (select the data range, then **Insert > Table**).
- **AutoSave** must be turned on (files must be saved to OneDrive or SharePoint).
- Select **Copilot** in the Excel ribbon to open the Copilot pane.

> [!IMPORTANT]
> **Data Preparation:** Your report files include title rows at the top (company name, report title, date range) above the actual column headers. When formatting as a Table, **select only the data range starting at the column header row** — do not include the title rows. Copilot needs clean headers in row 1 of the table to work effectively. If needed, you can delete the title rows or copy the data range to a new sheet before formatting as a Table.

> [!NOTE]
> Copilot in Excel Online now supports **Agent Mode**, which can make changes directly in your workbook — inserting charts, adding formula columns, creating PivotTables, and applying conditional formatting. When the Copilot pane opens, look for **Agent Mode** or **Tools** to enable it. If your version only shows Copilot Chat, you can still get analysis and then apply suggestions manually.

### Your Files

Open each of the following files from your OneDrive and prepare them as described above. You will work with all five throughout this exercise:

| File | What It Contains | Key Columns |
|------|-----------------|-------------|
| **Movers-Decliners** | Account-level revenue comparison across all divisions | Firm Name, City, CYTD / PYTD / TTM by division |
| **TTM - Incoming Orders** | Trailing 12-month order volume by firm and contact | Firm, Type (New/Existing), monthly order counts, YTD Change % |
| **TTM - Records Sales** | Revenue by firm for the Records division | Firm, Line of Business, monthly revenue, CYTD / PYTD / YTD Change % |
| **TTM - Reporting Sales** | Revenue by firm across all Reporting service lines | Firm, Line of Business (Court Reporter, Interpreter, Videographer, etc.), monthly revenue |
| **TTM - Scheduled Depos** | Deposition scheduling volume by firm | Firm, Type (New/Existing), monthly counts, YTD Change % |

> [!NOTE]
> **Sheet naming convention:** Each workbook contains multiple sheets. The **first sheet** is named after the sales rep (e.g., "Gina Hardin") and contains the firm-level detail — one row per firm with monthly breakdowns. The remaining sheets are summaries: **"Rep's New and Existing Business"** breaks out New vs. Existing totals by month, and some files also include a **"Type New and Existing Business"** sheet with additional roll-ups. When this exercise refers to the "first sheet" or "firm-level detail sheet," it means the sheet named after the rep.

---

### Task 1: Territory Health Check — Movers & Decliners (12 min)

The Movers-Decliners report is your territory's vital signs. It shows which accounts are spending more this year vs. last year, and which are pulling back — broken out across every US Legal division.

1. In **Excel Online**, open **Movers-Decliners** from your OneDrive. Prepare the data as a Table (select from the column header row through the last data row, then **Insert > Table**).

2. Take a moment to scan the column structure. Notice that revenue is broken out by **division codes** (e.g., MR8CA, RB8CA, RB8FL, RB8NY, RB8SP, RB8TX) with CYTD, PYTD, and TTM for each, plus a **Total** column group.

3. Select **Copilot** in the ribbon. Enter:

    **Analyze this account data and categorize every firm into one of four groups: (1) "Growing" — Total CYTD is higher than PYTD, (2) "Declining" — Total PYTD was higher than CYTD and the firm has CYTD revenue, (3) "Lost" — firm had PYTD revenue but zero CYTD revenue, (4) "New" — firm has CYTD revenue but no PYTD revenue. How many firms fall into each category? What is the total revenue at risk in the Declining and Lost groups?**

4. Review Copilot's analysis. This gives you the big picture of territory health. Now ask it to dig into the most actionable segment:

    **List the top 10 firms by total TTM revenue that are in the "Declining" category — where CYTD is lower than PYTD. For each firm, show the firm name, city, Total CYTD, Total PYTD, and the dollar amount of the decline. Sort by largest dollar decline first. These are my highest-priority save opportunities.**

5. Insert the results. These are the accounts you need to reach out to immediately.

6. Now look for cross-division patterns:

    **Are there any firms that are declining in one division but growing in another? For example, a firm whose RB8CA revenue dropped but whose MR8CA revenue increased. Identify these firms — they may indicate a service shift rather than true attrition, and I want to understand what's happening before I make an outreach call.**

7. Finally, ask Copilot for a clean visualization:

    **Create a bar chart showing the top 15 firms by Total TTM revenue. Color-code or annotate to show whether each firm's CYTD is above or below their PYTD. Title it "Top 15 Accounts — Year-over-Year Trajectory."**

8. Insert the chart into a new sheet.

> [!TIP]
> **Why this matters:** The Movers-Decliners report is the fastest way to build a weekly call list. A firm showing a $20K decline is a conversation waiting to happen — but only if you catch it before the firm is fully lost. Copilot just turned a 160-row spreadsheet into a prioritized outreach plan in under two minutes.

---

### Task 2: Division Balance Analysis — MR8CA vs. RB8CA Cross-Sell Gap (10 min)

The Movers-Decliners report breaks revenue across multiple divisions. Two of the most important are **MR8CA** (Medical Records — California) and **RB8CA** (Reporting Business — California). Ideally, every firm that uses one service should be a candidate for the other. In practice, the data tells a very different story — and that gap represents your single largest cross-sell opportunity.

1. Staying in the **Movers-Decliners** workbook, ask Copilot:

    **For each firm, compare the MR8CA TTM revenue to the RB8CA TTM revenue. Categorize every firm into one of four groups: (1) "Both Divisions" — has revenue in both MR8CA and RB8CA, (2) "MR8CA Only" — has MR8CA revenue but zero RB8CA, (3) "RB8CA Only" — has RB8CA revenue but zero MR8CA, (4) "Neither" — no revenue in either. How many firms fall into each category? What is the total TTM revenue in each group?**

2. Review the results. You should see a striking imbalance — the vast majority of firms use only one division, not both. This is the cross-sell gap in plain numbers.

3. Now ask Copilot to surface the highest-value targets:

    **List the top 10 firms that have RB8CA revenue but zero MR8CA revenue, sorted by RB8CA TTM revenue descending. These are firms already using our Reporting services but not our Medical Records services — they're warm cross-sell targets. Show firm name, city, and RB8CA TTM revenue.**

4. Insert the results. Then ask for the opposite:

    **Now list the top 10 firms that have MR8CA revenue but zero RB8CA revenue, sorted by MR8CA TTM revenue descending. These firms use our Medical Records services but not Reporting — another cross-sell opportunity. Show firm name, city, and MR8CA TTM revenue.**

5. Insert both lists. Now ask Copilot to build a visualization that makes this gap impossible to ignore:

    **Create a new worksheet with a scatter chart. Plot each firm as a point with MR8CA TTM revenue on the X-axis and RB8CA TTM revenue on the Y-axis. Firms clustered along the X-axis are MR8CA-only; firms along the Y-axis are RB8CA-only. Firms near the origin use neither. Title it "Division Balance — Cross-Sell Opportunity Map." Add a reference line at a 1:1 ratio so balanced firms would fall on the diagonal. Label the outliers on the chart so key accounts are identifiable.**

6. Insert the chart. If Copilot can't produce the exact chart, try this alternative prompt:

    **Add a formula column that calculates each firm's "Division Balance Score" — the ratio of MR8CA TTM to the sum of MR8CA TTM + RB8CA TTM. A score of 0.5 means perfectly balanced. A score of 0 or 1 means entirely one-sided. Then create a bar chart of the top 20 firms by total TTM revenue, color-coded by whether their balance score is below 0.3 (RB8CA-heavy), above 0.7 (MR8CA-heavy), or between 0.3 and 0.7 (balanced).**

7. Save the chart worksheet. This becomes a visual tool you can bring to pipeline reviews or one-on-ones with your manager to show exactly where the cross-sell white space is.

> [!TIP]
> **The business case is simple:** A firm spending $300K in Medical Records but $0 in Reporting is not just a cross-sell opportunity — it's a relationship risk. If a competitor lands their Reporting business first, it creates a wedge into your Records revenue too. These charts turn that abstract risk into a concrete call list.

---

### Task 3: Revenue Deep-Dive — Reporting Sales by Service Line (12 min)

The Reporting Sales file is your richest data set — it breaks revenue down by firm, by individual service line (Court Reporter, CER Transcriptionist, Interpreter, Videographer, Technician, Process Service, and more), and by New vs. Existing business. This is where cross-sell opportunities hide.

1. Open **TTM - Reporting Sales** in Excel Online. Navigate to the **Rep's New and Existing Business** sheet and format the data range as a Table.

2. Select **Copilot** and enter:

    **Summarize this data by Line of Business. For each service line, show: Total revenue for the full period, CYTD revenue, PYTD revenue, YTD change amount, and YTD change percent. Which service lines are growing? Which are declining? Rank them from strongest growth to steepest decline.**

3. Review the results. You should see a clear story: some service lines are surging while others are flat or declining. Now ask Copilot to help you understand the composition:

    **What percentage of total Reporting revenue comes from New business vs. Existing business? Break this down by service line. Which service lines have the highest share of New business revenue? This tells me where my prospecting efforts are paying off and where I'm still dependent on the existing book.**

4. Insert the results. Now switch to the **first sheet** (named after the sales rep — this is the firm-level detail sheet with individual account rows) and format it as a Table. Ask:

    **Identify firms that are currently using only one Reporting service line (for example, only Court Reporter but no Videographer, Interpreter, or CER Transcriptionist). List the top 20 of these single-service firms by total revenue, along with which service they currently use. These are my best cross-sell targets — they're already spending with us but could be using more of our services.**

5. Insert the cross-sell target list.

6. Ask Copilot to find patterns in the monthly trends:

    **Look at the monthly revenue columns across all firms. Are there seasonal patterns? Which months had the highest and lowest total revenue? Is there a trend — is revenue accelerating, decelerating, or stable over the trailing 12 months? Show this as a line chart of total monthly revenue.**

7. Insert the chart.

> [!NOTE]
> **Cross-sell strategy:** A firm spending $50K/year on Court Reporting but using no other services represents significant expansion potential. Your Copilot analysis just identified those firms in seconds — keep this list for your next pipeline review.

---

### Task 4: Leading Indicators — Incoming Orders & Scheduled Depositions (12 min)

Revenue is a lagging indicator — it tells you what already happened. Order volume and deposition scheduling are **leading indicators** that signal what's coming next month. In this task, you correlate two data sets to spot early warnings and confirm growth trends.

1. Open **TTM - Incoming Orders** in Excel Online. Navigate to the **Rep's New and Existing Business** sheet and format as a Table. Ask Copilot:

    **Analyze the trend in total incoming orders month by month. Is order volume increasing, decreasing, or flat? Calculate the 3-month moving average for the last 6 months to smooth out noise. Also compare New vs. Existing order volume — is new business order flow growing fast enough to offset any decline in existing business?**

2. Review the analysis. Now open **TTM - Scheduled Depos** in a separate tab. Format the **Rep's New and Existing Business** sheet as a Table. Ask Copilot:

    **Show me the monthly trend in total scheduled depositions. Compare Existing business depo volume to New business depo volume over time. What's the YTD change for each? Is the growth in depositions accelerating or slowing down?**

3. Now comes the insight that matters — connecting the two data sets. Return to the **first sheet** in the Incoming Orders workbook (the firm-level detail sheet named after the sales rep), format as a Table, and ask:

    **List all firms that had incoming orders in the first half of the period (March–August 2025) but have had zero or declining orders in the most recent 3 months (December 2025–February 2026). These are accounts that may be going dormant — I need to re-engage them before they're fully lost.**

4. Insert the dormant-risk list.

5. Now look for the opposite pattern — emerging accounts:

    **Which firms had no orders in the first half of the period but have started placing orders in the last 3–4 months? These are new relationships ramping up — I want to nurture them and accelerate their growth. Show firm name, city, contact name, first order date, and total recent order count.**

6. Insert the emerging accounts list.

> [!TIP]
> **Leading vs. lagging:** If your deposition count is up 67% YTD but your incoming orders are down 16%, that divergence tells a story. Depositions reflect business already in the pipeline; declining orders signal a potential future slowdown. Use Copilot to catch these divergences early so you can act before the revenue impact hits.

---

### Task 5: Records Revenue & New Business Health (8 min)

The Records Sales file tracks a different revenue stream — record retrieval services. Comparing Records performance against Reporting performance reveals whether your territory's growth is broad-based or concentrated in one area.

1. Open **TTM - Records Sales** in Excel Online. Navigate to the **Type New and Existing Business** sheet and format as a Table. Ask Copilot:

    **Compare Existing business revenue to New business revenue for Records. Existing is declining — by how much in both dollars and percentage? New business started generating revenue midway through the year — at the current monthly run rate, will New business revenue offset the Existing decline by year-end? Project this forward and show me the gap.**

2. Review the projection. Then switch to the **first sheet** (the firm-level detail sheet named after the sales rep), format as a Table, and ask:

    **Identify the top 10 firms by Records revenue decline (largest drop from PYTD to CYTD). For each, show the firm name, CYTD revenue, PYTD revenue, dollar decline, and percent decline. Flag any firms that also appear to have a "Do Not Sell" or collection status if that data is present. These are the accounts I need to understand — are they leaving us or just reducing volume?**

3. Insert the at-risk Records accounts list.

4. Ask one final cross-reference question:

    > Note: Click on the **+** sign in the copilot prompt area and select the **TTM-Reporting Sales** spreadsheet. Then execute the following prompt

    **Among firms that are declining in Records, are any of them growing in the Reporting Sales file? I want to know if certain firms are shifting their business from Records to Reporting services — that's a different situation from a firm that's leaving us entirely.**

> [!NOTE]
> If Copilot cannot cross-reference files directly, note the top declining Records firms and manually check them in the Reporting Sales file. This cross-file comparison is one of the highest-value analyses a sales rep can do.

---

### Task 6: Build Your Quarterly Action Plan (6 min)

Now bring it all together. Using the insights you've gathered across all five files, ask Copilot to help you synthesize an action plan.

1. Return to any of your open files. Ask Copilot:

    **Based on everything in this workbook, help me build a prioritized action plan for the next 30 days. Create a table with columns for: Priority (1–10), Firm Name, Action (Save / Cross-Sell / Nurture / Re-engage), Reason (what the data shows), and Estimated Revenue Impact. Populate it with the most actionable opportunities from this data.**

2. Insert the action plan into a new sheet.

3. Ask Copilot to add conditional formatting to make the plan visual:

    **Apply conditional formatting to the Priority column — green for priorities 1–3, yellow for 4–6, red for 7–10. Also format the Estimated Revenue Impact column as currency.**

4. Save this sheet — it becomes your weekly operating rhythm.

> [!WARNING]
> Copilot in Excel may occasionally generate insights that don't perfectly match the data, particularly when calculating percentages or making projections. Always spot-check Copilot's top results against the source data before using them in client conversations or pipeline reviews.

---

### Optional: Explore Your Own Territory Perspective

If you're working with your own data exports (rather than sample files), take 5–10 minutes to explore questions specific to your territory, market, or role. Here are some ideas to try:

**Territory Strategy:**
> "Which geographic markets (cities) contribute the most revenue? Are any markets growing that I should invest more time in? Create a chart of revenue by city."

**Client Relationship Health:**
> "Sort all firms by 'Last Sale' or 'Last Ordered' date. Which of my top 20 revenue accounts haven't placed an order in the last 60 days? That's a red flag I need to investigate."

**Service Mix Optimization:**
> "What's the average number of service lines per firm in my top 25 accounts vs. my bottom 25? Is there a correlation between service breadth and total revenue?"

**New Business Pipeline:**
> "Plot the monthly trend of New business revenue and New business order count on the same chart. Is new business accelerating or plateauing? When did the inflection point happen?"

**Contact Intelligence:**
> "Which contacts (by name) are responsible for the most order volume? Are there firms where only one contact places orders — meaning I have single-point-of-failure risk?"

Pick one or more, submit them to Copilot, and iterate to refine the output. The best insights often come from the second or third follow-up question.

---

### Key Takeaways

By completing this exercise, you've demonstrated how Copilot in Excel Online can:

- **Segment accounts** into actionable categories (Growing, Declining, Lost, New) in seconds
- **Expose division balance gaps** — visually mapping which firms are one-sided between MR8CA and RB8CA to reveal cross-sell white space worth hundreds of thousands of dollars
- **Identify cross-sell opportunities** by finding single-service firms with high revenue
- **Spot leading indicators** by comparing order volume trends to revenue trends
- **Surface at-risk accounts** before the revenue impact materializes
- **Build prioritized action plans** directly from the data rather than gut feel

These are the same analyses that top-performing reps do regularly — Copilot just compresses hours of spreadsheet work into minutes of conversation.
