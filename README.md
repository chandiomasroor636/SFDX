Step 1.1: Create an Apex controller that retrieves a list of contacts:

For this step created an Apex class named `ContactController` with a method named `getContacts()`. Use the SOQL query to fetch the desired fields (FirstName, LastName, Email) from the Contact object.

Step 1.2 : Create a Lightning web component that displays contacts in a table: 

Created a Lightning web component named `contactList`. Designed its user interface using the `lightning-datatable` component to display the fetched contact records. Defined the columns (FirstName, LastName, Email) and set up a property to hold the data.

Step 1.3: Wire the getContacts() method
 Inside the `contactList` component, used the `@wire` adapter to wire the `getContacts()` method from the `ContactController` Apex class. This will automatically call the Apex method and retrieve the contact records. Handle the retrieved data and any potential errors in the wired function.

Step 1.4: Add the component to a new App page
 Passed the retrieved contact data to the `lightning-datatable` component and define the columns to display (FirstName, LastName, Email). This will automatically render the table with the contact records.
This component can then be added to a Lightning App Page to visualize the contact records.
