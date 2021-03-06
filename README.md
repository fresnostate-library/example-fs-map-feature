# Example FS Map Feature Repository
This repository contains the proposed code changes for the interactive Fresno State Map page. 

## Purpose
These code changes should allow one to manipulate the existing map page, so as to show a desired campus building upon the first visit to the page (without needing to use the building selection tool); all through the use of an URL-appended anchor ID ("#example-id"), fragment URL, or location hash property--whichever term you choose to use. 

This ID can be derived either from existing campus mail-stop acronyms (e.g., VR), using the filename of existing building image graphics (e.g., ViticultureEnologyResearchCenter), or adopting the base string of their respective checkbox IDs (e.g., viticulture_and_enology_research_center). For SEO purposes, it might be better to replace any "underscore" with a "hyphen" in the ID.

__IMPORTANT NOTE:__ This proposal only expands functionality that exists *currently* for the [University Center](https://www.fresnostate.edu/map/#universitycenter). The JavaScript code block is found about line 301, in the code view, and starts with the HTML comment: 
```html
// control special case where a direct link is needed to preactivate a set of map items
```

## Example Scenario
For instance, the V.E. Petrucci Library would like to include a link to the campus map page, which would automatically show their building, rather than display a map graphic file or force a visitor to multiple steps in order to find their campus location.

## Working Example
The working code, using the checkbox ID as the fragment URL, examples (any building should work) can be found at: 
- http://www.lib.csufresno.edu/map/#viticulture_and_enology_research_center
- http://www.lib.csufresno.edu/map/#library
