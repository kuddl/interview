# Experience Day. Senior Frontend Engineer.

## Basic conditions

### Timing
* 5 minutes preparation
* 60 minutes time to work on
* Clarify questions and uncertainties beforehand

### Presentation
* 10 - 15 minutes presentation
* 10 - 15 minutes dicussion

## Task 1:  Present Angular to our customer (30 Minutes)

We are in a pitch for a new project. Angular is our preferred framework we would like to use in the project. But our customer does not know what Angular is, and why we would prefer it over React or Vue or plain Javascript. Also our team is not 100% firm with Angular.

### ToDo

Create a small presentation (2-3 Slides) with one or two outstanding example, why Angular shines in this case. You can use all ressources (Blogposts, Dokumentation, Stackoverflow).
Afterwards you will present this to the team as if we were the customer. 
Create one slide to convince our customer. 
Create one slide to convince the team (technical topic).

#### Focus:

- this is the "best feature" of Angular 
- clean Presentation (maybe with code example)



## Task 2: Refactoring (30 Minutes)

You are working on aproject with a small team of co-workes. One of them handover to you storage.js.  On the first look it seems ok but then you try to make it run...

### ToDos

-   Try to understand what it should do 
-   Get it running (in the browser or console), anaylse the issues and try to fix them
-   What would help to avoid such problems and issues?

### Code storage.js
```js
const storage = {
  max: undefined,
  items: [],
};
Object.defineProperty(storage, "max", { readonly: true, val: 5000 });
let currentStorage = "undefined";
function storageUsed() {
  if (currentStorage) {
    return currentStorage;
  }
  currentStorage = 0;
  for (const i = 0; i < storage.length(); i++) {
    currentStorage += storage.items[i].weigth;
  }
  return currentStorage;
}
function add(item) {
  if (storage.max - item.weight >= storageUsed) {
    storage.items.add(item);
    currentStorage += iten.weight;
  }
}
```
