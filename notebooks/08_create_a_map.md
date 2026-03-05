# Create a map

We're going to add a new page to our site with a map showing all of the
carceral sites.

First, we need to assign all of the items in Omeka to the site. Every
site in an Omeka S instance has a collection of items which it "knows
about" and will show up in its searches and visualisations - it's
possible to configure this to automatically include new items, but
by default a new site won't have any items in it. Click the "Resources"
item in the left nav panel, which takes us to the Resources page

![Resources](figures/07_resources.png)

Select the second option, "Add - keep existing items and assign items from a new search query"

Underneath this is a section to define a search query, which we'd use
if we only wanted to add some items to the site. We want to add everything,
so we can leave the query empty.

Click "Save" to add the items to the site.

![Resources](figures/07_add_resources.png)

After this you should be able to click in the "Items" entry under
"Resources" on the left nav panel and see a list of all of the items.

![Resources](figures/07_added_items.png)

Now that the site has some items, we're ready to put them on a map. Click Pages in the left nav panel, then click "Add new page".

![Add new page](figures/07_add_page.png)

Like the site as a whole, the page needs to have a title, and the URL
slug can be customised but usually will just be the title.

![New page](figures/07_new_page.png)

The page editor looks like this:

![Page editor](figures/07_page_editor.png)

We can build up a page by adding one or more blocks - each block is like
a component which provides a particular bit of web functionality in the
page once it's live. This can be something dynamic and interactive like
a map or a timeline, or just some static content.

We're going to add one block to this - "Map by query"



The "Map by query" has a lot of details in it - we can leave the defaults
for now

Click the "Save" button in the top left hand corner


