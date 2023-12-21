##  Behavior Of Customers Using Television Service Analysis

**Project description:** 

This project is to analyze the behavior of service usage characteristics of users who have canceled their contracts for television services and suggest recommendations.

### 1. Dataset

[Data](https://github.com/thaihiendo190699/thaihiendo190699.github.io/blob/main/DataSampleTest.zip)

This dataset is in log. I have used Python to parse them into pandas data frame by the following code script:

"#Folder path to log files

folder_path = r'C:\Users\ASUS\Desktop\FPT test\DataSampleTest'

"# Find all file txt in the folder

file_pattern = folder_path + '/log*.txt'
file_list = glob.glob(file_pattern)

"# List to store DataFrame from each file

data_frames = []

"# Read each file and convert to DataFrame

for file_name in file_list:
    data_dicts = []
    with open(file_name, 'r') as file:
        lines = file.readlines()
        for line in lines:
            if line.strip():
                data_dict = eval(line)
                data_dicts.append(data_dict)
    df = pd.DataFrame(data_dicts)
    data_frames.append(df)

"# Concat them to 1 dataframe

data = pd.concat(data_frames, ignore_index=True)"

### 2. Dashboard

<img src="https://github.com/thaihiendo190699/thaihiendo190699.github.io/blob/main/FPT-1.png?raw=true"/>

<img src="https://github.com/thaihiendo190699/thaihiendo190699.github.io/blob/main/FPT-2.png?raw=true"/>

<img src="https://github.com/thaihiendo190699/thaihiendo190699.github.io/blob/main/FPT-8.png?raw=true"/>

<img src="https://github.com/thaihiendo190699/thaihiendo190699.github.io/blob/main/FPT-4.png?raw=true"/>

<img src="https://github.com/thaihiendo190699/thaihiendo190699.github.io/blob/main/FPT-5.png?raw=true"/>

<img src="https://github.com/thaihiendo190699/thaihiendo190699.github.io/blob/main/FPT-6.png?raw=true"/>

