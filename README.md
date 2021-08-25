# ams_database
Database for uploading and sharing spectra data from samples taken using Thermo Fisher Scientific Compound Discoverer software

### Running the code (local machine)
#### Using Git Bash:

1. To run the code in a virtual environment and have it on your local machine, you will need Git Bash which you can download here: https://git-scm.com/downloads

2. Open your Git Bash terminal and change into directory holding flask files e.g. `cd /c/my_flask`

3.	Create a virtual environment e.g. `python -m venv virtual`

4.	Turn on virtual environment e.g. `source virtual/Scripts/activate`

5. Install flask and openpyxl packages e.g. `pip install flask` and `pip install openpyxl`

6.	Run code e.g. `flask run`

### Notes

#### SQL Database
A SQL database table needs to be created before running the code and should contain the same number of columns as found in the Thermo Fisher Scientific Compound Discoverer exported excel file as well as the same order. The code written will not create a table for you. However note that the column names in the SQL database table do not necessarily need to match the ones in the exported excel file exactly e.g. Fragment header in excel file can be called Fragment 1 in SQL table, what matters is that the order and number of columns is the same between SQL table and excel file.


#### Import feature
The webpage's .xlsx import feature only works if the SQL database contains all the same number of columns, there does not need be an exact match in names but this means you need to be careful with ordering.


#### Excel Column Headers
The column headers in the excel file are as follows:
* CompoundName
* ExperimentType
* Compound Type
* ChemicalFormula
* Category
* CAS
* Ionization
* ResponseThreshold
* Internal Standard
* Internal Standard Concentration
* PrecursorMass
* ExtractedMass
* Adduct
* Polarity
* ChargeState
* RT
* Window
* CollisionEnergy
* Lens
* EnergyRamp
* Confirm Precursor
* Confirm Extracted
* Confirm Energy
* Target Ratio
* Window Type
* Ratio Window
* Ion Coelution
* Confirm Precursor
* Confirm Extracted
* Confirm Energy
* Target Ratio
* Window Type
* Ratio Window
* Ion Coelution
* Confirm Precursor
* Confirm Extracted
* Confirm Energy
* Target Ratio
* Window Type
* Ratio Window
* Ion Coelution
* Confirm Precursor
* Confirm Extracted
* Confirm Energy
* Target Ratio
* Window Type
* Ratio Window
* Ion Coelution
* Confirm Precursor
* Confirm Extracted
* Confirm Energy
* Target Ratio
* Window Type
* Ratio Window
* Ion Coelution
* Fragment
* Fragment
* Fragment
* Fragment
* Fragment
