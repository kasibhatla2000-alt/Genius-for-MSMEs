# Genius-for-zoho
Ledger-native credit scoring and loan quotes for Indian MSMEs. NUS BMF5342 Group 4 prototype (synthetic data).

**NUS MSc Finance · BMF5342 Financial Technology, Analytics, and AI · Group 4**
Status: prototype on synthetic data. Not an official Zoho product and not for real lending decisions.

**Authors**

1. Shreya Kasibhatla
2. Vivan Pande

**Run the prototype**

1. Open the notebook in Colab: Open in Colab
2. Choose Runtime → Run all. The first run builds the synthetic database and takes a few minutes; later runs load a cache.
3. Open the link printed by the last cell. The link is temporary: re-run the last cell for a new one.
   
Requires Python 3.10 or newer (provided by Colab).

**Try it**

1. Select Kaveri Foods and choose Read the books.
2. Choose Get my credit standing.
3. Open Borrow, enter ₹5,00,000 and 60 days, then choose Calculate my quote.
4. Compare with Sharma Traders at 14 days and at 60 days.
   
Sample firms (Sharma Traders, Kaveri Foods, Swift Freight) have made-up books.

**What is inside**

1. Genius Score: financial-only, learned monotone coefficients on 49 measures; data-integrity gate and knock-out rules
2. Grit: demonstrated recovery, kept separate from the score
3. Second Opinion: independent machine-learning challenger and review queue
4. Lender policy engine: versioned limits, prices and whole-book preview
5. Borrow engine: stressed affordability, full fees, effective cost
6. Ask Genius: rule-based answers, no external AI model
7. 46 automated tests
   
**Limitations**

1. All outcomes are synthetic; results test the method, not real repayments.
2. Grit adds no measured prediction in this test and is priced only as an assumed concession of at most 50 bps.
3. Pricing inputs and commercial figures are assumptions; see the report for the full list.
