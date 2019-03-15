# Sidewalks Paths and Crossings


## Mapping Crossings

## Elements

* The road
* The intersecting sidewalk, cycleway or path
* The node at which they intersect
* The curb nodes or where the sidewalk surface transitions to road surface (if it does)

### Crossing tags

* `highway=footway`+`footway=crossing` is needed
* `crossing=*`
* `crossing_ref=*`
* `surface=*`
  - `smoothness=*`, `incline=*`
* `barrier=kerb`
  - `kerb=*`, `tactile_paving=*`, `wheelchair=*`

### Common ways to map

  0. null
    - Path and road cross but aren't connected
    - Mapper needs more training
  1. Simple connection
    - Sidewalk intersects road with untagged node
    - Don't do this unless there really is no information known
  2. Crossing node only
    - The intersection is tagged with `footway=crossing`
  3. Separate crossing way
  4. Separate crossing way and kerb nodes
