# Objective: 
Refractor starter code.

## Technical Debugging  

### **Broken Links**  

#### ** * Search Engine Optimization**  
> *Issue:* The jump to section when clicking on "Search Engine Optimization" in the header renders no action.  
> *Soluation:* The corresponding id declaration was missing from the "Search Engine Optimization" `div`. This was fixed by changing the following:  
>>`<div class="services">` -> `<div id="search-engine-optimization" class="services">`  

#### ** * Horiseon Logo **  
> *Issue:* The Horiseon logo rendered no action and did not re-link to the home page.    
> *Soluation:* An `a` tag was added to the corresponding `h1` tag to redirect back to the `index.html` file when clicked by the user. This was done by changing the following:  
>>`<h1>Hori<span class="seo">seo</span>n</h1>` -> `<h1><a href="index.html">Hori<span class="seo">seo</span>n</a></h1>`  

## Code Clean-Up

### Consolidation of Duplicated Code

> *Issue:* Many of the CSS styles were duplicated with unnecessary multiple class declarations.  
> *Soluation:* Unnecessary classes were consolidated into one class. The following is the list of class changes:  
>> `search-engine-optimization`, `online-reputation-management`,
and `social-media-marketing` -> `services`  
>> `benefit-lead`, `benefit-brand`, and `benefit-cost` -> `benefit`