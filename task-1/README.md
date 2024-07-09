Step-by-Step Guide to Build the Interactive List Component

1) Create and Configure ListComponent
Create a New Component (ListComponent.vue):
This component will handle displaying the list and navigation.

2) Define Props and Setup Component Structure:
In ListComponent.vue, define props for list (type: Array) and index (type: Number) using the Composition API.

3) Implement Computed Property for Styling:
Create a computed property that returns style settings, highlighting the item at the current index.

4) Template Setup with v-for and Slot:
Use the v-for directive to render each item and apply the computed styles.
Utilize slots to allow the parent component to define the content of each list item.

5) Add Navigation Buttons and Emit Index:
Include buttons to navigate to the previous and next items, and ensure that the new index is emitted to the parent component whenever it changes. This will allow the parent component to react to changes and update the displayed index accordingly.

6) Current Index Display:
Display the current index in the template to indicate which item is highlighted.

