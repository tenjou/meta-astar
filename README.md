# meta-astar v1.0

A* pathfinding algorithm implementation.

## Quick start

### Installation

```js
npm install meta-astar
```

### Usage

```js
import AStar from "meta-astar"

const data = [ 0, 0, 0,
	       0, 1, 0,
	       0, 0, 0 ]
const astar = new AStar(data, 3, 3)
const astarOptions = new AStar.Options(0)
const path = []
if(astar.search(0, 0, 2, 2, path, astarOptions)) {
	console.log(path)
}
```

## API

### AStar
```js
AStar(data:Array<int>, sizeX:int, sizeY:int):void
```
```js
AStar.setup(data:Array<int>, sizeX:int, sizeY:int):void
```
```js
AStar.search(startX:int, startY:int, endX:int, endY:int, output:Array<AStarNode>, options:AStarOptions):bool
```
### AStar.Options
```js
AStar.Options(walkableMask:int = 0, diagonal:bool = false, range = 0)
```
