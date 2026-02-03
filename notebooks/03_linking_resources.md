# Uploading more resources

Now we're going to upload a second CSV file of Carceral Sites.

This one can link to the existing Geolocations, but I also noticed
that the sites have related links - some of these won't work on
import because they are circular

use isRelatedTo, not relatedTo

There is an inverseProperties module which can create bidirectional
links

Go through cutting and pasting the Sites, and get to the failed
import with the mysterious error messages

Find and replace the weird en-dash hyphens in the spreadsheet and
start again

Note that Dublin Core : identifier and schema.org: identifier are
different

Circular references have not been resolved : screenshot



Now we're going to upload a third CSV file with quotations. These
will be imported as Text items.

First problem - saving the sheet as a CSV and exporting gives the
unequal columns error.

Quick fix - select the exact columns and rows, cut and paste into a
new spreadsheet and save that as CSV.

We select Text as the resource template. Here's a screenshot of the
Text template - we can see that the only required field is 'name'.

When we upload, there's a report of identifiers which Omeka S has not
been able to find in the database already [ screenshot ] - this can
be because of typos in the spreadsheet or inconsistencies.

By default, Omeka S will still add resources if it can't resolve a link.

The way to handle this is to either manually add the links in Omeka S,
or delete the items uploaded, fix the spreadsheet and re-import.

Depending on how many errors there are, the first (updating the links
in the website) might be less work.


