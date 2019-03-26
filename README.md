# dep-cleaner

## Purpose
- Take data downloaded from rs.pmi.org
- Convert date formats to sqlite3-friendly date format
- Split the multiple-field values into separate CSV files

## Conversions
- The following date fields converted into a sqlite3-friendly format
  - PMPDate
  - PMIJoinDate
  - PMIExpirationDate
  - JoinDate
  - ExpirationDate
  - RecordEdited
  - DataDate

## Output
Multiple CSV files - all suitable for import using sqlite3:
- dep.csv: Main data table
- chapters.csv: Normalized contents of Chapters field (if applicable)
- sigs.csv: Normalized contents of SIGs field
- industrycodes.csv: Normalized contents of IndustryCodes field
- occupationcodes.csv: Normalized contents of OccupationCodes field
