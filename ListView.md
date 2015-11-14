# List View #

_Coming Soon_

# Indexed List View #

The `IndexedListView` is an extension of the `ListView`, and will sort and group items alphabetically. Just like the `ListView`, the `IndexedListView` also implements `HasData<T>`.

First, we create the `IndexedListView`:

```
IndexedListView<String> indexedListView =
		new IndexedListView<String>();
```

Next, we create an `ArrayList` of type `String` and add our data:

```
List<String> list = new ArrayList<String>();
list.add("Doe, Jane");
list.add("Smith, John");
```

Then we create a `ListDataProvider`, which we give the `ArrayList`, and then bind to the `IndexedListView`.

```
ListDataProvider<String> dataProvider =
		new ListDataProvider<String>();

dataProvider.setList(list);
dataProvider.addDataDisplay(indexedListView);
```