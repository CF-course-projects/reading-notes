# RecyclerView for displaying lists of data

## Create dynamic lists with RecylcerView
- You supply the data and define how it looks and RecyclerView library dynamically creates the elements when they're needed
- As the name implies, RecyclerView recyclers elements of list that have been scrolled off the list.

### Key classes
- RecyclerView is the ViewGroup that contains the views corresponding to your data. It is a view itself, so you add Recycler view into your layout like any other UI element
- Each individual element in the list is a ***view holder*** object. You can define a `view holder` by extending `RecyclerView.ViewHolder`.
- The `RecylcerView` binds the views to their data by calling methods in the `adapter`. You can define the adapter by extending `RecyclerView.Adapter`
- The `LayoutManager` arragnes the individual elements in your list. You can use one of the layout managers provided by the RecyclerView library, or define your own.

### Steps for implementing your Recycler View
- Plan your layout 
  - Items in RecyclerView are arranged via `LayoutManager` class. The RecycleView library provides the three most common layout managers
    - `LinearLayoutManager`: one dimensional list
    - `GridLayoutManager`: two dimensional list
    - `StaggeredGridLayoutManager`: similar to GradLayoutManager, but does not require items to ahve the same height
- Implementing your adapter and view holder
  - `ViewHolder` is a wrapper around a `View` that contains the layout for an individual item in the list.
  - `Adapter` creates `ViewHolder` objects and sets the data for those views. 
  - When defining your `Adapter` you need three key methods:
    - `onCreateViewHolder()`: `RecyclerView` calls this method to create a new `ViewHolder`
    - `onBindViewHolder()`: `RecyclerView` calls this method to bind a `ViewHolder` with data. 
    - `getItemCount()`: `RecyclerView` calls this method to get the size of the data set. RecyclerView usees this to determine when there are no more items to display
  