SELECT 'AWtoAP' as DateRange,
Avg(CASE When year(agreement_written) = year(curdate()) and quarter(agreement_written) = quarter(curdate()) Then AWtoAP End) As CurQ,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 1 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 1 QUARTER)) Then AWtoAP End) As TQ1,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 2 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 2 QUARTER)) Then AWtoAP End) As TQ2,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 3 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 3 QUARTER)) Then AWtoAP End) As TQ3
FROM SaleToPermit

UNION ALL

SELECT 'APtoFieldISS' as DateRange,
Avg(CASE When year(agreement_written) = year(curdate()) and quarter(agreement_written) = quarter(curdate()) Then APtoFieldISS End) As CurQ,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 1 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 1 QUARTER)) Then APtoFieldISS End) As TQ1,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 2 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 2 QUARTER)) Then APtoFieldISS End) As TQ2,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 3 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 3 QUARTER)) Then APtoFieldISS End) As TQ3
FROM SaleToPermit

UNION ALL 

SELECT 'FFComplete' as DateRange,
Avg(CASE When year(agreement_written) = year(curdate()) and quarter(agreement_written) = quarter(curdate()) Then FFComplete End) As CurQ,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 1 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 1 QUARTER)) Then FFComplete End) As TQ1,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 2 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 2 QUARTER)) Then FFComplete End) As TQ2,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 3 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 3 QUARTER)) Then FFComplete End) As TQ3
FROM SaleToPermit

UNION ALL

SELECT 'AWtoSel' as DateRange,
Avg(CASE When year(agreement_written) = year(curdate()) and quarter(agreement_written) = quarter(curdate()) Then AWtoSel End) As CurQ,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 1 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 1 QUARTER)) Then AWtoSel End) As TQ1,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 2 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 2 QUARTER)) Then AWtoSel End) As TQ2,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 3 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 3 QUARTER)) Then AWtoSel End) As TQ3
FROM SaleToPermit

UNION ALL

SELECT 'AWtoPermit' as DateRange,
Avg(CASE When year(agreement_written) = year(curdate()) and quarter(agreement_written) = quarter(curdate()) Then AWtoPermit End) As CurQ,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 1 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 1 QUARTER)) Then AWtoPermit End) As TQ1,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 2 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 2 QUARTER)) Then AWtoPermit End) As TQ2,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 3 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 3 QUARTER)) Then AWtoPermit End) As TQ3
FROM SaleToPermit

UNION ALL

SELECT 'PermitRecdtoStart' as DateRange,
Avg(CASE When year(agreement_written) = year(curdate()) and quarter(agreement_written) = quarter(curdate()) Then PermitRecdtoStart End) As CurQ,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 1 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 1 QUARTER)) Then PermitRecdtoStart End) As TQ1,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 2 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 2 QUARTER)) Then PermitRecdtoStart End) As TQ2,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 3 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 3 QUARTER)) Then PermitRecdtoStart End) As TQ3
FROM SaleToPermit

UNION ALL

SELECT 'PermitSubtoPermitApp' as DateRange,
Avg(CASE When year(agreement_written) = year(curdate()) and quarter(agreement_written) = quarter(curdate()) Then PermitSubtoPermitApp End) As CurQ,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 1 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 1 QUARTER)) Then PermitSubtoPermitApp End) As TQ1,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 2 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 2 QUARTER)) Then PermitSubtoPermitApp End) As TQ2,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 3 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 3 QUARTER)) Then PermitSubtoPermitApp End) As TQ3
FROM SaleToPermit

UNION ALL

SELECT 'AWtoStart' as DateRange,
Avg(CASE When year(agreement_written) = year(curdate()) and quarter(agreement_written) = quarter(curdate()) Then AWtoStart End) As CurQ,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 1 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 1 QUARTER)) Then AWtoStart End) As TQ1,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 2 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 2 QUARTER)) Then AWtoStart End) As TQ2,
Avg(CASE When year(agreement_written) = Year(Date_SUB(curdate(), INTERVAL 3 QUARTER)) and quarter(agreement_written) = Quarter(Date_SUB(curdate(), INTERVAL 3 QUARTER)) Then AWtoStart End) As TQ3
FROM SaleToPermit



