[![Funding](https://img.shields.io/static/v1?label=powered+by&message=LIFE+RIPARIAS&labelColor=323232&color=00a58d)](https://www.riparias.be/)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-blue.svg)](https://creativecommons.org/licenses/by/4.0/)

# manIAS
Development of a community driven data exchange format for sharing data about the management of Invasive Alien Species (IAS) and wildlife.

## Proposed table scheme

![data schema](https://user-images.githubusercontent.com/33662631/175322984-6409370d-d576-4016-bda5-8a1200338a55.png)

The model foresees **metadata** about the IAS management project and five tables:
- **Actors** table about the people involved in the project, making a distinction between field managers and field executors.
- **Taxa** table containing the targeted IAS taxa as well the by catch.
- **Actions** table containing the performed management actions ...
- **Evaluations** table containing observations assessing the status of invasion of a certain location. Based on evaluations, actions can be planned and assigned to field executors. We decided to use the term _evaluations_ instead of simply observations, as it fits better the jargon used within the IAS management community. As shown in the figure above, evaluations are linked to a location, not a specific action. This approach has the advantage to better track the IAS management progress over time.
- Locations table containing the locations where both actions and evaluations take place. Locations can be points, lines or polygons.

## Proposed data exchange format

Management data are tabular and so they can fit the Frictionless Tabular Data Package format. [Tabular Data Package](https://specs.frictionlessdata.io/tabular-data-package/) is a simple container format used for publishing and sharing tabular-style data.

## Contribute

Questions? Suggestions? **Use cases**? Contribute to the development of manIAS by watching the [repository](https://github.com/riparias/manIAS) and participating in [issue discussions](https://github.com/riparias/manIAS/issues).
