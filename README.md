# Smoke-Detection-for-Fire-Safety-Alram
Smoke Detection for Fire Safety Alarm A machine learning-based project focused on detecting smoke patterns to trigger early fire safety alarms. Utilized data preprocessing, feature engineering, and classification models to accurately identify smoke presence for timely alerts in critical environments.

# Context
A smoke detector is a device that senses smoke, typically as an indicator of fire. Smoke detectors are usually housed in plastic enclosures, typically shaped like a disk about 150 millimetres (6 in) in diameter and 25 millimetres (1 in) thick, but shape and size vary.

## Types of Smoke Detectors

### Photoelectric Smoke Detector

A photoelectric smoke detector contains a source of infrared, visible, or ultraviolet light, a lens, and a photoelectric receiver. In some types, the light emitted by the light source passes through the air being tested and reaches the photosensor. The received light intensity will be reduced due to scattering from particles of smoke, air-borne dust, or other substances; the circuitry detects the light intensity and generates an alarm if it is below a specified threshold, potentially due to smoke. Such detectors are also known as optical detectors.

### Ionization Smoke Detector

An ionization smoke detector uses a radioisotope to ionize air. If any smoke particles enter the open chamber, some of the ions will attach to the particles and not be available to carry the current in that chamber. An electronic circuit detects that a current difference has developed between the open and sealed chambers, and sounds the alarm

# About the dataset
Collection of training data is performed with the help of IOT devices since the goal is to develop a AI based smoke detector device.
Many different environments and fire sources have to be sampled to ensure a good dataset for training. A short list of different scenarios which are captured:


Normal indoor

Normal outdoor

Indoor wood fire, firefighter training area

Indoor gas fire, firefighter training area

Outdoor wood, coal, and gas grill

Outdoor high humidity

etc.

The dataset is nearly 60.000 readings long. The sample rate is 1Hz for all sensors. To keep track of the data, a UTC timestamp is added to every sensor reading.

index

UTC  :
Timestamp UTC seconds

Temperature[C] :
Air Temperature

Humidity[%] :
Air Humidity

TVOC[ppb] :
otal Volatile Organic Compounds; measured in parts per billion

eCO2[ppm] :
co2 equivalent concentration; calculated from different values like TVCO

Raw H2 :
raw molecular hydrogen; not compensated (Bias, temperature, etc.)

Raw Ethanol :
raw ethanol gas

Pressure[hPa] :
Air Pressure

PM1.0 :
particulate matter size < 1.0 µm (PM1.0). 1.0 µm < 2.5 µm (PM2.5)

PM2.5 :
particulate matter size < 1.0 µm (PM1.0). 1.0 µm < 2.5 µm (PM2.5)

NC0.5 :
Number concentration of particulate matter. This differs from PM because NC gives the actual number of particles in the air. The raw NC is also classified by the particle size: < 0.5 µm (NC0.5); 0.5 µm < 1.0 µm (NC1.0); 1.0 µm < 2.5 µm (NC2.5);

NC1.0 :
Number concentration of particulate matter. This differs from PM because NC gives the actual number of particles in the air. The raw NC is also classified by the particle size: < 0.5 µm (NC0.5); 0.5 µm < 1.0 µm (NC1.0); 1.0 µm < 2.5 µm (NC2.5);

NC2.5 :
Number concentration of particulate matter. This differs from PM because NC gives the actual number of particles in the air. The raw NC is also classified by the particle size: < 0.5 µm (NC0.5); 0.5 µm < 1.0 µm (NC1.0); 1.0 µm < 2.5 µm (NC2.5);


CNT :
Sample counter


### Applied data preprocessing, feature engineering, and exploratory data analysis. Trained and evaluated multiple classification models including Random Forest (RF), Support Vector Classifier (SVC), Decision Tree (DT), and Logistic Regression (LR), with Decision Tree selected as the final model for its best performance.

Fire Alarm :
ground truth is "1" if a fire is there
