# Phase 4: System/Design Requirements

## *Navbar (global asset)*
### Navbar is one section on *all* pages and must satisfy:
1. Brand logo and product title
2. Page navigation links to Home, Learn, Game, and Special Cases
3. Page navigation should reflect current page with an underline bar
4. Navigation bar is in a fixed position (top of page)

## *Footer (global asset)*
### Footer is one section on *all* pages and must satisfy:
1. Footer states "INFO 442 Project"
2. Footer has "Contact Us" link which is an a href = "mailto:" attribute
3. Footer contains copyright symbol
## *Homepage*
### Home page is one section and must have:
1. A top-level heading that says “It’s our planet.”
2. A paragraph that contains our mission statement
3. “Learn more” button that links to the Learn page  
4. A photo related to our mission statement such as sustainability and responsible waste management  
5. Does not include sections  

## *Learn page*
### Learn page is divided into 5 sections (top to bottom):
#### L1: “Recycling statistics”
1. A paragraph containing statistics about recycling and waste consumption to generate empathy and motivation from the user in order to align them with our mission  
2. A photo related to the statistic, such as littering or landfills  
3. A top level-heading that says “Recycling Statistics”  
#### L2: “What can I compost?”
- Section should contain cards, cards should have:
  1. A photo of a compostable item
  2. Description/title of item
  3. Should only have 4 cards per row
#### L3: “What can I trash”
- Section should contain cards, cards should have:
  1. A photo of a trash item
  2. Description/title of item
  3. Should only have 4 cards per row
#### L4: “What can I recycle”
- Section should contain cards, cards should have:
  1. A photo of a recyclable item
  2. Description/title of item
  3. Should only have 4 cards per row
#### L5: “Reduce, reuse, recycle” triad
- 3x3 table
  1. Row 1 should contain 3 photos over 3 columns related to reduce, reuse, recycle
  2. Row 2 should contain paragraphs of “reduce”,“reuse”, and “recycle” over 3 columns
  3. Row 3 should contain an image of arrows displaying “ reduce”, “reuse”, and “recycle” over 3 columns
  4. Title the table “Reduce, Reuse, Recycle”


## *Game page (interactive)*
### Game page has 3 total sections: Static header, interactive "play space", and responsive drop boxes
#### G1: Header should contain:
1. Header title "Recycle Game"
2. paragraph description of how to play the game/what the game is
#### G2: “Play space” should contain:
1. a draggable card with
    - An image of the active game item
    - Description of the item below image
    - Kebab vector showing the card is manipulatable
    - Card should increase its drop-shadow when clicked, and move with the cursor if the user clicks and drags.
    - Card should snap back to its starting position unless dragged into the correct bin
2. A button “new item” that once clicked changes the draggable card to the next active game item
#### G3: “Drop bins” should contain:
1. Three responsive drop-bin sections
    - Recycle bin
    - Trash bin
    - Compost bin
2. Each bin should respond to user interaction if they drag an item into the correct bin by:
    - If the item is dropped into the correct bin, overlay a “Correct” header and paragraph about why the user is correct
    - Hold the active item until user clicks “new item” button
    - Populate the native land with brand mascot and “great job” message
3. If bin detects an incorrect answer:
    - If the item is dropped into the incorrect bin, overlay an “incorrect” header
    - Automatically repopulate the draggable element back to its starting position
    - The bin should no longer function and the message should remain until the user clicks “new item”

## *Special cases page*
### Special cases is divided into two sections: One permanent header section, and one repeating unit section
1. Special Cases header
    - A top-level heading that says “Special Cases”
    - a paragraph explaining the purpose of the page, which is to showcase the items that are special cases when it comes to responsible waste management
2. Actual special case item (repeating)
    - Section divider spanning the full width of main-body flex box on top
    - A level-three heading of the item name (Example: “batteries”, “light bulbs”, etc).
    - List elements of the special instructions to dispose of the item responsibly
    - List elements should be unordered (bullet points)
    - If list elements contains emails or phone numbers, it should use the href = "mailto:" or "tel:" attribute
