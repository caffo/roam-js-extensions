## Sort Linked References

The Sort Linked References extension adds an icon button to the user's page that could be used to sort linked references.

### Usage

The script supports the following configuration attributes, to be added in the `[[roam/js/sort-references]]` page:

- `Default Sort` - (Optional) The default mode used to sort references on all pages. Valid values include all the options below, written without the 'Sort By' prefix. For example, `Default Sort:: Page Title`.

Near the linked references, there will appear a sort icon next to the filter icon. Clicking on the sort icon will make a sort menu visible to the user with the following options:

- Sort By Page Title - This will sort all the linked references in ascending alphabetical order of the page title.
- Sort By Page Title Descending - This will sort all the linked references in descending alphabetical order of the page title.
- Sort By Created Date - This will sort all the linked references in ascending order that the page was created.
- Sort By Created Date Descending - This will sort all the linked references in descending order that the page was created.
- Sort By Daily Note - This will sort all the linked references in ascending order by Daily Note, followed by created date of non-daily note pages.
- Sort By Daily Note Descending - This will sort all the linked references in descending order by Daily Note, followed by created date of non-daily note pages.

You could also add a `Default Sort` attribute with a valid value on the page itself to have a specific sorting for just that page. 

```javascript
var old = document.getElementById("sort-references");
if (old) {
  old.remove();
}

var s = document.createElement("script");
s.src = "https://roam.davidvargas.me/master/sort-references.js";
s.id = "sort-references";
s.async = false;
s.type = "text/javascript";
document.getElementsByTagName("head")[0].appendChild(s);
```

### Demo

<video width="320" height="240" controls>
  <source src="../../videos/sort-references.mp4" type="video/mp4">
</video>

<br/>

<iframe src="https://github.com/sponsors/dvargas92495/button" title="Sponsor dvargas92495" height="35" width="116" style="border: 0;"></iframe>
