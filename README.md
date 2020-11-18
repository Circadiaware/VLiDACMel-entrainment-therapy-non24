# non24article
Work-in-progress draft of a protocol to entrain the Non 24 circadian rhythm disorder.

## VLiDACMel entrainment therapy protocol

The goal is to define a therapy that can reliable entrain the circadian rhythm of (sighted) individuals with non-24 circadian rhythm disorder, using a combination of 2 insights:

1. New therapies based on the careful manipulation and combination of zeitgebers, such as light therapy, melatonin and food timing, can allow for better results. It is hence necessary to determine what is the minimal set of zeitgebers for effective long-term entrainment and what parameters and conditions affect their effeciency on the circadian rhythm.

2. Self-monitoring of the circadian rhythm is necessary to optimally time the therapies on a day-to-day basis and achieve stable therapeutic benefits, as is the case for other chronic diseases such as diabetes where glucose monitoring is necessary. Similarly, circadian rhythm monitoring is a necessity.

The latest working therapy protocol, which worked for 2.5 months and reproduced for 4 months (still ongoing) at the time of this writing, is named **VLiDACMel**, which stands for:

* **V**ery long **Li**ght therapy at wake-up (after minimal core body temperature),
* **D**ark therapy in the evening,
* **A**void **C**arbs and **Mel**atonin mixup,
* and take exogenous instant-release **Mel**atonin timed before DLMO (measured via core body temperature or approximated via 3 days average of wake-up times).

This protocol, along with data of the author's sleep patterns with a > 1y annotated sleep diary, are available in this repository.

To read the draft of the VLiDACMel protocol, use this HTML previewer: https://lrq3000.github.io/non24article/SleepNon24VLiDACMel.html

If you reuse some of my material, please feel free to use it under Creative Commons v4 with attribution ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed)).

I am also open to collaborations (eg, to design a group study on healthy volunteers and/or patients with sighted non-24).

A (messy) side notebook with lots of references along with an older draft protocol (based on chronotherapy and melatonin - which did not work) is available here: To view the draft, use this HTML previewer: https://lrq3000.github.io/non24article/other_docs/SleepNon24.html

## Vitals dataset

In order to both better characterize the non-24 circadian rhythm disorder's phenomenology without intervention, and the effect of the VLiDACMel intervention (and maybe of other interventions) in an objective fashion, the author is developing a set of software tools and self-monitoring wearable devices to monitor the circadian rhythm disorder.

All the vital datasets under the `analysis/` folder are published under Creative Commons v4 with attribution (CC BY 4.0). Please feel free to use the dataset for any research prupose, without requiring to notify the author beforehand (although that would be appreciated). The author only asks that the dataset is not used to degrade the author's dignity.

More datasets will be published in the future (need to find a server to store opensourced big data - please let me know if you have a suggestion!), but for now the complete manually maintained sleep diary in CSV format as generated by the Sleepmeter app is available. This dataset is complete and reliable, consider it the most reliable dataset of all vitals, as it is manually and rigorously curated, so that there is no missing sleep session. For example, there are sometimes wide gaps between two sleep sessions, more than 24h: these are not missing information, they are all-nighters (or even longer sleep deprivation periods). On the other hand, the vitals have missing periods as it's necessary to have washout periods where the wearables are not worn, otherwise they cause skin damage if worn for longer than 1 week, and it's not uncommon that I unconsciously detach them during sleep sessions due to the very inconvenient itchiness. I am investigating ways to reduce this issue and increase the continuous wear time, but there is likely no ideal solution, the wearables have to be worn off regularly for some period of time. Some wearables also have missing data periods between the acquisition periods, as it is necessary to stop the recording to download the data before restarting the next, and it takes some time to both download the data and recharge the device's battery. For all these reasons, the manually curated sleep diary should be considered the most reliable dataset with no missing sleep period, so please use the sleep diary as a reference and stack onto it the other vitals.

The planned toolset (work-in-progress for now) will include:
* 130Hz ECG and 100Hz 4g 3-axis trunk actigraphy using Polar H10.
* 1Hz core body temperature from the trunk using dual-heat-flux method.
* 5min skin temperature using Thermocron iButtons, body sites to be defined.
* 100Hz 4g 6-axis wrist actigraphy using Axivity AX6.
* 1Hz light intensity and color spectrometer sensor using a custom DIY Arduino-based system.
* an improved mobile software to replace Sleepmeter to manually curate a sleep diary with more event types (ie, not only the sleep sessions will be recorded, but also the precise time of any periodical event such as meal times, therapies timing, etc. - this will improve our ability to statistically test the influence of various time-sensitive factors).
