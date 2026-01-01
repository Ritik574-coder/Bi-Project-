## DAX QUERY

**Dataset:** `'ATM Transactions Data'`

```DAX
DEFINE

/* =========================
   TRANSACTION MEASURES
   ========================= */

MEASURE 'ATM Transactions Data'[Total Financial Transactions] =
SUM ( 'ATM Transactions Data'[Fin Txn] )

MEASURE 'ATM Transactions Data'[Total Non-Financial Transactions] =
SUM ( 'ATM Transactions Data'[Non Fin Txn] )

MEASURE 'ATM Transactions Data'[Total Monthly Transactions] =
SUM ( 'ATM Transactions Data'[Monthly Txn] )

MEASURE 'ATM Transactions Data'[Average Daily Transactions] =
AVERAGE ( 'ATM Transactions Data'[AVG Total TXN] )


/* =========================
   REVENUE MEASURES
   ========================= */

MEASURE 'ATM Transactions Data'[Transaction Revenue] =
SUM ( 'ATM Transactions Data'[Monthly Rev] )

MEASURE 'ATM Transactions Data'[MHA Revenue Total] =
SUM ( 'ATM Transactions Data'[MHA Revenue] )

MEASURE 'ATM Transactions Data'[Total ATM Revenue] =
SUM ( 'ATM Transactions Data'[ATM Rev Total] )

MEASURE 'ATM Transactions Data'[Average Revenue per ATM] =
DIVIDE (
    [Total ATM Revenue],
    DISTINCTCOUNT ( 'ATM Transactions Data'[ATM id] )
)


/* =========================
   COST MEASURES
   ========================= */

MEASURE 'ATM Transactions Data'[Total Operating Cost] =
SUM ( 'ATM Transactions Data'[Total Cost] )

MEASURE 'ATM Transactions Data'[Fixed Cost] =
SUMX (
    'ATM Transactions Data',
    'ATM Transactions Data'[RENT]
    + 'ATM Transactions Data'[EBILL]
    + 'ATM Transactions Data'[ATM AMC]
    + 'ATM Transactions Data'[VSAT AMC]
    + 'ATM Transactions Data'[UPS AMC]
)

MEASURE 'ATM Transactions Data'[Maintenance Cost] =
SUMX (
    'ATM Transactions Data',
    'ATM Transactions Data'[FLM]
    + 'ATM Transactions Data'[SUPPLIES]
    + 'ATM Transactions Data'[Site Maint  (Non Asset)]
)

MEASURE 'ATM Transactions Data'[Penalty & Compensation Cost] =
SUMX (
    'ATM Transactions Data',
    'ATM Transactions Data'[Penalty]
    + 'ATM Transactions Data'[Compensation]
    + 'ATM Transactions Data'[EJ]
)


/* =========================
   PROFITABILITY MEASURES
   ========================= */

MEASURE 'ATM Transactions Data'[Gross Profit Amount] =
SUM ( 'ATM Transactions Data'[Gross Profit] )

MEASURE 'ATM Transactions Data'[Gross Profit Percentage] =
DIVIDE (
    [Gross Profit Amount],
    [Total ATM Revenue]
)

MEASURE 'ATM Transactions Data'[Profit per ATM] =
DIVIDE (
    [Gross Profit Amount],
    DISTINCTCOUNT ( 'ATM Transactions Data'[ATM id] )
)


/* =========================
   OPERATIONAL MEASURES
   ========================= */

MEASURE 'ATM Transactions Data'[Average Uptime Percentage] =
AVERAGE ( 'ATM Transactions Data'[Up Time] )

MEASURE 'ATM Transactions Data'[Average Effective Days] =
AVERAGE ( 'ATM Transactions Data'[Effective days] )

MEASURE 'ATM Transactions Data'[Revenue per Effective Day] =
DIVIDE (
    [Total ATM Revenue],
    SUM ( 'ATM Transactions Data'[Effective days] )
)


/* =========================
   RISK & LOSS MEASURES
   ========================= */

MEASURE 'ATM Transactions Data'[Loss Making ATM Count] =
CALCULATE (
    DISTINCTCOUNT ( 'ATM Transactions Data'[ATM id] ),
    'ATM Transactions Data'[Gross Profit] < 0
)

MEASURE 'ATM Transactions Data'[Profitable ATM Count] =
CALCULATE (
    DISTINCTCOUNT ( 'ATM Transactions Data'[ATM id] ),
    'ATM Transactions Data'[Gross Profit] > 0
)

MEASURE 'ATM Transactions Data'[Loss Percentage] =
DIVIDE (
    [Loss Making ATM Count],
    DISTINCTCOUNT ( 'ATM Transactions Data'[ATM id] )
)


/* =========================
   EFFICIENCY MEASURES
   ========================= */

MEASURE 'ATM Transactions Data'[Revenue per Transaction] =
DIVIDE (
    [Total ATM Revenue],
    [Total Monthly Transactions]
)

MEASURE 'ATM Transactions Data'[Cost per Transaction] =
DIVIDE (
    [Total Operating Cost],
    [Total Monthly Transactions]
)


/* =========================
   FINAL OUTPUT TABLE
   ========================= */

EVALUATE
SUMMARIZECOLUMNS (
    "Total Financial Txn",        [Total Financial Transactions],
    "Total Non-Financial Txn",    [Total Non-Financial Transactions],
    "Total Monthly Txn",          [Total Monthly Transactions],
    "Avg Daily Txn",              [Average Daily Transactions],

    "Transaction Revenue",        [Transaction Revenue],
    "MHA Revenue",                [MHA Revenue Total],
    "Total ATM Revenue",          [Total ATM Revenue],
    "Avg Revenue per ATM",        [Average Revenue per ATM],

    "Total Operating Cost",       [Total Operating Cost],
    "Fixed Cost",                 [Fixed Cost],
    "Maintenance Cost",           [Maintenance Cost],
    "Penalty & Compensation",     [Penalty & Compensation Cost],

    "Gross Profit",               [Gross Profit Amount],
    "Gross Profit %",             [Gross Profit Percentage],
    "Profit per ATM",             [Profit per ATM],

    "Avg Uptime %",               [Average Uptime Percentage],
    "Avg Effective Days",         [Average Effective Days],
    "Revenue per Day",            [Revenue per Effective Day],

    "Loss ATM Count",             [Loss Making ATM Count],
    "Profitable ATM Count",       [Profitable ATM Count],
    "Loss %",                     [Loss Percentage],

    "Revenue per Txn",            [Revenue per Transaction],
    "Cost per Txn",               [Cost per Transaction]
)
```

---
