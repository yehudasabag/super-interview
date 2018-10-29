# super-interview
An interview question for full-stack position

Hi,

Your task is to build a map that shows a supermarket structure by shelves. 
## Client side (React.js)
In client side you should create one page that shows the supermarket map of shelves. A shelf is a simple rectangle.
When the user click on the shelf, you should show the list of products in this shelf. You should decide how the products will be shown to the user. Think and take a decision that seems right to you. There is no 'right answer'.

## Server side (Node.js)
On the server side, you should use the 'supermarketData.json' file in this repo as your DB. No need to push the data to a real DB, you can keep it in server memory or in file, whatever you prefer. I do recommend to keep the data in efficient way.

The server should expose 2 apis:
1. Get all the supermarket shelves
2. Get products of a shelf

The client should use those apis in order to represent the data.

## Data explained
### Store
```json
  "store": {
		"name": "Oriient store",
		"xLength": 20,
		"yLength": 13
	}
```
xLength - the size of the store in meters in x axis

yLength - the size of the store in meters in y axis

The (0,0) coordinate is the bottom-left of the store

### Shelf
```json
    {
        "shelfNum": 1,
        "coordinates": {
            "x": 3,
            "y": 2
        },
        "xLength": 2,
        "yLength": 3
    }
```
coordinates - these are coordinates of the shelf in the store. Notice that these coordinates are from the bottom-left of the store.

xLength - the length of the self in the x axis

yLength - the length of the self in the y axis

### Product
shelf - correspond to the the shelfNum in the shelves data

Good luck and feel free to ask me any question.

### Important
Do not invest too much time. If you see it takes too much time feel free to submit only part of the exercise. 
