# RecyclerView

### Create dynamic lists with RecyclerView   

* RecyclerView is a library that easily displays large sets of data. It lets you define how each item should look and how it should appear.

* RecyclerView recycles the elements that it sees when an item scrolls off the screen. It does so by reusing the view for new items so We can get the benefit of using RecyclerView to improve performance.

### Key classes

To build a dynamic list, there are several different classes work together such as:


1. RecyclerView is the ViewGroup that contains the views corresponding to your data.

2. The view holder object is defined for each element in the list. When it is created, the view holder will bind to the data of the RecyclerView.ViewHolder.

3. The RecyclerView requests those views, and binds the views to their data, by calling methods in the adapter.

4. The layout manager arranges the individual elements in the list.

### Steps for implementing your RecyclerView

1. decide what the list or grid is going to look like.

2. Design how each element in the list is going to look and behave

3. Define the Adapter that associates your data with the ViewHolder views

### Plan your layout

The items in your RecyclerView are arranged by a LayoutManager class.

1. LinearLayoutManager arranges the items in a one-dimensional list.

2. GridLayoutManager arranges all items in a two-dimensional vertically and horizontally

3. StaggeredGridLayoutManager, which is similar to GridLayoutManager, but it does not require that items in a row have the same height (for vertical grids) or items in the same column have the same width (for horizontal grids).


### Implementing your adapter and view holder

When you define your adapter, you need to override three key methods:

1. onCreateViewHolder() RecyclerView calls this method whenever it needs to create a new ViewHolder.

2. onBindViewHolder() RecyclerView calls this method to associate a ViewHolder with data.

3. getItemCount()RecyclerView calls this method to get the size of the data set.

**************
[RecyclerView for displaying lists of data - source site](https://developer.android.com/guide/topics/ui/layout/recyclerview#java)

**************
