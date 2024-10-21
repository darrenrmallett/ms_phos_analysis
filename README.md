Analyze and pull-out phosphorylation data using MS Excel files generated by Proteome Discoverer in Nelson et al.:

**DOWNLOAD FROM GITHUB**: download "main" branch. Extract ZIP and rename "Python" folder. Then download "msfiles" and "output" branches. Extract those as ZIP and put them within the "Python" parent folder.

Alternative download:

1) Drag and drop 'python' folder into a directory you want or on the Desktop

2) User should install "Anaconda" if you want to avoid a bunch of errors (https://www.anaconda.com/). This installs python modules that are required to run the software.

    --> alternatively, you can install open-source MiniForge (https://conda-forge.org/).

3) After installing Python and basic libraries through the above sources, user must install additional modules (third party) by typing the following into Terminal and hitting enter:

    --> if pip is not working, you can install it here: https://pip.pypa.io/en/stable/installation/
    
    The following modules are required to run the scripts. Run the following commands in your terminal:

    ```
    pip install regex
    pip install XlsxWriter
    pip install pandas
    pip install requests
    ```
    
    If the script throws an error for a particular library not mentioned above, it is easiest to troubleshoot by typing "pip install" followed by the library in the error message and then re-starting the program.

4) The MS data being analyzed is in the 'msfiles' folder. To analyze your own, add your MS files into 'msfiles' folder within the parent package folder. Note that it is easier to run the script using simple filenames, such as wildtype.xlsx or something.

5) IMPORTANT: Make sure your MS files have the 'Proteins & Peptides' worksheet (tab) as the first tab in the .xlsx file (all the way to the left). This is the table with the expandable/hidden rows. Otherwise the script will not work.

5) Open terminal, and set working directory to the Python directory using the following command:

    ```
    cd directory_path/Python
    ```
    
    For instance, if you put Python folder on desktop, you would type:
    
    ```
    cd Desktop/python
    ```
    
6) To run the phosphorylation analysis, type into Terminal:

    ```
    python phospho.py
    ```
    
    note: sometimes for python3 users, it is ```python3 phospho.py```
    
Follow the commands. When the analysis is done, the 'output' folder contains the comparison file.
    
