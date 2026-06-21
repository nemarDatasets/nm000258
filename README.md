# Imagined Speech EEG database — Spanish vowels and commands (Pressel et al. 2016)

## Overview

An open-access EEG dataset comprising recordings from 15 healthy Spanish-speaking subjects during imagined speech tasks. The dataset includes 11 imagery classes: 5 Spanish vowels and 6 directional commands, acquired using 6-channel EEG at 1024 Hz with preprocessed data (bandpass filtered 2-45 Hz). Trials consist of 4-second periods with a 3-second imagery window occurring within each trial. This resource supports brain-computer interface research and motor imagery classification studies.

## Dataset Summary

| Property | Value |
|---|---|
| Subjects | 15 |
| Channels | 6 |
| Classes | 11 |
| Trial length | 4 s |
| Sampling frequency | 1024 Hz |
| Sessions | 1 |
| Total trials | 8670 |
| Paradigm | MotorImagery |

## Data Collection Methods

EEG signals were recorded from 15 healthy subjects (age 24-28 years) using a Grass 8-18-36 amplifier with DataTranslation DT9816 ADC. Six channels (F3, F4, C3, C4, P3, P4) were positioned according to the standard 10-20 montage. Sampling rate was 1024 Hz with online bandpass filtering (2-45 Hz). Subjects performed cue-based imagery tasks of 5 Spanish vowels and 6 directional commands in response to visual stimuli, with trial duration of 4 seconds and imagery period of 3 seconds. Data were preprocessed with bandpass filtering and artifact rejection applied.

## How to Access via MOABB

Install MOABB and load this dataset directly:

```python
from moabb.datasets import Pressel2016
from moabb.paradigms import MotorImagery
paradigm = MotorImagery()

dataset = Pressel2016()
X, y, metadata = paradigm.get_data(dataset)
```

For more details see the [MOABB documentation](https://moabb.neurotechx.com/) and the
[MOABB dataset page](https://moabb.neurotechx.com/docs/generated/moabb.datasets.Pressel2016.html).

## Citation

If you use this dataset please cite the primary publication:

> DOI: [10.1117/12.2255697](https://doi.org/10.1117/12.2255697)

## NEMAR / MOABB Benchmark Collection

This BIDS-formatted dataset was converted from the original data using the
[MOABB](https://moabb.neurotechx.com/) pipeline and re-hosted on
[NEMAR](https://nemar.org/) as part of the MOABB benchmark collection.
The original data and license terms apply — see `dataset_description.json` for details.
