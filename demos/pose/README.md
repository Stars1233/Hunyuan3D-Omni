# Bone Data File Description

## Overview

Each pose's skeleton involves two files: a `.txt` file and a `.json` file. The `.txt` file stores the 3D start and end point coordinates of the bone, while the `.json` file contains the names of these bones along with their corresponding 3D start and end point coordinates.

## File Description

### 1. Coordinate Data File (`.txt`)

This file contains the 3D coordinate data for multiple bones, with each line representing the start and end point coordinates of a bone. Each bone is represented by two points, formatted as follows:
```txt
x1 y1 z1 x2 y2 z2
```
where `(x1, y1, z1)` are the 3D coordinates of the starting point of the bone, and `(x2, y2, z2)` are the 3D coordinates of the ending point.

### 2. Skeleton Information File (`.json`)

This file describes the name of each bone and its corresponding 3D coordinate data in JSON format. Each bone name is a key, and the associated start and end point coordinates are an array containing two points. The example format is as follows:
```json
{
    "Bone_Name": [
        [x1, y1, z1],
        [x2, y2, z2]
    ]
}
```
