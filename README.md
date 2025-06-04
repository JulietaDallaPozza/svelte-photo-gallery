✨ Summary
This is a casual photo search app built in Svelte. It shows how to use:

Svelte's lifecycle hooks

Transitions for visual polish

API integration with a reactive interface


📦 Features
Reactive input for search queries

Unsplash API integration

Animated photo transitions (fly and fade)

Svelte lifecycle logging (onMount, onDestroy, etc.)

Clean layout with simple responsive styling

🔧 Imports and Setup
Lifecycle Hooks:

onMount, onDestroy, beforeUpdate, afterUpdate from Svelte

Transitions:

fade, fly from svelte/transition

Variables:

search_term: stores user input

photos: stores API response (photo list)

🔄 Lifecycle Hooks (Logging Only)
onMount: Fires once on component load → fetches default photos

onDestroy: Fires when the component is destroyed → logs a message

beforeUpdate: Fires before any DOM update → logs a message

afterUpdate: Fires after the DOM updates → logs a message

🌐 Data Fetching
fetchData():

Fetches from Unsplash using search_term (or defaults to "animals")

Updates the photos array with the results

🧑‍💻 User Interaction
handleFetch():

Triggered by button click

Calls fetchData() using the current search term

Clears the search input after fetching

🖼️ Rendering & Transitions
A search bar and button for user input

Image results rendered using {#each}

Each image:

Slides in (fly) with a staggered delay

Fades out (fade) on removal

🎨 Styling
Simple layout using flexbox

Responsive grid for images

Styled search input and fetch button

🧱 Additional Layout
Imported a custom Header component

Wrapped layout with a global app structure (<main>, <footer>)

Footer includes a link to SvelteKit docs