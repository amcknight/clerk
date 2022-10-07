# clerk
A force-based, live dependency visualization tool that allows for unknown dependencies, disconnected graphs, and a small amount of cyclic dependencies. Designed with the Jets of Time Chrono Trigger randomizer in mind, but with hopes of generalizing much further.

## Install

`git clone` it

## Run

Just open `index.html` in a browser

## Changelog

### Unreleased
- Connected nodes attempt to stay vertically aligned
- Dependent nodes attempt to be a fixed distance above they're parents
- Nodes don't overlap much by pushing eachother out of they're rectangles
- "Next" line exists and has a node linked to it

## Roadmap

### v0.1
- Start with the standard race-flags Jets of Time graph loaded
- Add disconnected graph logic
  - Closed graphs push left
  - Open graphs push middle/right
  - Open Go mode graphs push right
  - Order by big to small, left to right
- Open nodes are in the "Next" bar
- Item types are colored differently
- Open pathways are colored or outlined differently

### v0.2
- Cycles of dependencies are treated differently to prevent "flattening"
- Event capturing
  - Item completion
  - Linking of newly discovered dependency

### v0.3
- Loading a dependency graph from a file
- Completed nodes that aren't saved are greyed out instead of deleted
- Save
- Revert

### Beyond
- Automatic event capturing for Jets of Time and other randomizers
- Editor for creating new dependency types