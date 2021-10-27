# RecyclerView
[Notes taken from this site](https://developer.android.com/guide/topics/ui/layout/recyclerview#java)

- RecyclerView *recycles* elements as they are scrolled off screen and new elements are scrolled on screen.

- Key classes:
  - `RecyclerView`
  - `RecyclerView.ViewHolder`
  - `RecyclerView.Adapter`
  - `LayoutManager`

- Basic steps for implementing RecyclerView
  - Plan your layout. RecyclerView provides three layouts:
    1. `LinearLayoutManager` - arranges data in a one-dimensionsl list.
    2. `GridLayoutManager` - arranges data in a two-dimensional grid.
    3. `StaggeredGridLayoutManager` - similar to `GridLayoutManager`, but columns/rows do not need to have the same width/height.
  - Implement an adapter and view holder. Override 3 key methods:
    1. `onCreateViewHolder()` - creates a new `ViewHolder`
    2. `onBindViewHolder()` - associates a `ViewHolder` with data.
    3. `getItemCount()` - gets the size of the data.

[Back to HOME](../README.md)