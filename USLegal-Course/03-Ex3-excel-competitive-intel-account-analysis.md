---
lab:
  title: 'Exercise 3: Excel — Competitive Intel & Account Analysis'
  description: 'Use Copilot in Excel to analyze competitor pricing data, identify expansion opportunities in account lists, and prioritize prospects.'
  duration: 35 minutes
  level: 100
  islab: true
  primarytopics:
    - Microsoft 365 Copilot
    - Excel
    - Competitive Analysis
    - Account Prioritization
---

# Exercise 3: Excel — Competitive Intel & Account Analysis (35 min)
---

In this exercise, you use Copilot in Excel to turn raw data into actionable sales intelligence. You'll analyze competitor pricing to find where US Legal has an advantage, examine your account list for expansion opportunities, and prioritize your prospecting targets for the quarter. These are high-value activities that directly support both sides of your dual mandate.

### Before You Begin

Copilot in Excel works directly with data in the open workbook. For Copilot to analyze your data:
- Data must be formatted as an **Excel Table** (select your data range, then **Insert > Table**).
- **AutoSave** must be turned on (the file must be saved to OneDrive).
- Select **Copilot** in the Excel ribbon to open the Copilot pane.

> [!NOTE]
> Copilot in Excel is transitioning from **App Skills** to **Agent Mode**. If the Copilot menu displays two options (**Chat** and **App Skills**), select **App Skills** to work directly in the open workbook. If your version has transitioned to Agent Mode, select **Copilot** in the ribbon, then use **Tools > Agent Mode**. If neither option is available, use **Copilot Chat** and apply its suggestions manually.

---

### Task 1: Analyze competitor pricing data (15 min)

Your manager shared a spreadsheet containing competitive pricing intelligence gathered from public sources, client feedback, and RFP responses. You need to find where US Legal has pricing advantages and where you're vulnerable.

1. In **Excel for the web**, open the **USLegal_Competitor_Pricing.xlsx** file from your OneDrive (**USLegal-ResourceFiles** folder).

2. Take a moment to review the data. The spreadsheet contains columns for:
    - Competitor Name
    - Service Category (Document Retrieval, Court Filing, Compliance, Process Service, etc.)
    - Pricing Model (per transaction, monthly flat rate, tiered)
    - Price Point (low / mid / high range)
    - Market Segment (small firms, mid-size firms, large firms)
    - Differentiator / Notes

3. Ensure the data is formatted as a Table. If not, select the data range and go to **Insert > Table**.

4. Select **Copilot** in the Excel ribbon. In the Copilot pane, enter:

    **Summarize the key patterns in this competitive pricing data. Which service categories show the most price variation across competitors? Where does US Legal appear to have a pricing advantage, and where are we most vulnerable?**

5. Review Copilot's analysis. Ask a follow-up question:

    **Create a summary table comparing US Legal's pricing position against the top 3 competitors for each service category. Include columns for Competitor, Service, Their Price Range, US Legal Price Range, and Advantage (US Legal / Competitor / Even).**

6. If Copilot offers to insert the summary into a new sheet, select that option.

7. Now ask Copilot to visualize the data:

    **Create a bar chart showing average price points by service category, grouped by competitor. This will help me see at a glance where we're priced competitively.**

8. Insert the chart into a new sheet.

9. Ask one more analytical question:

    **Based on this pricing data, what are 3 talking points I could use when a prospect says "your competitor is cheaper"? Focus on total cost of ownership, service bundling advantages, and areas where our pricing is actually lower.**

10. Copy these talking points — you'll use them in the Word exercise later.

> [!NOTE]
> **HubSpot Bridge:** After completing your competitive analysis, update relevant competitor fields in HubSpot deal records. If you've identified pricing advantages for specific service categories, note these in the deal's "Competitive Notes" field so other reps can benefit.

---

### Task 2: Analyze your account list for expansion opportunities (12 min)

You have a list of existing accounts with their current services, contract values, firm size, and engagement metrics. You need to figure out where you have the best expansion potential.

1. In **Excel for the web**, open the **USLegal_Account_List.xlsx** file from your OneDrive (**USLegal-ResourceFiles** folder).

2. Review the data. The spreadsheet contains:
    - Firm Name
    - Firm Size (# of attorneys)
    - Current Services (which US Legal services they use)
    - Annual Contract Value
    - Contract Renewal Date
    - Last Contact Date
    - Engagement Score (1-10, based on recent interaction frequency)
    - Region
    - Notes

3. Ensure the data is formatted as a Table. Select **Copilot** in the Excel ribbon and enter:

    **Look at this account list and identify where I have the best expansion potential. Consider factors like: firms that only use 1-2 of our services (room to cross-sell), larger firms with lower contract values relative to their size, and accounts with high engagement scores that might be receptive to expansion conversations.**

4. Review Copilot's analysis. Follow up with:

    **Create a new column called "Expansion Priority" that ranks each account as High, Medium, or Low based on the expansion potential factors you identified. Add another column called "Recommended Next Service" suggesting which US Legal service to pitch next based on what they currently use and their firm type.**

5. Insert the results into the workbook.

6. Now ask Copilot to help you prioritize your quarter:

    **Help me prioritize which accounts to focus on this quarter. I can realistically have deep expansion conversations with 8-10 accounts. Rank the top 10 accounts by expansion opportunity, considering: contract renewal timing (accounts renewing soon are more urgent), engagement score, and revenue upside. Present this as a prioritized table.**

7. Insert the prioritized list into a new sheet.

> [!WARNING]
> Copilot in Excel may occasionally generate insights that don't perfectly match the data. Always verify Copilot's calculations and rankings against the source data before using them in client conversations.

---

### Task 3: Spot patterns and create prospect prioritization (8 min)

Finally, you want to prioritize your net-new prospecting efforts.

1. Return to the **USLegal_Account_List.xlsx** file (it also contains a second sheet with prospect data).

2. Select the **Prospects** sheet tab. This contains firms you're targeting but haven't won yet, with columns for firm size, practice areas, region, estimated deal value, and competitive situation.

3. Ask Copilot:

    **Help me prioritize which prospects to focus on this quarter. Consider firm size (larger firms = bigger deals), whether they're in a region where we already have strong references, and competitive situation (prospects currently unhappy with their provider are warmer). Rank the top 10 and explain your reasoning.**

4. Review and insert the results.

5. Ask one final question:

    **What patterns do you see across my most successful existing accounts that I should look for when qualifying new prospects? Compare my top-performing accounts (by contract value and engagement score) to this prospect list and flag any prospects that match the pattern.**

6. Review the insights. These patterns can inform your prospecting strategy and help you focus on firms most likely to convert.

---

### Hands-On Practice: Your Turn

Using either the competitor pricing data or the account list, ask Copilot a question that's relevant to your actual territory. Ideas:
- "Which accounts have renewal dates in the next 90 days and low engagement scores?" (churn risk)
- "What's the average contract value by firm size? Are there outliers I should investigate?"
- "Compare pricing across regions — are there geographic patterns?"

