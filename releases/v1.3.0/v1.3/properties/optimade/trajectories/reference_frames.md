# reference frames (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.3/properties/optimade/trajectories/reference_frames`](https://schemas.optimade.org/defs/v1.3/properties/optimade/trajectories/reference_frames.md)**  
**Definition name:** `reference_frames`

**Property name:** reference frames  
**Description:** The indices of a set of frames that give a good but very brief overview of the trajectory.
The first reference frame could for example be a starting configuration, the second a transition state and the third the final state.  
**Type:** list  

**Requirements/Conventions**:

- The values MUST be larger than or equal to 0 and less than nframes.

**Examples:**

- `[0, 397, 1000]`

**Formats:** [[JSON](reference_frames.json)] [[MD](reference_frames.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.3/properties/optimade/trajectories/reference_frames",
    "$schema": "https://schemas.optimade.org/meta/v1.3/optimade/property_definition.json",
    "title": "reference frames",
    "x-optimade-type": "list",
    "x-optimade-definition": {
        "label": "reference_frames_optimade_trajectories",
        "kind": "property",
        "version": "1.3.0",
        "format": "1.3",
        "name": "reference_frames"
    },
    "x-optimade-dimensions": {
        "names": [
            "dim_trajectory_reference_frames"
        ],
        "sizes": [
            null
        ]
    },
    "type": [
        "array",
        "null"
    ],
    "description": "The indices of a set of frames that give a good but very brief overview of the trajectory.\nThe first reference frame could for example be a starting configuration, the second a transition state and the third the final state.\n\n**Requirements/Conventions**:\n\n- The values MUST be larger than or equal to 0 and less than nframes.",
    "examples": [
        [
            0,
            397,
            1000
        ]
    ],
    "x-optimade-unit": "inapplicable",
    "items": {
        "x-optimade-type": "integer",
        "type": [
            "integer"
        ],
        "x-optimade-unit": "inapplicable",
        "description": "A frame index. It MUST be larger than or equal to 0 and less than nframes.",
        "examples": [
            397
        ]
    }
}
```