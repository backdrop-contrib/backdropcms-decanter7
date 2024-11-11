# Decanter (v7) Styles and Classes

Decanter 7 and tailwind come with a large number of css classes which can be used within the Backdrop admin interface to change the look of standard Backdrop elements to match the examples from the [Decanter Developer Site](https://decanter.stanford.edu/examples/cards)

## Cards

Cards are a standard way of displaying summary content. These cards may link to other content, to the detail view of the card content or may just be informational with no links at all. There are three standard card styles:


### Card Types

#### Plain

Plain cards are minimally adorned and best for simple information and links to content. Cards will automatically take this form or you can use the class `.plain`.

![A plain card with a Call to Action link](img/card-plain.png)

#### Bordered

Bordered cards have a moderate level of decoration and provide a more impactful visual for high criticality and news links. This style can be invoked with the `.bordered` class.

![A bordered card with a credit and external link](img/card-bordered.png)

#### Dark

The dark or 'background' card has a dark background and contrasting text for the most visual impact. Use the `.dark` or `.background` class.

![A bordered card with a credit and external link](img/card-black.png)

### Creating Cards with Paragraphs Aplenty

The [Paragraphs Aplenty module](https://backdropcms.org/project/paragraphs_aplenty) when combined with the [Paragraphs module](https://backdropcms.org/project/paragraphs) allow content authors to create cards using either the 'Card' or 'Cards' paragraph type.

![The edit screen to add a Paragraphs Aplenty card](img/card-paragraphs-aplenty.png)

### Creating Cards with Views

Coming soon

## Grids

Cards and other summary views are often displayed in grids. This theme uses the [Tailwind Grid system](https://tailwindcss.com/docs/grid-template-columns) along with some helper classes to create a 12 column grid. This allows grids and sections with 1, 2, 3, 4, 6 or 12 columns. These grids are responsive should collapse down on smaller screens.

### Creating a Grid with Views

The built in `Grid` views formatter works with the Decanter theme.

![Setting a grid](img/grid-view-edit.png)

### Spanning Columns in a Grid.

Adding the following classes to a grid item will cause it to span across columns. This can be used to create complex layouts:

- `.col-md-1`, `.col-span-1`
- `.col-md-2`, `.col-span-2`
- `.col-md-3`, `.col-span-3`, `.quarter-width`
- `.col-md-4`, `.col-span-4`, `.third-width`
- `.col-md-5`, `.col-span-5`
- `.col-md-6`, `.col-span-6`, `.third-width`
- `.col-md-7`, `.col-span-7`
- `.col-md-8`, `.col-span-8`, `.twothird-width`
- `.col-md-9`, `.col-span-9`, `.threequarter-width`
- `.col-md-10`, `.col-span-10`
- `.col-md-11`, `.col-span-11`
- `.col-md-12`, `.col-span-12`, `.full-width`

NB: The `col-md-*` have been kept for compatibility with older Bootstrap code. If possible, use the `.col-span-*` version for future compatibility.

## Utility Styles

Some other useful utility styles include:

- `.cta`: Turn any link into a round sided Call to Action button
- `.btn`: Turn a link into a square submit button
- `.link-arrow`: Add an animated internal link arrow to a link
- `.ext-link`: Add an animated external link arrow.
- `.gridded-region`: Turn a layout region into a responsive 12 column grid. NB: The 'Page Bottom' and 'Local Footer' regions already have this style applied.
- `.hero`: Turn any block or content into a Hero block. You can also create hero blocks by using the default 'Hero' content type.