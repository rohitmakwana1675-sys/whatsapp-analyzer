# GroupDNA: WhatsApp Chat Analyzer 

A Python-based data analysis tool that transforms raw, exported WhatsApp group chat logs into fun, comprehensive, and actionable insights. 

> **Note:** This is a minor project developed as part of an assignment by **The Unlox Academy**. 

## Overview

GroupDNA moves beyond basic message counting. By parsing standard WhatsApp `.txt` exports, this script leverages Python and NumPy to analyze group dynamics, track activity trends, and even assign humorous "Personality Archetypes" to group members based on their texting habits.

##  Features

* **Chat Parsing Engine:** Cleans and processes raw WhatsApp data, effectively handling timestamps, senders, media omissions, and deleted messages.
* **Activity Heatmap:** Uses a NumPy matrix to generate an ASCII heatmap, visualizing the group's most active hours of the day.
* **Response Patterns & Silent Streaks:** Calculates average response times to identify the fastest and slowest repliers, alongside tracking the longest streaks of inactivity.
* **Vocabulary Analysis:** Filters out common stop-words and punctuation to extract the group's top 10 most frequently used words.
* **Personality Archetypes:** Custom algorithms analyze texting behavior to assign titles such as:
    * *The Spammer* (longest consecutive message bursts)
    * *The Group Mom* (highest usage of caring keywords)
    * *The Night Owl* (most active between 11 PM and 4 AM)
    * *The Drama Queen* (excessive use of all-caps and exclamation marks)
    * *The Storyteller* (highest average words per message)
    * *The Ghost* (highest percentage of days silent)
    * *The Lazy Texter* (lowest average words per message)

##  Tech Stack

* **Language:** Python 3.x
* **Libraries:** `numpy`, `datetime`, `string`

## How to Use

1.  **Export your WhatsApp Chat:** * Open a WhatsApp group chat on your phone.
    * Tap the group name > **Export Chat** > **Without Media**.
    * Save the exported `.txt` file to your project directory.
2.  **Rename the File:**
    * Rename the exported text file to `hostel_bois.txt` (or update the filename in the `run_groupdna_analysis()` function call at the bottom of the script).
3.  **Run the Script:**
    * Execute the script in your terminal:
        ```bash
        python whatsapp analyzer.py
        ```
4.  **View the Report:**
    * The terminal will output a clean, formatted "GroupDNA Report" containing all the calculated metrics and insights.

## 🤝 Acknowledgments
* Built as a minor project for **The Unlox Academy**.
