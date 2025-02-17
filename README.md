# Artificial Dust Prediction Dataset

## Table of Contents

- [Overview](#overview)
- [Features](a#features)
- [Data Generation Methodology](#data-generation-methodology)
- [Use Case](#use-case)
- [Example Data](#example-data)
- [License](#license)
- [References](#references)
- [Contact](#contact)

## Overview

This dataset contains artificially generated environmental data designed for predicting dust levels based on various factors such as wind speed, voltage, and climate conditions. It was created to address the lack of publicly available datasets with specific dust values.

## Features

The dataset includes the following columns:

| Column Name        | Description                                            |
| ------------------ | ------------------------------------------------------ |
| City               | Name of the city.                                      |
| State              | State where the city is located.                       |
| Climate Condition  | General climate condition (e.g., Dry, Mild, Humid).    |
| Type of Location   | Type of location (e.g., Urban, Coastal, Desert).       |
| Day                | Day of the observation.                                |
| Month              | Month of the observation.                              |
| Year               | Year of the observation.                               |
| Hour               | Hour of the observation.                               |
| Wind Speed (knots) | Wind speed in knots.                                   |
| Voltage            | Simulated sensor output voltage (0–12V).               |
| Dust Value         | Simulated dust concentration (normalized score, 1–10). |

## Data Generation Methodology

- The dataset was artificially generated using domain knowledge and tools like ChatGPT.
- The **Dust Value** column represents normalized dust concentrations ranging from 1 to 10.
- The **Voltage** column is derived from the dust values using a linear relationship:

Voltage = Dust Value \* 1.2

## Use Case

This dataset can be used to train machine learning models for predicting dust levels based on environmental conditions.

## License

This dataset is licensed under [CC0: Public Domain](https://creativecommons.org/publicdomain/zero/1.0/), meaning it is free to use, modify, and distribute without restriction.

## References

- Inspired by real-world datasets such as the [Air Quality Dataset by UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/360/air+quality).
