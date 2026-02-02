# Upload resources

We're now going to take one spreadsheet and use it to create a set of
resources in Omeka S and add them to the site we've just created.

This installation of Omeka S comes with some pre-installed templates for
resources - in general, it's a good idea to use these.

We're going to start with the locations spreadsheet and use them to
create "Place" resources in Omeka S.

- need to split the lat/longs here

To start the import process, click "CSV Import" near the bottom of the
navigation panel.

We need to go through a couple of pages for this to tell Omeka S how to
map spreadsheet rows to resources.

The first page lets us select the file, and set some basic parameters
for the CSV - the default values for these are fine. Click "Next" when
you've found the spreadsheet.

The next page will have a table for each column in the spreadsheet you've
just uploaded. We need to map these onto values for the resources.

Before we start this, we should select a resource template - select the
"Basic Settings" tab at the top, and select "Place" from the drop-down

Notice that there's also a "Sites" field on this page, which should have
your new site as its value.

Once we've selected Place, clicl "Map to Omeka S Data" to go back to the
list of spreadsheet columns.

Click the + icon next to "ID [GEO-xxx]" and a panel with the header
"Add mapping". Click the "Properties" drop down and search for a property
called "Identifier"

NOTE - you need to click the "Apply changes" button! I always forget this.

If the changes are applied, the column "ID" will have "Identifier" next
to it under "Mappings"

We now need to do this for the other fields except for Geolocation

Geolocation needs to use the mappings tab in the panel


