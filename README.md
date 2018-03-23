# Summer of Haskell proposals

This repository collects ideas that will be submitted to the Google Summer of Code 2018 via Haskell.org.

Both prospective students and mentors are encouraged to discuss new proposals with the rest of the DataHaskell community at https://gitter.im/dataHaskell/Lobby .

The project ideas will be submitted first to Haskell.org (via https://summer.haskell.org/ideas.html , https://github.com/haskell-org/summer-of-haskell ) and ultimately to Google. 

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

## Expand json-autotype support to other functional programming languages

[json-autotype](http://github.com/mgajda/json-autotype) is currently the *most advanced* type and parser generator from JSON to Haskell. Using union types it works as most accurate type providers.

It was of great outside interest to enhance it to produce types and parsers for other strongly-typed programming languages like Elm, PureScript, Scala, Elixir, F#, or Java.
This project is of great practical importance, and will allow us to pitch Haskell as practical language to other strongly-typed language communities..

### Description

| **Intensity** | **Priority** | **Involves**  | **Mentors** |
| ------------- | -----------| ------------- | ----------- |
| Light         | High       | Haskell, Elm, PureScript, Scala, Elixir | [Michal Gajda](mailto:migamake migamake.com) |

## Expand json-autotype to directly query whole Web APIs, and create Servant endpoints

[json-autotype](http://github.com/mgajda/json-autotype) is currently the *most advanced* type and parser generator from JSON to Haskell.
However most programmers are not using JSON just to read and write it, but to interact with Web APIs. One would dream about generating the whole WebAPI types, and either client calls, and server endpoints just from Swagger descriptions, or a bunch of queries to the WebAPIs.

Implementing this project would put Haskell as possibly the best language to interact with WebAPIs in typed way. It would also make it superior to pure GraphQL solutions which are state-of-art now.

### Description

| **Intensity** | **Priority** | **Involves**  | **Mentors** |
| ------------- | -----------| ------------- | ----------- |
| Difficult     | High       | Haskell, Servant or Apiary | [Michal Gajda](mailto:migamake migamake.com) |

## Automatic finding of Data Science libraries for the project

As our package database ([Hackage](https://hackage.haskell.org)) grows, we get more and more data formats that can be easily parsed by our code. But it is increasingly difficult to find relevant parsers, and check whether they support given file format out-of-the-box.

Data Scientist interested in quick-and-dirty analyses need to either:
* spend some time just on parser and library discover for new formats,
* limit themselves to projects that only use formats they know well (like `.csv`),
* fall back to inefficient process using dynamically typed languages like Python and Octave.

It would be great to use Stackage and Hackage to establish a database of supported formats,
along with demonstration code that reads given file type.
First we can build the tool that automatically recognizes types and tries to parse them with the standard libraries, then we put it onto the web service, that takes data directory, and gives Haskell program that parses all the data inside.

### Description

| **Intensity** | **Priority** | **Involves**  | **Mentors** |
| ------------- | -----------| ------------- | ----------- |
| Moderate      | Medium       | Haskell | [Michal Gajda](mailto:migamake migamake.com) |

