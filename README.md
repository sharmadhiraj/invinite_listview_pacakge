# Infinite ListView

The Infinite ListView Flutter [package](https://pub.dev/packages/infinite_listview_package) provides
an infinite scroll listview widget.

## Getting Started

1. [Installation Guide](https://pub.dev/packages/infinite_listview_package/install)
2. [Example](https://pub.dev/packages/infinite_listview_package/example)

## Usage Guide

1. Create a class extending `InfiniteListView<T>`, where `T` is the type of item on the list you are
   going to build.
2. Implement the `getItemWidget(T item)` method. This method should return a widget for a single
   item on the list.
3. Implement the `getListData(int pageNumber)` method. This is an `async` method and should return a
   list of items according to the pageNumber parameter. This method should
   return `Future.error(...)` in case of an error.
4. Override
   the `getLoadingWidget()`, `getPaginationLoadingWidget()`, `getErrorWidget(dynamic error)`,
   and `getPaginationErrorWidget(dynamic error)` methods to customize widgets while the request is
   in progress and in case of an error.

<hr/>

I'm always working on making improvements. If you have any feedback, issues, or suggestions, feel
free to reach out. Happy coding!