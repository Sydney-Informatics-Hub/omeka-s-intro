# Editing an item

This is the main page used to edit and create new items in Omeka S -
it looks fairly complicated because this is where you see a lot of
the metadata-nerd aspects of Omeka S, but underneath that it's
relatively simple

![Editing an item](figures/04_edit_item.png)

If we remember our diagram at the start, it showed what a Carceral
Site looks like as a data object:

![Carceral object](figures/04_carceral_site.png)

This diagram shows one of our carceral site properties, "Cartographic
Name", and what it looks like in the Omeka S edit page:

![Carceral object edit](figures/04_item_diagram.png)

There's two reasons for all the extra complexity here. One is that
Omeka S properties have to be defined as part of a _vocabulary_ -
these are metadata standards defining what certain terms mean.

You can see the list of vocabularies in this Omeka S on the left panel
of the edit view:

![Vocabularies](figures/04_vocabularies.png)

The first four of these are part of our standard distribution # Editing an item

This is the main page used to edit and create new items in Omeka S -
it looks fairly complicated because this is where you see a lot of
the metadata-nerd aspects of Omeka S, but underneath that it's
relatively simple

![Editing an item](figures/04_edit_item.png)

If we remember our diagram at the start, it showed what a Carceral
Site looks like as a data object:

![Carceral object](figures/04_carceral_site.png)

This diagram shows one of our carceral site properties, "Cartographic
Name", and what it looks like in the Omeka S edit page:

![Carceral object edit](figures/04_item_diagram.png)

There's two reasons for all the extra complexity here. One is that
Omeka S properties have to be defined as part of a _vocabulary_ -
these are metadata standards defining what certain terms mean.

This can make the interface complicated - the value is that when we
use these predefined terms, it will allow us to build an archived
version of the Carceral Archipelago collection which can be used
outside Omeka S, and which has long-term sustainability.

You can see the list of vocabularies in this Omeka S on the left panel
of the edit view:

![Vocabularies](figures/04_vocabularies.png)

The first four of these are part of our standard distribution # Editing an item

This is the main page used to edit and create new items in Omeka S -
it looks fairly complicated because this is where you see a lot of
the metadata-nerd aspects of Omeka S, but underneath that it's
relatively simple

![Editing an item](figures/04_edit_item.png)

If we remember our diagram at the start, it showed what a Carceral
Site looks like as a data object:

![Carceral object](figures/04_carceral_site.png)

There's two reasons for all the extra complexity here. One is that
Omeka S properties have to be defined as part of a _vocabulary_ -
these are metadata standards defining what certain terms mean.

This can make the interface complicated - the value is that when we
use these predefined terms, it will allow us to build an archived
version of the Carceral Archipelago collection which can be used
outside Omeka S, and which has long-term sustainability.

You can see the list of vocabularies in this Omeka S on the left panel
of the edit view:

![Vocabularies](figures/04_vocabularies.png)

The first four of these are part of our standard distribution. They are
all widely used standards which we don't have to worry too much about
today.  All of this metadata stuff makes the interface complicated -
the value is that when we use these predefined terms, it will allow us to
build an archived version of the Carceral Archipelago collection which
can be used outside Omeka S, and which has long-term sustainability.

Let's go back to a view of our data object and a view which zooms in
to one of its properties, "Cartographic Name", and what it looks like
in the Omeka S edit page:

![Carceral object edit](figures/04_item_diagram.png)

The small label "schema:name" tells us that this field is using the
'name' property from schema.org.

The red * is an indication that it's a mandatory field - you can't create
an item which has it empty.

Underneath the value is an "Add value" button - this allows us to add
extra values. Omeka S allows any property to have multiple values.

The second reason for the extra complexity is the large number of empty
fields, like 'Region', 'Locality', 'Street address' etc:

![Empty fields](figures/04_empty_fields.png)

These are here because when I imported the spreadsheet, I used a
resource template called Place. A resource template is a predefined
set of properties which can be used to create a new item without
having to add every property manually.

This speeds things up a lot when adding items, but the resource
templates have quite a lot of fields, which are left empty when there's
no value for them.

We'll have a quick look at the standard resource templates at the end
of the workshop.

For now, I've added a description (from Wikipedia) to the item I'm
editing - you can do the same. It's probably easiest if we make sure
we're not editing the same record.

![Edit description](figures/04_edit_description.png)

Once you've added something, click the "Save" button in the top right

![After editing](figures/04_edited_item.png)

This will return you to the item view, with a green message saying
"Item successfully updated"

