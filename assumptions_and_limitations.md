# Assumptions and Limitations

## Assumptions
- Source files are treated as authoritative public reporting datasets.
- Shared fields such as year and department name were used to structure relationships across tables.
- Aggregate totals are calculated in the reporting layer where appropriate rather than relying on mixed total rows in the source files.
- Simplified map fields were created to support clearer geographic visuals.

## Limitations
- The project uses aggregate workforce data, not employee-level data.
- It cannot support employee-level HR analytics such as turnover, hires, terminations, or retention calculations.
- Some source files include suppressed values or special geography categories that require interpretation.
- Geographic reporting is limited by source definitions such as NCR and Outside of Canada.
- The project is designed as a workforce reporting case study, not a full HRIS analytics build.


