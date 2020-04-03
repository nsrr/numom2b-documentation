# Polysomnography introduction

Data collection for PSG was standardized among various manufactured instruments by use of standardized collection and display montages. Each unit used for collection was certified before use to maximize signal quality integrity throughout the EDF conversion and import into Compumedics Profusion software used for scoring.

Notes:

- [Montage and Sampling Rate Information](:pages_path:/montage-and-sampling-rate-information.md)
- [Sleep Breathing Substudy Manual of Operations](:files_path:/documentation/nuMoM2b-SBS-MOO.pdf)

## Signal and annotation files

[Raw polysomnography data](:files_path:/polysomnography) are available for 3,009 subjects at Visit 1 and 2,332 subjects at Visit 3. Each recording has a signal file (.EDF) and two versions of the event scoring and epoch staging annotations (.XML).

1. **[EDF](:files_path:/polysomnography/edfs)** - Signal files in the [European Data Format](http://www.edfplus.info/) exported from Compumedics Profusion and processed in [Luna](http://zzz.bwh.harvard.edu/luna/)
2. **[XML (Profusion)](:files_path:/polysomnography/annotations-events-profusion)** - Annotation files exported from Compumedics Profusion. ([Learn more...](https://github.com/nsrr/edf-editor-translator/wiki/Compumedics-Annotation-Format))

## Known issues

- Annotation file event counts may not always directly match the [core datasets](:files_path:/datasets). SHHS data are more than 15 years old and there may have been conversion issues in a limited number of cases.
- Oxygen desaturation events from the annotation files may be absent and/or may not line up as anticipated with respiratory events. Original scoring data were indelibly changed when converting to a newer version of the scoring software that allowed for the creation of EDF/XML files. Users may opt to derive new desaturation events from the SaO2 signal.

## History / changelog

*April 2020*
- Polysomnography data uploaded to sleepdata.org after exports from Compumedics Profusion

## Questions?

Please reach out to us at support@sleepdata.org or in the [Forum](https://sleepdata.org/forum) if you have questions.
