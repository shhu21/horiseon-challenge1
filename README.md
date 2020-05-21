# Objective: 
Refractor starter code.

## Technical Debugging  

### **Broken Links**  

#### 1. Search Engine Optimization 
> *Issue:* The jump to section when clicking on "Search Engine Optimization" in the header renders no action.  
> *Solution:* The corresponding id declaration was missing from the "Search Engine Optimization" `div`. This was fixed by changing the following:  
>>`<div class="services">` -> `<div id="search-engine-optimization" class="services">`  

#### 2. Horiseon Logo
> *Issue:* The Horiseon logo rendered no action and did not re-link to the home page.    
> *Solution:* An `a` tag was added to the corresponding `h1` tag to redirect back to the `index.html` file when clicked by the user. This was done by changing the following:  
>>`<h1>Hori<span class="seo">seo</span>n</h1>` -> <br>`<h1><a href="index.html">Hori<span class="seo">seo</span>n</a></h1>`  

## Code Clean-Up

### Consolidation of Duplicated Code

> *Issue:* Many of the CSS styles were duplicated with unnecessary multiple class declarations.  
> *Soluation:* Unnecessary classes were consolidated into one class. The following is the list of class changes:  
>> `search-engine-optimization`, `online-reputation-management`, `social-media-marketing` -> `services` <br><br>
>> `benefit-lead`, `benefit-brand`, `benefit-cost` -> `benefit`

<br><br>
**Live URL: ** https://shhu21.github.io/horiseon-challenge1/