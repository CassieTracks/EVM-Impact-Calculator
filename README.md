
## Earned Value Management Impact Calculator
### Introduction
This tool allows users to analyze changes in cost profiles and item attributes to understand their impact on EVM metrics. It provides visualizations to aid project cost and schedule tracking.

### Setup Instructions
Ensure you have Python installed (recommended: Python 3.8+)

### Dependencies
- streamlit
- pandas
- ploty
- reportlab
- kaleido (Note on Windows must use kaleido version 0.1.0post1 for it to work with streamlit)

### Running the App
#### Installation
    use pip to install the required third party packages: pip -r requirements.txt

#### Usage
 
    From a IDE you can just run the relevant .py file. If you don’t have a IDE, open a terminal,cd to the appropriate folder and type in python <.py file>

    main.py: run it in the project root folder, so it can import from the testpack folder


Launch the app locally:
    > streamlit run main.py
or use the following command replacing the folder location to where the repository is stored:
    > streamlit run "[folder location]/main.py"  
Navigate to localhost:8501

### Usage Guide
- Upload Cost Data: Upload a CSV or Excel file with columns: Date, Cost, Item Number, and Type.
- Upload Attribute Data: Upload a file with columns: Item Number, Cost, Lead Time, Yield, and Hours.
- Interactive Sliders: Adjust the parameters for Cost, Lead Time, Yield, and Hours in the sidebar.
- Visualizations: View cumulative line and bubble charts showing cost profiles before and after adjustments.
- Export Charts: Download a PDF summarizing the analysis with the "Export and Download PDF" button.

### Caveats
- Ensure the dataset matches the required schema; missing columns will generate an error.
- The app assumes all data is in a consistent format.
