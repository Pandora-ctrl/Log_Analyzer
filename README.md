# Log_Analyzer
Simple Log Analyzer for IARU HF contest
rev 1.0, by OE8TED

Two different Cabrillo logs can be opened, analyzed and compared.
Analysis focuses on hourly and 10min QSO rates, worked zones, continents and points.
A basic points per QSO calculation resolves zones over multiple continents.
Zone and continent of the respective log should be set before the log is opened. Else QSO points are not calculated correctly.
If zone and continent are changed after opening the log file, the log should be opened again to envoke correct points calculation.
png diagrams of each analysis are saved as well as logs per band and mode.
Log files and diagrams for Log1 are saved in the path of Log1, equivalent for Log2. Comparisions between the logs are stored in the path of Log1.
In total 240 files are written, if all analysis options are selected. This can take more than 70s.
What this program can not do:
- Remove duplicate entries: All dupes are always considered as those contribute to QSO rates.
- Any result calculation: This is done much better by any dedicated contest logging software.
- Analyze other than IARU HF contests

Log Analzyer is written in Python 3.13 and compiled with Nuitka to run under Windows 10 (64bit).
A distribtion package is available for download.
Step 1: Download Log_Analyzer.Dist.zip and unzip the content.
Step 2: Download Log_Analyzer.zip and unzip Log_Analyzer.exe.
Step 3: Move Log_Analyzer.exe in .\Log_Analyzer\Dist\
Step 4: Execute Log_Analyler.exe. If Log_Analzer.exe is not in the above mentioned folder, DLLs and Python libs will not be found.
In certain cases code execution needs to permitted for Anti-virus SW.
