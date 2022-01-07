<link rel="icon" type="image/x-icon" href="knowdive_logo" />

# Dataset Description
This section should highlight the main features of the datasets and list the sources of data, that will be detailed in the subparagraphs. Usually the sources of data are (i) Online questionnaire (synchronic); (ii) ESM/EMA (diachronic); Sensor data (diachronic).

## Participants
This section describes the main characteristics of the participants: how many they are, their demographics (e.g. gender, age, occupation, ...), and the average of the observations collected (from ESM/EMA and/or sensor data).

E.g.: The dataset contains XX participants, XX are Female and XX are Male. Additional information are listed below.

|  | Range | Average |
|-------|--------|---------|
**Age** | 20-26 | 22 |
**N. obs.** | 396-932 | 700 |


## Online questionnaires 
This section should briefly describe the questionnaire used, the languages in which it was administered and its sections. If standardized measuring instruments or already tested scales have been used (e.g. Big Five for personality traits), these must be presented here together with the link to the reference article. E.g .:
- personality, collected with a 10-item short version of the [Big Five](https://pdfs.semanticscholar.org/4646/5a97ab883cc72d9f601263a208afae6fb31a.pdf) Inventory-44
This section concludes with a link to the complete questionnaire and the codebook, in the formatted version and in English.


## ESM/EMA
This section should describe the ESM / EMA tools, the languages in which it was administered and its sections. If standardized measuring instruments or already tested scales have been used (e.g., HETUS) and apps for data colletion (e.g., iLog), these must be presented here together with the link to the reference article.
In addition, all stimuli used and the timing with which they were administered should be presented (possibly in a table).
This section concludes with a link to the codebook.

## Sensor Data
This section should describe the Sensor data collected, namely their tipology, timing, number of observation, and description. Below is an example of a complete description.

The data from the sensors can be divided into: 
-	Hardware (HW) sensors, namely the sensors that one can find in a phone, e.g., accelerometer, gyroscope, GPS. The complete list of HW sensors used in this survey is reported in Table 1 
-	Software (SW) sensors, by which we mean all the SW events that can be collected from the Operating system and SW, for instance the Wifi the HW is connected and so on. The complete list of SW sensors is reported in Table 2
-	QU sensors (where QU stands for Questionnaire), by which we mean events which relate to the compilation of the Time Use Diary, mainly related to the various execution times, e.g., when a question arrived or was answered. The complete list of QU sensors is reported in Table 3

The complete documentation can be found [here]().


No | HW Sensor | Estimated Frequency |  N.Obs. | Description |
|-------|--------|---------|---------|---------|
1 | Accelerometer | up to 20 samples per second | ... | measures the acceleration to which the phone is subjected and it captures it as a 3D vector |
2 | Gyroscope | up to 20 samples per second | ... | measures the rotational forces to which the phone is subjected and it captures it as a 3D vector |
3 | Linear Acceleration | up to 20 samples per second | ... | measures the acceleration force to which the phone is subjected and it captures it as a 3D vector |
4 | Location | Once every minute | Small | returns the geocoordinates of where the phone is located, for more accuracy this sensor combines GPS and WIFI/cellular connections |
5 | Magnetic Field | up to 20 samples per second | ... | measures the magnetic field to which the phone is subjected and it captures it as a 3D vector |
6 | Pressure | up to 20 samples per second | ... | measures the ambient air pressure to which the phone is subjected |

*Table 1. HW sensors.*

No | SW Sensor | Estimated Frequency | N.Obs. | Description |
|-------|--------|---------|---------|---------|
7  | Activity Performed (Google Data)                   | Once every minute     | ... | returns a label identifying the activity performed by the user. This value is computed by Android using Google's Activity Recognition API along with low power signals from multiple sensors in the device. Possible activities are: _still, in\_vehicle, on\_bicycle, on\_foot, running, tilting, walking_ |
8  | Audio from the internal microphone                 | 10 seconds per minute | ... | Audio from the internal microphone |
9  | Audio mode (Silent/Normal)                     | On change             | ... | Audio from the internal microphone |
10 | Battery Charge (ON/OFF)                        | On change             | ... | returns whether the phone is currently charging its battery |
11 | Battery Level                                      | On change             | ... | returns the phone's battery level |
12 | Cellular network info                              | Once every minute     | ... | returns information related to the cellular network (cellid, dbm, type) to which the phone is connected to |
13 | Doze Modality (ON/OFF)                         | On change             | ... | returns whether the phone's doze mode is on or off. Doze mode is a low battery consumption state in which the phone enters after some time of not being used |
14 | Flight Mode (ON/OFF)                           | On change             | ... | returns whether the phone's Airplane mode is on or off, Airplane mode turns off all the connectivity features of the phone |
15 | Gravity                                            | 20 times per second   | ... | report the force of gravity on the axis |
16 | Headset plugged in (ON/OFF)                    | On change             | ... | returns whether the headphones of the phone where connected |
17 | Humidity                                           | 20 times per second   | ... | return ambient relative humidity.
18 | Music Playback (no track information) (ON/OFF) | On change             | ... | eturns whether music is being played on the phone (yes or no) using the default music player from the operating system |
19 | Notifications received                             | On change             | ... | measures when the phone receives a notification and when it is dismissed by the user |
20 | Orientation                                        | 20 times per second   | ... | return the azimuth, pintch and roll.
21 | Proximity                                          | On change             | ... | measures the distance between the user's head and the phone, depending on the phone it may be measured in centimeters (i.e., the absolute distance) or as labels (e.g, 'near', 'far') |
22 | Rotation Vector                                    | 20 times per second   | ... | return the rotation vector component along the axis
23 | Running Application                                | Once every 5 seconds  | ... | returns the name of the application (or application package) that is currently running in the foreground of the phone |
24 | Screen Status (ON/OFF)                         | On change             | ... | returns whether the phone's screen is on or off |
25 | Temperature                                        | 20 times per second   | ... | return the ambient air temperature.
26 | Touch event                                        | On change             | ... | generates a touch value each time the user touches the screen |
27 | WIFI Network Connected to                          | On change             | ... | returns information related to the WiFi network to which the phone is connected to, if connected will also report the WiFi network id |
28 | WIFI Networks Available                            | Once every minute     | ... | returns all WiFi networks detected by the smartphone |

*Table 2. SW sensors.*

No | QU Sensor | Estimated Frequency | N.Obs. | Description |
|-------|--------|---------|---------|---------|
29 | Time Diary questions | On change | ...| contains the question, the question id (for traceability purposes) and the timestamp when it was generated on the server and sent to the cloud provider for delivery |
30 | Time Diary confirmation | On change | ...| contains the timestamp at which each question, identified by its unique id, has been delivered to the device of the participant (which may coincide or not with the time the participant sees it) |
31 | Time Diary answers | On change | ...| contains the answer, the timestamp when it was saved in the server, and the difference between answer and notification times in milliseconds |
32 | Task questions | On change | ...| contains the question and the timestamp when it was sent from the server |
33 | Task confirmation | On change | ...| contains the timestamp when each specific question was notified to the participant |
34 | Task answers | On change | ...| contains the answer, the timestamp when it was saved in the server, and the difference between answer and notification times in milliseconds |

*Table 3. Questionnaire sensors.*

In these three sensor tables, the frequency by which the sensors are captured is reported, according to the following conventions: _on change_ means that the value of the sensor is recorded only when the current value is changed (along with a timestamp of when it happened), _up to X samples per second_ means that for each second the value of the sensor will be stored up to maximum of X times (these values are estimated), and _once every Y_ means that the values of a sensor is recorded once the time Y has passed (these values are estimated).


# Data collection
This section should describe the different phases of the data collection protocol and highlight the main features of the data collection process. Usually its divided into three subsections. E.g.:

The data collection was conducted in an interdisciplinary framework, involving sociology and IT experts. The survey methodology adopted is a variant of the ESM. In our case, in addition to the self-reported question, data from the smartphone sensors were collected through an app called [iLog](http://datascientia.disi.unitn.it/ilog/).

## Timing
The overall data collection process last for XX weeks. The first two weeks were dedicated to sample recruitment by sending the first two questionnaires XXX. The remaining month was entirely dedicated to ESM through iLog, separated into two parts: during the first part XX, while for the second XX. Participants can/cannot interrupt ESM during the data collection

## Sample recruitment
The sample was selected XX. All students were sent an invitation to participate in the survey, excluding a priori those who did not have a smartphone compatible with the study (only Android Operating System greater than 6.0) and XX. After the first contact via email/face to face/..., the online questionnaire was sent to investigate their XX, and finally it was sent a password to download and install the app iLog. 

Additional requirements or constrains for the sample selection (e.g. randomization, number, age,...) are described here.

## Incentive strategy
Particpants received XX€ payments, ...

# Example of application
This section should list all the scientific article, workshop, and projects in which the datasets was used (therefore it should be updated periodically). Each reference must have an url link.
### Scientific Article
### Workshops
### Projects

# Contact

Do you want to acess our dataset? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) and contact us at [datadistribution.knowdive@unitn.it](datadistribution.knowdive@unitn.it).
