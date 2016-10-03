#OpenRefine VIAF Reconciliation Script

This script reconciles a list of names against the Virtual International Authority File (VIAF) API to find possible matches and display URIs from VIAF, Library of Congress (LC) and International Standard Name Identifier (ISNI) for the most relevant match. While this automated search is efficient, it is not always accurate so the results of this script always require manual review.

##Using the script

1. Create a new project in OpenRefine using the 'sample-organization-names.csv' file that is included in this repository. 
2. Click on the 'Undo / Redo' tab
3. Click the 'Apply' button
4. Paste the contents of the 'organizationsViafReconciliation.json' file into the window
5. Click the 'Perform Operations' button.

Note that this VIAF search is optimized for organization names by using VIAF's corporateNames index (`"http://viaf.org/viaf/search/viaf?query=local.corporateNames..."`). To optimize the search for personal names, use VIAF's personalNames index (`"http://viaf.org/viaf/search?query=local.personalNames..."`).


This script is based on the work of [Matt Carruthers](https://github.com/mcarruthers).
