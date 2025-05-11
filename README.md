# Monitoring stress and mental health using Diffusion Models


the dataset is in the form of :
weasad/
├── S2/
│   ├── S2.pkl
│   ├── S2_quest.csv
│   ├── S2_readme.txt
│   ├── S2_respiban.txt
│   └── S2_E4_Data/
│       ├── EDA.csv
│       ├── BVP.csv
│       ├── ACC.csv
│       ├── IBI.csv
│       ├── HR.csv
│       └── tags.csv
├── S3/
│   └── ...
...
└── S17/


it has 12 folders each folder has a 1)pkl file and 

2)quest csv:-

PANAS – Positive and Negative Affect Schedule

STAI – State-Trait Anxiety Inventory

DIM – Could represent dimensional ratings (e.g., pleasure-arousal)

SSSQ – Short Stress State Questionnaire

START / END times – Likely represent timestamps or reaction durations across tasks

ORDER / Base / TSST / Medi 1 / Fun / Medi 2 / sRead / fRead – Possibly different task conditions or phases



3)readme which has 
"### Personal information ###
Age: 27
Height (cm): 175
Weight (kg): 80
Gender: male
Dominant hand: right

### Study pre-requisites ###
Did you drink coffee today? NO
Did you drink coffee within the last hour? NO
Did you do any sports today? NO
Are you a smoker? NO
Did you smoke within the last hour? NO
Do you feel ill today? NO

### Additional notes ###
The RespiBAN temperature sensor was not fully attached throughout the entire duration of the study protocol.


4)respibhan txt which has "# OpenSignals Text File Format
# {"00:07:80:D8:AB:58": {"sensor": ["ECG", "EDA", "EMG", "TEMP", "XYZ", "XYZ", "XYZ", "RESPIRATION"], "device name": "RespiBan", "column": ["nSeq", "DI", "CH1", "CH2", "CH3", "CH4", "CH5", "CH6", "CH7", "CH8"], "sync interval": 2, "time": "9:39:1.0", "comments": "", "device connection": "BTH00:07:80:D8:AB:58", "channels": [1, 2, 3, 4, 5, 6, 7, 8], "date": "2017-5-22", "mode": 0, "digital IO": [0, 1], "firmware version": 770, "device": "biosignalsplux", "position": 0, "sampling rate": 700, "label": ["CH1", "CH2", "CH3", "CH4", "CH5", "CH6", "CH7", "CH8"], "resolution": [16, 16, 16, 16, 16, 16, 16, 16], "special": [{}, {}, {}, {}, {}, {}, {}, {}]}}
# EndOfHeader"  


5)e4_data :-which has "
TEMP.csv
Data from temperature sensor expressed degrees on the Celsius (°C) scale.

EDA.csv
Data from the electrodermal activity sensor expressed as microsiemens (μS).

BVP.csv
Data from photoplethysmograph.

ACC.csv
Data from 3-axis accelerometer sensor. The accelerometer is configured to measure acceleration in the range [-2g, 2g]. Therefore the unit in this file is 1/64g.
Data from x, y, and z axis are respectively in first, second, and third column.

IBI.csv
Time between individuals heart beats extracted from the BVP signal.
No sample rate is needed for this file.
The first column is the time (respect to the initial time) of the detected inter-beat interval expressed in seconds (s).
The second column is the duration in seconds (s) of the detected inter-beat interval (i.e., the distance in seconds from the previous beat).

HR.csv
Average heart rate extracted from the BVP signal.The first row is the initial time of the session expressed as unix timestamp in UTC.
The second row is the sample rate expressed in Hz.


tags.csv
Event mark times.
Each row corresponds to a physical button press on the device; the same time as the status LED is first illuminated.
The time is expressed as a unix timestamp in UTC and it is synchronized with initial time of the session indicated in the related data files from the corresponding session.

"

