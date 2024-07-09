Goal:
You are tasked with creating a modal component named Modal.vue.

Requirements:
1) Create a modal component named Modal.vue.
2) The modal should have a prop called isModalAccepted.
3) Add two buttons to this modal: Accept and Decline.
4) Clicking 'Accept' should store the value true in local storage, and clicking 'Decline' should store false.
5) Display a <div> only if the modal is accepted: <div v-if="isModalAccepted">Display this div only if modal is accepted</div>.
6) If the modal is not accepted, an alert message should be displayed, stating that the user must accept the content.
7) If the user refreshes the page and has previously accepted the modal, the modal should not appear again.

Additional Notes:
1) Avoid using localStorage.getItem inside the App.vue component. Instead, handle this within the Modal.vue component.
2) Add event listeners to the Accept and Decline buttons, enabling them to be triggered by keyboard inputs. Use the 'a' key for Accept and the 'd' key for Decline.