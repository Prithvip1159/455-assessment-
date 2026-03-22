| Module Code        | IY455                                   |
| ------------------ | --------------------------------------- |
| Group              | B                                       |
| Module Title       | Information Systems Analysis and Design |
| Assessment Type    | Coursework Stage 2                      |
| Module Tutor Name  | Mustafa Ghasim                          |
| Student ID Number  | P500331                                 |
| Date of Submission | 22-03-2026                              |

☒ *I confirm that this assignment is my own work. Where I have
referred to academic sources, I have provided in-text citations and included
the sources in the final reference list.*

 ☒ *Where I have used AI, I have
cited and referenced appropriately.*

|                                          |              |                         |                                 |                     |                 |             |                 |                |            |                 |
| ---------------------------------------- | ------------ | ----------------------- | ------------------------------- | ------------------- | --------------- | ----------- | --------------- | -------------- | ---------- | --------------- |
| Normalisation                            |              |                         |                                 |                     |                 |             |                 |                |            |                 |
|                                          |              |                         |                                 |                     |                 |             |                 |                |            |                 |
| Convert to 1 NF                          |              |                         |                                 |                     |                 |             |                 |                |            |                 |
|                                          |              |                         |                                 |                     |                 |             |                 |                |            |                 |
| Table 1: T0500331_Loan                   |              |                         |                                 |                     |                 |             |                 |                |            |                 |
|                                          |              |                         |                                 |                     |                 |             |                 |                |            |                 |
| Loan No.(PK)                             | Borrower No. | Borrower Name           | Borrower Address                | Borrower Total Fine | Borrower Status | Loan Date   | Total loan Cost |                |            |                 |
| LN74857                                  | BN1721       | Ben Jones               | 28 Low Road, Nottingham NG5 3PB | £0.00               | Allowed         | 06-02-2002  | £8.00           |                |            |                 |
|                                          |              |                         |                                 |                     |                 |             |                 |                |            |                 |
| Table 2: T0500331_DVD                    |              |                         |                                 |                     |                 |             |                 |                |            |                 |
| Composite Key =<br> (DVD No. , Loan No.) |              |                         |                                 |                     |                 |             |                 |                |            |                 |
| DVD No.                                  | Loan No.     | DVD Title               | DVD Starring Actor              | DVD Year            | Rental Category | Rental Cost | Copy No         | Shelf Position | DVD Status | Return Due Date |
| DN198                                    | LN74857      | Raiders of the Lost Ark | Harrison Ford                   | 1981                | Adventure       | £3.50       | CN1099          | AV123          | On Loan    | 13-02-2002      |
| DN9829                                   | LN74857      | John Wick               | Keanu Reeves                    | 2014                | Action          | £4.50       | CN8739          | AC8728         | On Loan    | 13-02-2002      |

<style>
</style>

|                            |                         |                                 |                     |                 |             |
| -------------------------- | ----------------------- | ------------------------------- | ------------------- | --------------- | ----------- |
| Convert<br> to 2 NF        |                         |                                 |                     |                 |             |
|                            |                         |                                 |                     |                 |             |
| Table 3: T0500331_Loan     |                         |                                 |                     |                 |             |
|                            |                         |                                 |                     |                 |             |
| Loan No.(PK)               | Borrower No.(FK)        | Loan Date                       | Total loan Cost     |                 |             |
| LN74857                    | BN1721                  | 06-02-2002                      | £8.00               |                 |             |
|                            |                         |                                 |                     |                 |             |
| Table 4: T0500331_Borrower |                         |                                 |                     |                 |             |
|                            |                         |                                 |                     |                 |             |
| Borrower No.(PK)           | Borrower Name           | Borrower Address                | Borrower Total Fine | Borrower Status |             |
| BN1721                     | Ben Jones               | 28 Low Road, Nottingham NG5 3PB | £0.00               | Allowed         |             |
|                            |                         |                                 |                     |                 |             |
| Table 5: T0500331_DVDLoan  |                         |                                 |                     |                 |             |
|                            |                         |                                 |                     |                 |             |
| DVD No. (PK, FK)           | Loan No. (PK, FK)       |                                 |                     |                 |             |
| DN198                      | LN74857                 |                                 |                     |                 |             |
| DN9829                     | LN74857                 |                                 |                     |                 |             |
|                            |                         |                                 |                     |                 |             |
| Table 6: T0500331_DVD      |                         |                                 |                     |                 |             |
|                            |                         |                                 |                     |                 |             |
| DVD No. (PK)               | DVD Title               | DVD Starring Actor              | DVD Year            | Rental Category | Rental Cost |
| DN198                      | Raiders of the Lost Ark | Harrison Ford                   | 1981                | Adventure       | £3.50       |
| DN9829                     | John Wick               | Keanu Reeves                    | 2014                | Action          | £4.50       |

<style>
</style>

|                                      |                         |                                 |                     |                     |
| ------------------------------------ | ----------------------- | ------------------------------- | ------------------- | ------------------- |
| Convert<br> to 3 NF                  |                         |                                 |                     |                     |
|                                      |                         |                                 |                     |                     |
|                                      |                         |                                 |                     |                     |
| Table 3: T0500331_Loan               |                         |                                 |                     |                     |
|                                      |                         |                                 |                     |                     |
| Loan No.(PK)                         | Borrower No.(FK)        | Loan Date                       |                     |                     |
| LN74857                              | BN1721                  | 06-02-2002                      |                     |                     |
|                                      |                         |                                 |                     |                     |
| Table 4: T0500331_Borrower           |                         |                                 |                     |                     |
|                                      |                         |                                 |                     |                     |
| Borrower No.(PK)                     | Borrower Name           | Borrower Address                | Borrower Status     |                     |
| BN1721                               | Ben Jones               | 28 Low Road, Nottingham NG5 3PB | Allowed             |                     |
|                                      |                         |                                 |                     |                     |
| Table 5: T0500331_LoanItem           |                         |                                 |                     |                     |
|                                      |                         |                                 |                     |                     |
| Copy No (PK)                         | Loan No. (FK)           | Return Due Date                 |                     |                     |
| CN1099                               | LN74857                 | 13-02-2002                      |                     |                     |
| CN8739                               | LN74857                 | 13-02-2002                      |                     |                     |
|                                      |                         |                                 |                     |                     |
| Table 6:<br> T0500331_RentalCategory |                         |                                 |                     |                     |
|                                      |                         |                                 |                     |                     |
| Rental Category(PK)                  | Rental Cost             | rental_duration_days            | fine_charge_per_day |                     |
| Adventure                            | £3.50                   |                                 |                     |                     |
| Action                               | £4.50                   |                                 |                     |                     |
|                                      |                         |                                 |                     |                     |
| Table 7: T0500331_DVDCopy            |                         |                                 |                     |                     |
| Copy No (PK)                         | DVD No. (FK)            | Shelf Position                  | DVD Status          |                     |
| CN1099                               | DN198                   | AV123                           | On Loan             |                     |
| CN8739                               | DN9829                  | AC8728                          | On Loan             |                     |
|                                      |                         |                                 |                     |                     |
| Table 8: T0500331_DVD                |                         |                                 |                     |                     |
| DVD No. (PK)                         | DVD Title               | DVD Starring Actor              | DVD Year            | Rental Category(FK) |
| DN198                                | Raiders of the Lost Ark | Harrison Ford                   | 1981                | Adventure           |
| DN9829                               | John Wick               | Keanu Reeves                    | 2014                | Action              |

### ERD TABLE

---

![CORRECT ERD FINAL VERSION.jpg](C:\private\brainrot\NTIC%20Sem%202\455\455%20stage%202\CORRECT%20ERD%20FINAL%20VERSION.jpg)

---

### SQL CODE

---

DROP DATABASE IF EXISTS dvd_loan_management;  
CREATE DATABASE dvd_loan_management;  
USE dvd_loan_management;  

-- 1. Borrower  
CREATE TABLE borrower (  
    borrower_no VARCHAR(6) PRIMARY KEY,  
    borrower_name VARCHAR(100) NOT NULL,  
    borrower_address VARCHAR(255) NOT NULL,  
    borrower_status ENUM('active', 'dormant', 'suspended', 'terminated') NOT NULL  
);  

-- 2. Rental Category  
CREATE TABLE rental_category (  
    rental_category VARCHAR(30) PRIMARY KEY,  
    rental_cost DECIMAL(5,2) NOT NULL,  
    rental_duration_days TINYINT UNSIGNED NULL,  
    fine_charge_per_day DECIMAL(5,2) NULL  
);  

-- 3. DVD  
CREATE TABLE dvd (  
    dvd_no VARCHAR(6) PRIMARY KEY,  
    dvd_title VARCHAR(200) NOT NULL,  
    star_actor VARCHAR(100) NOT NULL,  
    release_year YEAR NOT NULL,  
    rental_category VARCHAR(30) NOT NULL,  
    CONSTRAINT fk_dvd_category  
        FOREIGN KEY (rental_category)  
        REFERENCES rental_category(rental_category)  
);  

-- 4. DVD Copy  
CREATE TABLE dvd_copy (  
    copy_no VARCHAR(6) PRIMARY KEY,  
    dvd_no VARCHAR(6) NOT NULL,  
    shelf_position VARCHAR(20) NOT NULL,  
    dvd_status ENUM('available', 'on loan', 'overdue', 'reserved', 'missing') NOT NULL,  
    CONSTRAINT fk_copy_dvd  
        FOREIGN KEY (dvd_no)  
        REFERENCES dvd(dvd_no)  
);  

-- 5. Loan  
CREATE TABLE loan (  
    loan_no VARCHAR(8) PRIMARY KEY,  
    borrower_no VARCHAR(6) NOT NULL,  
    loan_date DATE NOT NULL,  
    CONSTRAINT fk_loan_borrower  
        FOREIGN KEY (borrower_no)  
        REFERENCES borrower(borrower_no)  
);  

-- 6. Loan Item  
CREATE TABLE loan_item (  
    loan_no VARCHAR(8) NOT NULL,  
    copy_no VARCHAR(6) NOT NULL,  
    return_due_date DATE NOT NULL,  
    actual_return_date DATE NULL,  
    fine_charge DECIMAL(5,2) NOT NULL DEFAULT 0.00,  
    fine_paid BOOLEAN NOT NULL DEFAULT FALSE,  
    PRIMARY KEY (loan_no, copy_no),  
    CONSTRAINT fk_loanitem_loan  
        FOREIGN KEY (loan_no)  
        REFERENCES loan(loan_no),  
    CONSTRAINT fk_loanitem_copy  
        FOREIGN KEY (copy_no)  
        REFERENCES dvd_copy(copy_no)  
);  

-- rental categories  
INSERT INTO rental_category (rental_category, rental_cost, rental_duration_days, fine_charge_per_day) VALUES  
('Action', 4.00, NULL, NULL),  
('Adventure', 3.50, NULL, NULL),  
('Animation', 3.50, NULL, NULL),  
('Biography', 3.80, NULL, NULL),  
('Comedy', 4.50, NULL, NULL),  
('Crime', 3.80, NULL, NULL),  
('Drama', 4.20, NULL, NULL),  
('Horror', 4.00, NULL, NULL),  
('Mystery', 3.80, NULL, NULL),  
('Romance', 4.50, NULL, NULL),  
('Sci-Fi', 4.50, NULL, NULL),  
('Superhero', 4.50, NULL, NULL),  
('Thriller', 4.50, NULL, NULL);  

-- DVDs  
INSERT INTO dvd (dvd_no, dvd_title, star_actor, release_year, rental_category) VALUES  
('DN0140', 'John Wick', 'Keanu Reeves', 2014, 'Action'),  
('DN0135', 'Prometheus', 'Noomi Rapace', 2012, 'Adventure'),  
('DN0102', 'Sing', 'Matthew McConaughey', 2016, 'Animation'),  
('DN083', 'Hidden Figures', 'Taraji P. Henson', 2016, 'Biography'),  
('DN0157', 'La La Land', 'Ryan Gosling', 2016, 'Comedy'),  
('DN056', 'Hounds of Love', 'Emma Booth', 2016, 'Crime'),  
('DN062', 'Arrival', 'Amy Adams', 2016, 'Drama'),  
('DN0171', 'Split', 'James McAvoy', 2016, 'Horror'),  
('DN0110', 'Shutter Island', 'Leonardo DiCaprio', 2010, 'Mystery'),  
('DN080', 'The Bad Batch', 'Keanu Reeves', 2016, 'Romance'),  
('DN093', 'Realive', 'Tom Hughes', 2016, 'Sci-Fi'),  
('DN050', 'Guardians of the Galaxy', 'Chris Pratt', 2014, 'Superhero'),  
('DN017', 'Mine', 'Armie Hammer', 2016, 'Thriller');  

-- borrowers  
INSERT INTO borrower (borrower_no, borrower_name, borrower_address, borrower_status) VALUES  
('BN1721', 'Ben Jones', '28 Low Road, Nottingham NG5 3PB', 'active'),  
('BN2001', 'Aisha Khan', '14 Trent Street, Derby DE1 2AB', 'active'),  
('BN2002', 'Mark Smith', '7 Forest Road, Leicester LE2 4GH', 'suspended');  

-- dvd copies  
INSERT INTO dvd_copy (copy_no, dvd_no, shelf_position, dvd_status) VALUES  
('CN1099', 'DN0135', 'AV123', 'available'),  
('CN8739', 'DN0140', 'AC8728', 'available'),  
('CN2001', 'DN050', 'SH100', 'available'),  
('CN2002', 'DN0171', 'HR210', 'overdue'),  
('CN2003', 'DN062', 'DR330', 'on loan'),  
('CN2004', 'DN0157', 'CO410', 'available'),  
('CN2005', 'DN056', 'CR510', 'available'),  
('CN2006', 'DN093', 'SF610', 'reserved');  

-- loans  
INSERT INTO loan (loan_no, borrower_no, loan_date) VALUES  
('LN74857', 'BN1721', '2026-03-10'),  
('LN74858', 'BN2001', '2026-03-11'),  
('LN74859', 'BN1721', '2026-03-15');  

-- loan items  
INSERT INTO loan_item (loan_no, copy_no, return_due_date, actual_return_date, fine_charge, fine_paid) VALUES  
('LN74857', 'CN1099', '2026-03-13', '2026-03-13', 0.00, TRUE),  
('LN74857', 'CN8739', '2026-03-13', '2026-03-15', 3.00, FALSE),  
('LN74858', 'CN2003', '2026-03-18', NULL, 0.00, FALSE),  
('LN74859', 'CN2005', '2026-03-18', '2026-03-20', 2.00, TRUE);  

-- views  
CREATE OR REPLACE VIEW v_loan_total_cost AS  
SELECT  
    l.loan_no,  
    ROUND(COALESCE(SUM(rc.rental_cost), 0), 2) AS total_loan_cost  
FROM loan l  
LEFT JOIN loan_item li ON l.loan_no = li.loan_no  
LEFT JOIN dvd_copy dc ON li.copy_no = dc.copy_no  
LEFT JOIN dvd d ON dc.dvd_no = d.dvd_no  
LEFT JOIN rental_category rc ON d.rental_category = rc.rental_category  
GROUP BY l.loan_no;  

CREATE OR REPLACE VIEW v_borrower_total_fine AS  
SELECT  
    b.borrower_no,  
    b.borrower_name,  
    ROUND(COALESCE(SUM(CASE  
        WHEN li.fine_paid = FALSE THEN li.fine_charge  
        ELSE 0  
    END), 0), 2) AS borrower_total_fine  
FROM borrower b  
LEFT JOIN loan l ON b.borrower_no = l.borrower_no  
LEFT JOIN loan_item li ON l.loan_no = li.loan_no  
GROUP BY b.borrower_no, b.borrower_name;  

-- outputs  
SHOW TABLES;  

SELECT * FROM borrower;  
SELECT * FROM rental_category;  
SELECT * FROM dvd;  
SELECT * FROM dvd_copy;  
SELECT * FROM loan;  
SELECT * FROM loan_item;  

SELECT * FROM v_loan_total_cost;  
SELECT * FROM v_borrower_total_fine;

---

### CODE SCREENSHOTS:

---

![Screenshot 2026-03-22 215418.png](C:\Users\Prithvi\OneDrive\Pictures\Screenshots\Screenshot%202026-03-22%20215418.png)

![Screenshot 2026-03-22 215649.png](C:\Users\Prithvi\OneDrive\Pictures\Screenshots\Screenshot%202026-03-22%20215649.png)

![Screenshot 2026-03-22 215746.png](C:\Users\Prithvi\OneDrive\Pictures\Screenshots\Screenshot%202026-03-22%20215746.png)

![Screenshot 2026-03-22 215814.png](C:\Users\Prithvi\OneDrive\Pictures\Screenshots\Screenshot%202026-03-22%20215814.png)

![Screenshot 2026-03-22 215838.png](C:\Users\Prithvi\OneDrive\Pictures\Screenshots\Screenshot%202026-03-22%20215838.png)

---

### PRINT SCREEN OF SQL OUTPUT

---

![Screenshot 2026-03-22 180945.png](C:\private\brainrot\NTIC%20Sem%202\455\455%20stage%202\stage%202%20sql%20output%20pics\Screenshot%202026-03-22%20180945.png)

![Screenshot 2026-03-22 181139.png](C:\private\brainrot\NTIC%20Sem%202\455\455%20stage%202\stage%202%20sql%20output%20pics\Screenshot%202026-03-22%20181139.png)

![Screenshot 2026-03-22 181245.png](C:\private\brainrot\NTIC%20Sem%202\455\455%20stage%202\stage%202%20sql%20output%20pics\Screenshot%202026-03-22%20181245.png)

![Screenshot 2026-03-22 181336.png](C:\private\brainrot\NTIC%20Sem%202\455\455%20stage%202\stage%202%20sql%20output%20pics\Screenshot%202026-03-22%20181336.png)

![Screenshot 2026-03-22 181420.png](C:\private\brainrot\NTIC%20Sem%202\455\455%20stage%202\stage%202%20sql%20output%20pics\Screenshot%202026-03-22%20181420.png)

![Screenshot 2026-03-22 181458.png](C:\private\brainrot\NTIC%20Sem%202\455\455%20stage%202\stage%202%20sql%20output%20pics\Screenshot%202026-03-22%20181458.png)

![Screenshot 2026-03-22 181529.png](C:\private\brainrot\NTIC%20Sem%202\455\455%20stage%202\stage%202%20sql%20output%20pics\Screenshot%202026-03-22%20181529.png)

![Screenshot 2026-03-22 181610.png](C:\private\brainrot\NTIC%20Sem%202\455\455%20stage%202\stage%202%20sql%20output%20pics\Screenshot%202026-03-22%20181610.png)

---
