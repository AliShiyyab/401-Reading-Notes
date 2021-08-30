# RecyclerView

## Key classes

* `RecyclerView` is the **ViewGroup** that contains the views corresponding to your data.
* `Each` individual element in the list is defined by a view **holder** object. 
* The RecyclerView requests those views, and binds the views to their data, by calling methods in the **adapter**. You define the adapter by extending `RecyclerView.Adapter`.
* The layout manager arranges the individual elements in your list. Layout managers are all based on the library's `LayoutManager` abstract class.

## Steps for implementing your RecyclerView

* First of all, decide what the list or grid is going to look like. Ordinarily you'll be able to use one of the `RecyclerView` library's standard layout managers.
* Design how each element in the list is going to look and behave. Based on this design, extend the `ViewHolder` class. Your version of `ViewHolder` provides all the functionality for your list items. Your view holder is a **wrapper around a View**, and that view is managed by `RecyclerView`.
* Define the Adapter that associates your data with the `ViewHolder` views.

## Plan your layout

* The items in your RecyclerView are arranged by a LayoutManager class.
    * `LinearLayoutManager` arranges the items in a one-dimensional list.
    * `GridLayoutManager` arranges all items in a two-dimensional grid:
        * If the grid is arranged vertically, GridLayoutManager tries to make all the elements in each row have the same width and height, but different rows can have different heights.
        * If the grid is arranged horizontally, GridLayoutManager tries to make all the elements in each column have the same width and height, but different columns can have different widths.
    * `StaggeredGridLayoutManager` is similar to GridLayoutManager, but it does not require that items in a row have the same height (for vertical grids)

