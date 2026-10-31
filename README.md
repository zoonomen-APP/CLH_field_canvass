# CLH field canvass

What each herbarium's data look like in the Consortium of Lichen Herbaria (CLH), as the portal's public download holds them.

The pages are at https://zoonomen-app.github.io/CLH_field_canvass/ (start from the index).

## What the pages show

Each page describes one herbarium's records in snapshot clh_2026_08, the public download of the whole portal made in August 2026: how many records there are, which of the download's 106 fields hold values and how often, which values are most repeated, and the spread of years and elevations.

The pages describe; they do not grade. A value that looks unusual from outside may be the best answer to a constraint that cannot be seen from here. The people who know why are the herbarium's own curators.

## Things worth knowing when reading them

Field names are those of the public download (Darwin Core terms). The portal's own pages use other labels for some of them: "Collector" is recordedBy, "Number" is recordNumber, "Additional Collectors" is associatedCollectors, "Determiner" is identifiedBy, "Date" is eventDate.

Some fields are filled by the portal, not by the herbarium (for example the higher taxonomic ranks, from the portal's thesaurus, and identifiers the portal assigns). Values there say little about a herbarium's own entry work.

A field counts as filled when it holds anything other than an empty or whitespace-only string. Placeholders such as "s.n." or "[data not captured]", and codes such as recordSecurity "0", count as filled.

Codes are the institutionCode values in the download. Codes beginning "hb." are personal herbaria. Some codes hold very few records.

## What is not included

institutionCode "Consortium", which is not a herbarium; codes that are comma-separated lists of herbaria; and the code IIBYT (66 records), whose name differs from IIByT only in capital letters, which file names here cannot keep apart.

## How it was made

From the public download only, loaded into a local SQLite database and summarized with shell, awk and R scripts. The scripts are kept in the author's working files, not in this repository.

This is a dated snapshot. A later canvass, if made, will sit beside this one rather than replace it, so that changes made by curators can be seen.

## Who

Prepared by Alan Peterson, an independent researcher. Not affiliated with CLH or Symbiota. Corrections and comments are welcome.
