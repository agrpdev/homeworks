# Algorithms

## Text highlight algorithm

Your task is to create a text highlighting algorithm:

Document example:

```
 <div id="doc">
 Hello, welcome to the text document.
 <div id="asdfge">
 Please read first section of <a href="http://who.org">WHO</a> chart. As soon as you come to the conclusion...
 <div id="34223asf">
 This text is located in inner-section, effectively a subsection of super section. <span class="bold">This</span> section contains interesting data, about some other stuff.
 </div>
 </div>
 </div>
```

Algorithm specification:
 
 - backend receives id of source div, starting offset and highlighted text from frontend and performs highlighting logic
 - backend returns html with highlights
 - highlight is rendered in span with highlight ID and specific class `<span>`

1) User can create text highlight of arbitrary size, crossing section boundaries  
  `welcome to the text document. Please read first section of`
2) Bordering highlights are merged together  
 e.g. highlight `welcome to the text document.` is created, then highlight ` Please read first section of` is created and those are merged into `welcome to the text document. Please read first section of`
3) Highlight can "eat" another highlight (or highlights) if it fully overlaps it   
  e.g. highlights `to the text document.` and `Please read` are created, overlaping highlight `welcome to the text document Please read first` replaces them
4) Highlight partially overlaping another highlight shrinks that highlight   
 e.g. `welcome to the text document.` highlight exists, highlighting `welcome to the` results in two existing highlights - `welcome to the` and ` text document.`
5) All conditions apply together

Assignment:

1) How would you hold and store highlight informations? Each user can have his own highlights and a-href links in underlying document can change their position and target (not the text content)
2) Write an algorithm implementing given highligting logic


