# Log_Analyzer
Simple Log Analyzer for IARU HF contest
rev 1.0, by OE8TED

Two different Cabrillo logs can be opened, analyzed and compared.
Analysis focuses on hourly and 10min QSO rates, worked zones, continents and points.
A basic points per QSO calculation resolves zones over multiple continents.
Zone and continent of the respective log should be set before the log is opened. Else QSO points are not calculated correctly.
Diagrams of each analysis are saved as well as logs per band and mode.
In total 240 files are written in ~70s, if all analysis options are selected.
What this program can not do:
- Remove duplicate entries: All dupes are always considered as those contribute to QSO rates.
- Any result calculation: This is done much better by any dedicated contest logging software.
- Analyze other than IARU HF contests

Log Analzyer is written in Python 3.13 and compiled with Nuitka to run under Windows 10 (64bit).
A distribtion package for Win10 64bit is available for download.
Just unzip the content in a directory and execute Log_Analazer.exe
In certain cases code execution might be blocked by Anti-virus SW.
