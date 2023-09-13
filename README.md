# CSS Explanation for Active Games Template

## Hosted Link
You can view the project live at [Active Games Template](https://saifulislam05.github.io/active-game-template/)

## Project Description
The "Active Games Template" is a web template that showcases a user dashboard for a gaming platform. It includes a sidebar with navigation items, user profile information, and a display of active games.

## HTML Structure

### Sidebar (`.sidebar`)
- The sidebar contains user information, navigation items, and a promotional section.
- User details, including an image, username, and membership status, are displayed at the top.
- Navigation items, such as "Streams," "Games," "New," and "Library," are arranged horizontally.
- A "Join pro for free games" section is provided with a call-to-action button.

### Right Side (`.right-side`)
- The right side of the template displays information about active games.
- It includes a heading, a status line, and a collection of game cards.

### Game Cards (`.card`)
- Each game card contains an image, game title, version, and a progress bar.
- The cards are arranged in a column with spacing between them.
- Hovering over a card triggers a slight scaling effect for user interactivity.

## Global Styles
- `*`: Applies reset styles to normalize margin, padding, and box-sizing for all elements.

### Main Container (`.main`)
- `.main`:
  - `height: 90vh;`: Sets the main container's height to 90% of the viewport height.
  - `width: 80%;`: Sets the main container's width to 80% of its parent.
  - `background: linear-gradient(...)`: Adds a gradient background to the main container.
  - `border-radius: 2rem;`: Rounds the container's corners.
  - `display: flex;`: Uses a flex layout for child elements.
#### Sidebar (`.sidebar`)
- `.sidebar`:
  - `display: flex;`: Sets the display property to flex for the sidebar container, allowing flexible layout and positioning of child elements.
  - `flex-direction: column;`: Defines the main axis of the flex container as a vertical column, stacking child elements vertically.
  - `align-items: center;`: Centers child elements vertically within the flex container.
  - `text-align: center;`: Aligns text content to the center horizontally, ensuring text elements are centered.
  - `background`: Creates a gradient background using the `linear-gradient` function, providing a visually appealing background with a gradient effect.
  - `border-radius: 2rem;`: Adds rounded corners to the sidebar, enhancing its visual design with rounded edges.

##### User Image (`.user img`)
- `.user img`:
  - `width` and `height`: Makes the user image a square of 120x120 pixels.
  - `border-radius: 50%;`: Rounds the image to a circle.

##### Navigation Items (`.nav-item`)
- `.nav-item`:
  - `display: flex;`: Arranges items horizontally.
  - `margin: 20% 0;`: Adds vertical spacing.
  - `align-items: center;`: Vertically centers content.
  - `justify-content: space-between;`: Spaces content evenly.
  - `cursor: pointer;`: Indicates interactivity.
  - `transition: .2s ease-in;`: Smooth hover effect.

##### Promotion Section (`.pro`)
- `.pro`:
  - `background: linear-gradient(...)`: Adds a gradient background.
  - `border-radius: 2rem;`: Rounds corners.
  - `color: white;`: Sets text color.
  - `padding: 1rem;`: Adds padding.
  - `position: relative;`: Positions element relative to the container.
  - `cursor: pointer;`: Indicates interactivity.
  - `transition: .5s ease;`: Smooth hover effect.

###### Promotion Image (`.pro img`)
- `.pro img`:
  - `position: absolute;`: Absolutely positions the image.
  - `top: -10%; right: 10%;`: Sets position relative to the parent.

### Right Side (`.right-side`)
- `.right-side`:
  - `flex: 2;`: Takes up more space.
  - `padding: 5%;`: Adds padding.

#### Status Section (`.status`)
- `.status`:
  - `margin-bottom: 48px;`: Adds bottom margin.

##### Status Heading (`.status h1`)
- `.status h1`:
  - `font-size: 3rem;`: Increases font size.

##### Status Line (`.status-line`)
- `.status-line`:
  - `width: 50%;`: Makes a horizontal line.
  - `background`: Adds a gradient background.
  - `border: none;`: Removes borders.
  - `padding: 0.5rem;`: Adds padding.
  - `border-radius: 2rem;`: Rounds corners.

#### Game Cards Section (`.cards`)
- `.cards`:
  - `height: 80%;`: Takes up 80% of the container.
  - `display: flex;`: Uses flex layout.
  - `flex-direction: column;`: Stacks cards vertically.
  - `justify-content: space-between;`: Spaces cards evenly.

##### Game Card (`.card`)
- `.card`:
  - `width: 100%;`: Uses full width.
  - `height: calc(...)`: Sets card height.
  - `padding: 4%;`: Adds padding.
  - `display: flex;`: Uses flex layout.
  - `background`: Adds a gradient background.
  - `border-radius: 1rem;`: Rounds corners.
  - `box-shadow: 6px 6px 20px ...;`: Adds a subtle shadow.
  - `cursor: pointer;`: Indicates interactivity.
  - `transition: .3s ease-out;`: Smooth hover effect.

###### Game Card Image (`.card img`)
- `.card img`:
  - `width: 80px; height: 80px;`: Sets image size.

###### Game Card Information (`.card-info`)
- `.card-info`:
  - `display: flex;`: Uses flex layout.
  - `flex-direction: column;`: Stacks content vertically.
  - `justify-content: space-between;`: Spaces content evenly.

- `.card-info h2`:
  - `font-size: larger;`: Increases font size.

- `.card-info p`:
  - `font-size: small;`: Sets a smaller font size.

###### Progress Bar (`.progress`)
- `.progress`:
  - `background: rgb(...);`: Sets the progress bar's background color.
  - `width: 100%;`: Spans full width.
  - `height: 25%;`: Sets bar height.
  - `margin-top: 4%;`: Adds top margin.
  - `position: relative;`: Positions relatively.
  - `overflow: hidden;`: Hides overflowing content.

- `.progress::after`:
  - `content: "";`: Adds pseudo-element for fill.
  - `position: absolute;`: Positions absolutely.
  - `width: 60%;`: Sets initial fill width.
  - `height: 100%;`: Covers full height.
  - `background: linear-gradient(...)`: Adds gradient fill.
  - `left: 0; top: 0;`: Positions at top-left.
  - `z-index: 2;`: Stacks above the background.

###### Percentage Text (`.percentage`)
- `.percentage`:
  - `font-weight: bold;`: Makes text bold.
  - `font-size: larger;`: Increases font size.
  - `background: linear-gradient(...)`: Adds gradient background.
  - `-webkit-background-clip: text;`: Clips background to text.
  - `-webkit-text-fill-color: transparent;`: Makes text color transparent.
