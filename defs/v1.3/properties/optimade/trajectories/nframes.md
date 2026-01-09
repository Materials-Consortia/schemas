# number of frames (property)

This page documents an [OPTIMADE](https://www.optimade.org/) [Property Definition](https://schemas.optimade.org/#definitions). See [https://schemas.optimade.org/](https://schemas.optimade.org/) for more information.

**ID: [`https://schemas.optimade.org/defs/v1.3/properties/optimade/trajectories/nframes`](https://schemas.optimade.org/defs/v1.3/properties/optimade/trajectories/nframes.md)**  
**Definition name:** `nframes`

**Property name:** number of frames  
**Description:** The number of frames in the trajectory.
This value indicates the number of frames stored in the data, and may deviate from the number of steps used to calculate the trajectory.
For example, a 10 ps simulation with calculation steps of 1 fs where data is stored once every 50 fs, nframes will be 200.  
**Type:** integer  

**Requirements/Conventions**:

- The integer value MUST be equal to the number of frames in the trajectory (i.e., the length of the dim_frames dimension).
- The integer MUST be a positive non-zero value.

**Querying**:

- A filter that matches trajectories that have exactly 100 frames: `nframes=100`.
- A filter that matches trajectories that have between 100 and 1000 frames: `nframes>=100 AND nframes<=1000`.

**Examples:**

- `42`

**Formats:** [[JSON](nframes.json)] [[MD](nframes.md)]

**JSON definition:**

``` json
{
    "$id": "https://schemas.optimade.org/defs/v1.3/properties/optimade/trajectories/nframes",
    "$schema": "https://schemas.optimade.org/meta/v1.3/optimade/property_definition.json",
    "title": "number of frames",
    "x-optimade-type": "integer",
    "x-optimade-definition": {
        "label": "nframes_optimade_trajectories",
        "kind": "property",
        "version": "1.3.0",
        "format": "1.3",
        "name": "nframes"
    },
    "type": [
        "integer",
        "null"
    ],
    "description": "The number of frames in the trajectory.\nThis value indicates the number of frames stored in the data, and may deviate from the number of steps used to calculate the trajectory.\nFor example, a 10 ps simulation with calculation steps of 1 fs where data is stored once every 50 fs, nframes will be 200.\n\n**Requirements/Conventions**:\n\n- The integer value MUST be equal to the number of frames in the trajectory (i.e., the length of the dim_frames dimension).\n- The integer MUST be a positive non-zero value.\n\n**Querying**:\n\n- A filter that matches trajectories that have exactly 100 frames: `nframes=100`.\n- A filter that matches trajectories that have between 100 and 1000 frames: `nframes>=100 AND nframes<=1000`.",
    "examples": [
        42
    ],
    "x-optimade-unit": "dimensionless"
}
```