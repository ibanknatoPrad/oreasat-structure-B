### A What Now?
A syntactic versioning system helps differentiate the various stages of a file as it moves through the production process. This is done by assigning each new version a unique string of numbers in a specific format/order. OreSat files use the standard major.minor.patch format, where three numbers are separated by two periods. One or all of these numbers may incrementally increase depending on the changes made.

![Sample Version](https://upload.wikimedia.org/wikipedia/commons/8/82/Semver.jpg)

### Major
When the major slot is filled by 0, it represents an unfinished product. "Unfinished," in this context, means that the fundamental “stuff” of the file is missing. Any increase to the major would indicate an architectural change.

For example, let's say we changed things so that solar panels would connect at the middle of OreSat1 and batteries/ACS would go on the ends. This would be considered an architectural/major version change [notated as 1.0.0 -> 2.0.0].

### Minor
Minor is reserved for changes that are unable to exchange information with previous major.minor versions. So if the major.minor versions are the same across two files, then all the parts should work together.

### Patch
For the small "Oops, I forgot something" changes, we alter the patch number. Though most of the time, patch will be 0.

### Standard Operating Procedures
The important things to do when updating a version number are:
1. Update the version number on all of the frames
2. Confirm the model builds without errors
3. Push the changes and create a pull request into master
4. Tag the corresponding commit in the master branch on GitHub (after merging into master)
5. Send DXFs of all affected boards to the relevant electrical people
