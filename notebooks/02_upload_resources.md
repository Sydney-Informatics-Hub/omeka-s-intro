# Upload resources

I'm going to start with one of the worksheets from the spreadsheet and upload it into Omeka S.

This is a version of Omeka S running on my laptop, but it's the same
distribution we're using for Curated Collections

Each location will have a resource or item in Omeka S - you can think
of these as entities or rows in a database.

Omeka S comes with some pre-installed templates for resources - these
are recommended because they use standard vocabularies for their field
names, which is important for long-term preservation - eventually we'll
be exporting collections to an archival format, and the standard
vocabularies mean that those archives will be accessible for future
platforms.

We're going to start with the locations spreadsheet and use them to
create "Place" resources in Omeka S.

Before we start this - when importing tabular data into a system like
Omeka S, we want to be able to use Omeka's ability to create links based
on identifiers in the spreadsheet.

So when we import a row representing a quotation, we'll tell Omeka S to
look up the carceral site and geolocations by their ID, and create
links in the database automatically.

For this to work, we need to think about the order in which we import
the different tables - today I'm going to import the locations, the
carceral sites and quotations, in that order.

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

Click the + icon next to "ID [GEO-xxx]" and a panel with the header
"Add mapping". We get a panel which lets us select one of the fields from
the resource templates. I'm choosing "identifier" from schema.org -
there's also an "Identifier" from Dublin Core and it's important that
we stay consistent.

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


