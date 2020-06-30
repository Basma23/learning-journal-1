# Responsive Web Design and Regular Expressions
## Responsive Web Design
**Properties for the Parent(Grid Container):**
- **display:** Defines the element as a grid container and establishes a new grid formatting context for its contents.
   - **grid** – generates a block-level grid
   - **inline-grid** – generates an inline-level grid
- **grid-template-columns & grid-template-rows:** Defines the columns and rows of the grid with a space-separated list of values. The values represent the track size, and the space between them represents the grid line.   
   - **<track-size>** – can be a length, a percentage, or a fraction of the free space in the grid (using the fr unit)
   - **<line-name>** – an arbitrary name of your choosing
- **grid-template-areas:** Defines a grid template by referencing the names of the grid areas which are specified with the grid-area property. 
   -  **<grid-area-name>** – the name of a grid area specified with grid-area
   - **.** – a period signifies an empty grid cell
   - **none** – no grid areas are defined  
- **grid-template** A shorthand for setting grid-template-rows, grid-template-columns, and grid-template-areas in a single declaration.
   - **none** – sets all three properties to their initial values
   - **<grid-template-rows> / <grid-template-columns>** – sets grid-template-columns and grid-template-rows to the specified values, respectively, and sets grid-template-areas to none


**Properties for the Children(Grid Items):**
- **grid-column-start, grid-column-end, grid-row-start, and grid-row-end:** Determines a grid item’s location within the grid by referring to specific grid lines. grid-column-start/grid-row-start is the line where the item begins, and grid-column-end/grid-row-end is the line where the item ends.
   - **<line>** – can be a number to refer to a numbered grid line, or a name to refer to a named grid line
   - **span <number>** – the item will span across the provided number of grid tracks
   - **span <name>** – the item will span across until it hits the next line with the provided name
   - **auto** – indicates auto-placement, an automatic span, or a default span of one
- **grid-column, and grid-row:** Shorthand for grid-column-start + grid-column-end, and grid-row-start + grid-row-end, respectively.
   - **<start-line> / <end-line>** – each one accepts all the same values as the longhand version, including span
- **grid-area:** Gives an item a name so that it can be referenced by a template created with the grid-template-areas property. 
    - **<name>** – a name of your choosing
    - **<row-start> / <column-start> / <row-end> / <column-end>** – can be numbers or named lines
- **justify-self:** Aligns a grid item inside a cell along the inline (row) axis (as opposed to align-self which aligns along the block (column) axis). This value applies to a grid item inside a single cell.
    - **start** – aligns the grid item to be flush with the start edge of the cell
    - **end** – aligns the grid item to be flush with the end edge of the cell
    - **center** – aligns the grid item in the center of the cell
    - **stretch** – fills the whole width of the cell (this is the default)
- **align-self:** Aligns a grid item inside a cell along the block (column) axis (as opposed to justify-self which aligns along the inline (row) axis). This value applies to the content inside a single grid item. 
    - **start** – aligns the grid item to be flush with the start edge of the cell
    - **end** – aligns the grid item to be flush with the end edge of the cell
    - **center** – aligns the grid item in the center of the cell
    - **stretch** – fills the whole height of the cell (this is the default)   

## Regular Expressions
Regular expressions (regex or regexp) are extremely useful in extracting information from any text by searching for one or more matches of a specific search pattern.

Fields of application range from validation to parsing/replacing strings, passing through translating data to other formats and web scraping.

One of the most interesting features is that once we’ve learned the syntax, we can actually use this tool in (almost) all programming languages ​​(JavaScript, Java, VB, C #, C / C++, Python, Perl, Ruby, Delphi, R, Tcl, and many others) with the slightest distinctions about the support of the most advanced features and syntax versions supported by the engines).

**The application fields of regex can be multiple like:**

data validation (for example check if a time string i well-formed)
data scraping (especially web scraping, find all pages that contain a certain set of words eventually in a specific order)
data wrangling (transform data from “raw” to another format)
string parsing (for example catch all URL GET parameters, capture text inside a set of parenthesis)
string replacement (for example, even during a code session using a common IDE to translate a Java or C# class in the respective JSON object — replace “;” with “,” make it lowercase, avoid type declaration, etc.)
syntax highlightning, file renaming, packet sniffing and many other applications involving strings (where data need not be textual)