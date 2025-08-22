## Summary
- Most data types can be stored as tables
	- Even audio, images, videos, and text!
- Tables are typically stored in delimited files
	- .csv
	- .tsv
	- other
- Audio / video / images may be stored in other more efficient file formats
### Time Series Data
> Values of the array vary over time

### Images
>1 small box = 1 pixel
>Each pixel has a number for the amount of light in that box:
>0% for black
>100% for white
>In-between

### Color Images
>Similar to black and white images but with another dimension!

### Video
>How many dimensions does a black & white video have?
>	Rows, Columns, time
>What about a color video?
>	Rows, columns, colors, time
>Videos = sequences of images over time 
>	Each image = one frame
>	Number of sequences = frame rate

## Network Graphs

**Basic structure**: Nodes (vertices) connected by edges (links)

## Undirected Graphs

- **Edges have no direction** - connections go both ways
- If A connects to B, then B automatically connects to A
- Examples: Facebook friendships, physical roads, protein interactions
- **Adjacency matrix**: Symmetric (same above and below diagonal)

## Directed Graphs

- **Edges have direction** - connections are one-way
- A can connect to B without B connecting back to A
- Examples: Twitter follows, web page links, email sent/received
- **Adjacency matrix**: Not symmetric

## Quick Example

- **Undirected**: "Alice and Bob are friends" (mutual)
- **Directed**: "Alice follows Bob" (one-way)

## Common representations:

- **Adjacency matrix**: NxN table where 1 = connection, 0 = no connection
- **Edge list**: Simple list of all connections
- **Adjacency list**: Each node lists its neighbors

That's the core difference - whether relationships are mutual (undirected) or one-way (directed).