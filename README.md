# Summer of Haskell proposals

This repository collects ideas that will be submitted to the Google Summer of Code 2018 via Haskell.org.

Both prospective students and mentors are encouraged to discuss new proposals with the rest of the DataHaskell community at https://gitter.im/dataHaskell/Lobby .

The project ideas will be submitted first to Haskell.org (via https://summer.haskell.org/ideas.html , https://github.com/haskell-org/summer-of-haskell ) and ultimately to Google. ()

All student must apply between March 12 and March 27, 2018 (see the timeline : https://summerofcode.withgoogle.com/how-it-works/#timeline).

The current list of DataHaskell-related GSoC project proposals are listed in the following.




## Ergonomic dataframe API

### Abstract

This project aims at creating a comfortable API (e.g. an embedded domain-specific language) for dataframe manipulation (think `dplyr`, but type-safe). The aim is to lower the entry barrier for both data science practitioners and Haskell newcomers. 

### Description

| **Intensity** | **Priority** | **Involves**  | **Mentors** |
| ------------- | -----------| ------------- | ----------- |
| Moderate      | Medium     | Haskell       | [Marco Zocca](mailto:zocca.marco gmail) |



## Extending `Frames` with new storage formats

### Abstract

Currently the `Frames` library only supports CSV, but it would be very useful to interface it with other storage formats, e.g. SQL, HDF5, etc.
The project will likely involve interfacing two or more pre-existing libraries (e.g. `Frames`, `postgresql-simple`, `pipes` ..), so an intermediate level of Haskell proficiency would be beneficial.

### Description

| **Intensity** | **Priority**  | **Involves**  | **Mentors** |
| ------------- | -----------| ------------- | ----------- |
| Moderate      | Medium     | Haskell, C    | [Marco Zocca](mailto:zocca.marco gmail) |