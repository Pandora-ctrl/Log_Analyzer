# Log_Analyzer
Simple Log Analyzer for IARU HF contest
rev 1.0

# Features
- Up to 2 different logs in Cabrillo format can be analyzed and compared by band and mode.
- The analysis focuses on hourly and 10min QSO rates, hourly point rates, continents and zones.
- 13 different histogram plot formats are generated and saved in png format.
- For each band mode combination a dedicated log file is saved.
- A basic points per QSO calculation is done also resolving continent vs zone ambiguity.

# What this program can not do
- Remove duplicate entries: All dupes are always considered as those contribute to QSO rates.
- Summary result calculation: This is done much better by any dedicated contest logging software.
- Analyze other than IARU HF contests

# How To
- Zone and continent of the respective log should be set before the log is opened. Else QSO points are not calculated correctly.
If zone and continent are changed after opening the log file, the log should be opened again to envoke correct points calculation.
- Log files and diagrams for Log1 are saved in the path of Log1, equivalent for Log2. Comparisions between the logs are stored in the path of Log1.
- In total 240 files are generated, if all analysis options are selected. This takes around 80s.
- Selection of different analysis plots is self explaining

# Installation
Log Analzyer is written in Python 3.13 using vastly the Tkinter, numpy and matplotlib packages. 
It is compiled with Nuitka to run under Windows 10 (64bit), without the need to install Python.

A distribtion package is available for download.
- Step 1: Download Log_Analyzer.Dist.zip and unzip its content.
- Step 2: Download Log_Analyzer.zip and unzip Log_Analyzer.exe.
- Step 3: Move Log_Analyzer.exe in .\Log_Analyzer\Dist\ on the same level with all the python files and sub directories.
        If Log_Analzer.exe is not in the above mentioned folder, DLLs and Python libs will not be found.
- Step 4: Execute Log_Analyler.exe via command shell or double clicking.
