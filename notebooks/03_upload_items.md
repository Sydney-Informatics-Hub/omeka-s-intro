# Upload resources


We're going to start with the locations spreadsheet and use them to
create "Place" resources in Omeka S.

Omeka S comes with some pre-installed templates for resources - these
are recommended because they use standard vocabularies for their field
names, which is important for long-term preservation - eventually we'll
be exporting collections to an archival format, and the standard
vocabularies mean that those archives will be accessible for future
platforms.


Before we start this - when importing tabular data into a system like
Omeka S, we want to be able to use Omeka's ability to create links based
on identifiers in the spreadsheet.

So when we import the second spreadsheet, representing carceral sites,
we'll tell Omeka S to look up the location by its ID, and create
links in the database automatically.

![FIXME diagram](figures/relations_between_linked_tables)

For this to work, we need to think about the order in which we import
the different tables - we'll import the locations and then the carceral
sites.


To start the import process, click "CSV Import" near the bottom of the
navigation panel.

![CSV import](figures/02a_csv_import.png)

We need to go through a couple of pages for this to tell Omeka S how to
map spreadsheet rows to resources.

The first page lets us select the file, and set some basic parameters
for the CSV - the default values for these are fine.

![Import settings](figures/02b_select_file.png)

The next page will have a table for each column in the spreadsheet you've
just uploaded. We need to map these onto values for the resources.

Before we start this, we'll select a resource template for Omeka S to
use when creating the new items. Select the "Basic Settings" tab at the top, and select "Place" from the drop-down next to "Resource template"

![Basic settings](figures/02c_basic_settings.png)

Once we've selected Place, click the "Map to Omeka S Data" to go back to the list of spreadsheet columns.


Note that in this part of Omeka S's interface, the word 'map' is used
in two completely different senses. One is the normal, everyday sense of
putting records onto a map so that we can see where they are
geographically.

The other sense comes from maths and computer science, and it means taking
a set of fields in one system and defining where their values are going
to go in a second system.

This correspondence - in our case, between columns in a CSV, and fields
in items in Omeka S - is called a "mapping", and it's in this sense that
the heading on this page uses it in when it says "Map to Omeka S data"

![Map to Omeka](figures/02d_column_mappings.png)

Click the + icon next to "ID [GEO-xxx]" and a panel with the header
"Add mapping". We get a panel which lets us select one of the fields from
the resource templates. I'm choosing "identifier" from schema.org -
there's also an "Identifier" from Dublin Core and it's important that
we stay consistent.

![FIXME](figures/

NOTE - you need to click the "Apply changes" button! I always forget this.

If the changes are applied, the column "ID" will have "Identifier" next
to it under "Mappings"

We now need to do this for the other fields, with two exceptions

One is the link to Carceral sites - as these haven't been uploaded yet,
we can't expect Omeka S to find them, so we're going to try to create
reverse links when we upload the sites.

The other is Geolocation - I've split the latitude and longitude into
two columns, and use the Mapping tab to tell Omeka to use this as spatial
information


