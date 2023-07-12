# Simplicity

## Content of the health record should be in plain text, in files on disk

**in plain text** so that the content is readable even in low-tech environments. (Ideally a viewer will render this plain text into a much more usable and feature-rich application view. But you have the text-on-disk view there as a fallback.)

**in files** because files can easily be made to work interoperably across all operating systems.

**on disk**, as opposed to being in a database*

!!! note

    yes databases are also on disk somewhere, we know this, but there is a difference between data being buried in a database and being a file on disk.

## New entries in the record should be in a new file

Medical practice can usually be distilled down to an 'atomic unit of care' which is about the right size for resultant clinical record entries. For a clinic visit one might expect a single entry summarising the visit, or possibly a few linked entries

## All GitEHR entries are linkable 

As modern clinical records get larger and more complex, clinicians struggle to find specific items of data. The internet has solved this problem but the use of the URL or internet 'link' - yet this simplest of technologies has not found its way into healthcare records.

