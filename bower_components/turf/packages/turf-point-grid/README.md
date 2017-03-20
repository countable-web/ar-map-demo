# @turf/point-grid

# pointGrid

Takes a bounding box and a cell depth and returns a set of [points](http://geojson.org/geojson-spec.html#point) in a grid.

**Parameters**

-   `bbox` **[Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)&lt;[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)>** extent in [minX, minY, maxX, maxY] order
-   `cellSize` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** the distance across each cell
-   `units` **\[[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)]** used in calculating cellSize, can be degrees, radians, miles, or kilometers (optional, default `kilometers`)

**Examples**

```javascript
var extent = [-70.823364, -33.553984, -70.473175, -33.302986];
var cellSize = 3;
var units = 'miles';

var grid = turf.pointGrid(extent, cellSize, units);

//=grid
```

Returns **[FeatureCollection](http://geojson.org/geojson-spec.html#feature-collection-objects)&lt;[Point](http://geojson.org/geojson-spec.html#point)>** grid of points

<!-- This file is automatically generated. Please don't edit it directly:
if you find an error, edit the source file (likely index.js), and re-run
./scripts/generate-readmes in the turf project. -->

---

This module is part of the [Turfjs project](http://turfjs.org/), an open source
module collection dedicated to geographic algorithms. It is maintained in the
[Turfjs/turf](https://github.com/Turfjs/turf) repository, where you can create
PRs and issues.

### Installation

Install this module individually:

```sh
$ npm install @turf/point-grid
```

Or install the Turf module that includes it as a function:

```sh
$ npm install @turf/turf
```