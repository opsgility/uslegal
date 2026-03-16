---
lab:
  title: 'Lab Setup'
  description: 'Upload resource files and configure your environment for the US Legal Sales Copilot Workshop.'
  duration: 15 minutes
  level: 100
  islab: true
---

# Lab Setup

In this workshop, you'll use Microsoft 365 Copilot across Outlook, Excel, Teams, and Word to practice real sales scenarios for US Legal. First, download and upload the required resource files to OneDrive so Copilot can access them.

### Step 1: Download the Resource Files

1. In the Windows taskbar, select **Microsoft Edge**.
2. Navigate to the following URL to download the resource files:

    **[https://github.com/opsgility/uslegal/raw/refs/heads/main/USLegal-ResourceFiles/ResourceFiles.zip](https://github.com/opsgility/uslegal/raw/refs/heads/main/USLegal-ResourceFiles/ResourceFiles.zip)**

3. Once the download completes, open **File Explorer** and navigate to your **Downloads** folder.
4. Right-click the **ResourceFiles.zip** file and select **Extract All...**.
5. Choose a location to extract the files (your **Downloads** folder or **Desktop** is fine) and select **Extract**.
6. After extraction, you should see a folder containing the following seven files:
    - USLegal_Account_List.xlsx
    - USLegal_Competitor_Pricing.xlsx
    - USLegal_Company_Overview.docx
    - USLegal_Service_Catalog.docx
    - USLegal_Client_Account_History.docx
    - USLegal_Prospect_Meeting_Transcript.docx
    - USLegal_Client_QBR_Meeting_Transcript.docx

### Step 2: Upload Files to OneDrive

1. In **Microsoft Edge**, navigate to `https://www.office.com` and sign in with your Microsoft 365 credentials.
2. In **Microsoft 365**, select **Apps** in the navigation pane, then select **OneDrive**.
3. In **OneDrive**, in the top-left corner, select **+** (add new) > **File upload**.
4. Navigate to the folder where you extracted the resource files. Select **all seven files** and then select **Open** to upload them to **OneDrive**.
5. When the upload is complete, you should see **Uploaded 7 items to My files** in the bottom center of the screen.
6. Verify all seven files appear in your **OneDrive** root folder (or create a subfolder named **USLegal-ResourceFiles** and move them there for organization).
7. Leave **Edge** open and move on to the next section.

### Step 3: Open Files to Add Them to Your Most Recently Used List

When using Copilot, you may find that some files aren't immediately available in the suggestions. This occurs because certain Copilot experiences only reference files from the **Most Recently Used (MRU)** list, while others let you browse **OneDrive** directly.

To ensure the resource files are available to Copilot throughout the workshop:

1. In **OneDrive**, open **USLegal_Account_List.xlsx** in Excel for the web. Once it loads, you can close the tab.
2. Open **USLegal_Company_Overview.docx** in Word for the web. Once it loads, close the tab.
3. Open **USLegal_Client_Account_History.docx** in Word for the web. Once it loads, close the tab.

This adds them to your MRU list so Copilot can find them when you reference them in prompts. You'll open additional files as needed during each exercise.

> [!IMPORTANT]
> Microsoft 365 Copilot can only work with files saved to **OneDrive**. Files stored locally on your PC will need to be moved to **OneDrive** for Copilot to access them.

### Workshop Structure

This workshop is organized around the **dual mandate** that US Legal sales reps carry every day:

| Mandate | Focus |
|---|---|
| **Existing Business** | Maintain relationships, expand spend, grow reach within current buyers (new contacts, new departments, new service lines) |
| **Net New Business** | Prospect into new law firms, win new logos |

Every exercise is built around real scenarios you encounter daily. You'll practice with Copilot in the apps you already use — Outlook, Excel, Teams, and Word — and learn how to bridge Copilot outputs into your HubSpot workflow.

### Copilot Prompting Framework

One of the primary keys to effectively using Copilot is the quality of your prompts. A good Copilot prompt is built around four key elements:

- **Goal**. Clearly state what you want Copilot to do. *Example: "Draft a personalized check-in email to a client I haven't spoken to in 3 months."*

- **Context**. Provide background information so Copilot understands the situation. *Example: "This client is a mid-size litigation firm that currently uses our document retrieval service but not our compliance package."*

- **Sources**. Specify where Copilot should look for information. *Example: "Reference the attached account history document."*

- **Expectations**. Define how you want the response — tone, format, length. *Example: "Keep the email under 150 words, use a warm but professional tone, and include a specific reason to reconnect."*

Keep these four elements front and center as you practice creating prompts throughout this workshop.

