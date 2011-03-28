ACNFP Gene Models
==========

Non-model resources often have a set of gene models that evolve quite quickly, and it is easy to lose track of why particular genes were added, removed or modified. Checking our gene models into version control allows us to track who editied which models and why (assuming that people leave sensible commit messages). It also allows us to apply pre-commit hooks to ensure that the changes made do not result in incomprehensible gene models. NOTE: The hooks are yet to be finalised. The hooks will check to ensure that features are not left orphaned (eg: mRNA without gene) and that each protien does not include premature stop codons.

Genomes Currently Available
----------

### Stagonospora nodorum sn15 ###

S. nodorum sn15 was the first genome published by the ACNFP ([Hane et al., 2007](http://dx.doi.org/10.1105/tpc.107.052829)).

Genomes Coming Soon
----------
### Stagonospora nodorum sn79-1087 ###
### Stagonospora nodorum sn4 ###
### Pyrenophora teres sp. teres ###


Wishlist (TODO)
----------
### Wiki ###
It would be nice to run through each of the genes and generate a wiki page for each. Less structured information could then be added by those that are not comfortable with the command line and git. Perhaps a basic template can be set up that has defined fields that are then scraped by a commit hook that updates the gff. An example of a set field might be a boolean flag "Has this gene model been confirmed by experimental data?".
This approach of bi-directional updates might be a little fragile, but the fragility could be mitigated by a very formal gene wiki page template with a small number of very strict fields. Of course, the rest of the wiki page for each gene would be completely editable, allowing for informal notes to be taken.
#### PROS ####
- Keeps all relevant data in the same place
- Easy to control access
- Free version control of the wiki
- Easy layout control

### CONS ###
- Might be dangerous to let the gff be editable from the wiki (via hooks)
- Might be too complicated
- Github will sanitize javascript, so no fancy canvas tag renderings. This would have been awesome, but something similar might be possible with svg (including links!).


