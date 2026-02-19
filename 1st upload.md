<style>
</style>

| Module Code | IY455 |
| --- | --- |
| Group | B   |
| Module Title | Information Systems Analysis and Design |
| Assessment Type | Coursework Stage 1 |
| Module Tutor Name | Mustafa Ghasim |
| Student ID Number | P500331 |
| Date of Submission | 19-02-2026 |

☒ *I confirm that this assignment is my own work. Where I have
referred to academic sources, I have provided in-text citations and included
the sources in the final reference list.*

 ☒ *Where I have used AI, I have
cited and referenced appropriately.*

Normalisation-

Normalisation is the
process of organizing data into well structured table and creating relationships
between them using normal forms to reduce redundancy.

Fong J.S.P and Yan K.W.T,
(2021)Information system Reengineering Integration and Normalization Retrieved
From: https://link.springer.com/book/10.1007/978-3-030-79584-9 [19-February-2026].

Advantages of
normalisation-

1.    Normalisation
removes duplicate data stored in multiple places.

2.    Since
duplicate data is minimized, storage space is used efficiently.

3.    Data
is structured clearly into related tables.

Mullins C.S.,Leong .H
(2002)Database administration Retrieved From: Database administration : the
complete guide to practices and procedures - Nottingham Trent University [19-
February- 2026]

Disadvantages of
normalisation-

1.    Normalisation
creates many tables, so it makes the database design more complex and harder to
understand for beginners

2.    Sql
queries become longer and more complex.

3.    Slower
performance in some cases.

Mullins C.S.,Leong
.H(2002)Database administration Retrieved From: Database administration : the
complete guide to practices and procedures - Nottingham Trent University [19-
February- 2026]

|     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 N.F |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| Loan No.(PK) | Copy No (PK) | DVD No.(PK) | DVD Title | DVD Starring Actor | DVD Year | Rental Cost | Copy No | Shelf Position | Borrower Name | Borrower Address | Borrower Total Fine | Borrower Status | Loan Date | Total loan Cost |     |
| LN74857 | CN1099 | DN198 | Raiders of the Lost Ark | Harrison Ford | 1981 | £3.50 | CN1099 | AV123 | Ben Jones | 28 Low Road, Nottingham<br> NG5 3PB | £0.00 | Allowed | 06-02-2002 | £8.00 |     |
| LN74857 | CN8739 | DN9829 | John Wick | Keanu Reeves | 2014 | £4.50 | CN8739 | AC8728 |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |

| 2nd N.F |     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- | --- |
| T0500331_Borrower |     |     |     |     |     |     |
| Loan No.(PK) | Borrower Name | Borrower Address | Borrower Total Fine | Borrower Status | Loan Date | Total loan Cost |
| LN74857 | Ben Jones | 28 Low Road, Nottingham<br> NG5 3PB | £0.00 | Allowed | 06-02-2002 | £8.00 |
|     |     |     |     |     |     |     |
| T0500331_DVD |     |     |     |     |     |     |
| DVD No.(PK) | DVD Title | DVD Starring Actor | DVD Year | Rental Category | Rental Cost |     |
| DN198 | Raiders of the Lost Ark | Harrison Ford | 1981 | Adventure | £3.50 |     |
| DN9829 | John Wick | Keanu Reeves | 2014 | Action | £4.50 |     |
| T0500331_LOAN |     |     |     |     |     |     |
| Loan No.(FK) | Copy No (PK) | DVD Status | Return Due Date |     |     |     |
| LN74857 | CN1099 | On Loan | 13-02-2002 |     |     |     |
| LN74857 | CN8739 | On Loan | 13-02-2002 |     |     |     |

| 3rd N.F |     |     |     |     |
| --- | --- | --- | --- | --- |
| T0500331_Borrower |     |     |     |     |
| Borrower No.(PK) | Borrower Name | Borrower Address | Borrower Total Fine | Borrower Status |
| BN1721 | Ben Jones | 28 Low Road, Nottingham<br> NG5 3PB | £0.00 | Allowed |
|     |     |     |     |     |
| T0500331_LOAN |     |     |     |     |
| Loan No.(PK) | Borrower No.(FK) | Loan Date | Total loan Cost |     |
| LN74857 | BN1721 | 06-02-2002 | £8.00 |     |
|     |     |     |     |     |
| T0500331_DVD |     |     |     |     |
| DVD No.(PK) | DVD Title | DVD Starring Actor | DVD Year |     |
| DN198 | Raiders of the Lost Ark | Harrison Ford | 1981 |     |
| DN9829 | John Wick | Keanu Reeves | 2014 |     |
|     |     |     |     |     |
| T0500331_COPY |     |     |     |     |
| Copy No (PK) | DVD No.(FK) | Shelf Position |     |     |
| CN1099 | DN198 | AV123 |     |     |
| CN8739 | DN9829 | AC8728 |     |     |
|     |     |     |     |     |
| T0500331_LOAN-ITEM |     |     |     |     |
| Loan No.(FK) | Copy No (FK) | Return Due Date | DVD Status |     |
| LN74857 | CN1099 | 13-02-2002 | On Loan |     |
| LN74857 | CN8739 | 13-02-2002 | On Loan |     |