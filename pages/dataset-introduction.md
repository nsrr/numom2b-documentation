# Dataset introduction

The [nuMoM2b dataset](:files_path:/datasets) posted on the NSRR has gone through various post-processing steps in order to prepare the data for more widespread sharing. Changes and updates to the source data and variable definitions have been coordinated in the [numom2b-data-dictionary repository](https://github.com/nsrr/numom2b-data-dictionary).

**Disclaimer:** These data are not perfect. Please [submit issues](https://github.com/nsrr/numom2b-data-dictionary/issues) for any new problematic findings.

## Structure of the dataset

The dataset is broken down into five (5) files that correspond to the main SHHS encounters:

1. `shhs1` (Visit 1) -- the baseline clinic visit and polysomnogram performed between 1995 and 1998
  - 5,804 rows, down from the original 6,441 due to data sharing rules on certain cohorts and subjects
2. `shhs-interim-followup` (Interim Follow-up) -- an interim clinic visit or phone call 2-3 years after baseline
  - 5,804 rows, despite some subjects not having complete data, all original subjects are present in the dataset
3. `shhs2` (Visit 2) -- the follow-up clinic visit and polysomnogram performed between 2001 and 2003
  - 4,080 rows, not all cohorts and subjects took part
4. `shhs-cvd` (CVD Outcomes) -- the tracking of adjudicated heart health outcomes (e.g. stroke, heart attack) between baseline and 2008-2011 (varies by parent cohort)
  - 5,802 rows, outcomes data were not provided on all subjects
5. `shhs-cvd-events` (CVD Outcome Events) -- event-level details for the tracking of heart health outcomes
  - 4,839 rows, representing individual events

**Note:** Due to sovereignty issues, Strong Heart Study participants are not included in the shared SHHS data. Data from a total of 5804 participants (1915 ARIC, 1230 CHS, 688 Framingham Offspring and 1971 from other studies) consenting to share data are available.

## Identifiers in the dataset

As part of the de-identification process, all calendar dates were censored from the datasets. These dates have been replaced with a *day offset* type variable that is based upon the `index date`, which for SHHS represents the date of the overnight polysomnography measurement from SHHS Visit 1.

A "cohort" (i.e. data collection site) variable is not available. This variable was censored because it is an identifier.

## Questions?

Please reach out to us at support@sleepdata.org or in the [Forum](https://sleepdata.org/forum) if you have questions.