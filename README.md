# fSelect
A jQuery select box replacement library ([live demo](https://jsfiddle.net/r0pw7g11/3/))

<img src="https://image.ibb.co/g7AcFU/Capture54.png"  />

### Usage
```html
<select class="your-select-box" name="paramName[]" multiple>
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="opel">Opel</option>
</select>
```
```javascript
$('.your-select-box').fSelect();
```

### Available options

```javascript
$('.your-select-box').fSelect({
    placeholder: 'Select some options',
    numDisplayed: 3,
    overflowText: '{n} selected',
    noResultsText: 'No results found',
    searchText: 'Search',
    showSearch: true
    showSelectAll: true,
});
```

* **placeholder** (str) - the default placeholder text
* **numDisplayed** (int) - the number of values to show before switching to the `overflowText`
* **overflowText** (str) - the text to show after exceeding the `numDisplayed` limit
* **noResultsText** (str) - the text to show if no choices exist (or an empty string)
* **searchText** (str) - the search box placeholder text
* **showSearch** (bool) - show the search box?
* **showSelectAll** (bool) - show the Select All option?

### Single vs. multi-select

Add the `multiple` attribute to your `<select>` to enable multi-select:

```html
<select class="your-select-box" name="paramName[]" multiple>
```
