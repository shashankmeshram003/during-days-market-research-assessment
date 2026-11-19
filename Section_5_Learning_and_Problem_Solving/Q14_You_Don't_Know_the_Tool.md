**You Don't Know the Tool**

My approach would be to learn quickly, practise safely, verify carefully and communicate
honestly.

**Step-by-step approach with breakdown of time spent of each step**


1. **Step 1: Clarify the task (10 min)** : Confirm the data source, what the report should show, the audience,
and which Excel version the team uses (XLOOKUP needs Microsoft 365 or Excel 2021+).

2. **Step 2: Learn XLOOKUP from reliable sources (30-45 min)** : Read Microsoft's official XLOOKUP
documentation and watch one or two short tutorials. XLOOKUP follows the pattern [=XLOOKUP(lookup_value, lookup_array,return_array, [if_not_found])] and is similar to VLOOKUP but more flexible.

3. **Step 3: Practise on a small sample first (30 min)** : I wouldn’t learn on the real report. I’d build a tiny practice sheet, for example 10 orders and a 10-row product list, and try [=XLOOKUP(B2, Products!A:A, Products!C:C, "Not found")]
That looks up each order’s product and returns its cost price. I’d test the “not found” message by entering a product that doesn’t exist, and try a lookup that returns the wrong column on purpose, so I recognise the mistake when I see it.

4. **Step 4: Check it against a method I already know (15 min)** : I’d compare my XLOOKUP results with VLOOKUP or INDEX-MATCH on the same sample. If the answers match, I know I’m using it correctly.
  
5. **Step 5: Build the real report (60-90 min)** : Clean the data first (consistent names, no duplicate keys, no extra spaces), because lookups fail on messy data. Add the XLOOKUP columns (e.g. cost price, category) to the main dataset. Calculate any needed fields (profit, margin) with formulas.Create the Pivot Table from the completed dataset, for example sales and profit by category and month.

6. **Step 6: Verify the results (30 min)** : Filter the lookup columns for “Not found” or errors and fix the cause. Spot-check a random sample of 10-20 rows against the source data. Make sure the Pivot Table total equals the total in the source data. Refresh the Pivot Table and confirm it updates correctly.

7. **Step 7: Present clearly (15 min)** : Label the sheets, format the numbers (currency, %), and add a short note on what the report shows and how the data was prepared. Keep the practice sheet separate, so the report stays clean.

8. **Step 8: Communicate and handle the risks** : If I get stuck: I’d give myself a time limit (e.g. 30 minutes), then ask a colleague or my manager a specific question, not “I don’t understand.”
If XLOOKUP isn’t available in the team’s Excel version: I’d use INDEX-MATCH or VLOOKUP, which give the same result, and tell my manager why.I’d mention early that XLOOKUP is new to me and that I’ve been learning it, so nobody is surprised, and I’d show how I verified the results.

**This way the report is delivered on time, and I can explain and defend every number in it.**