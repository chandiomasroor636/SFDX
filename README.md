# Salesforce Development Assignment

This repository contains the solution for the Salesforce Development Assignment, which involves creating a Lightning web component that interacts with an Apex controller to retrieve contact records and display them in a `lightning-datatable`.

## Step 1.1: Create an Apex Controller to Retrieve Contact Records

- Created an Apex class named `ContactController` with a method named `getContacts()`.
- Utilized SOQL query to fetch the desired fields (FirstName, LastName, Email) from the Contact object.

## Step 1.2: Create a Lightning Web Component to Display Contacts

- Created a Lightning web component named `contactList`.
- Designed the user interface using the `lightning-datatable` component to display fetched contact records.
- Defined columns (FirstName, LastName, Email) and set up a property to hold the data.

## Step 1.3: Implement Wire Service for Automated Data Retrieval

- Inside the `contactList` component, utilized the `@wire` adapter to wire the `getContacts()` method from the `ContactController` Apex class.
- Automatically called the Apex method and retrieved contact records.
- Handled the retrieved data and potential errors in the wired function.

## Step 1.4: Add the Component to a New App Page

- Passed the retrieved contact data to the `lightning-datatable` component and defined columns to display (FirstName, LastName, Email).
- Automatically rendered the table with contact records.
- This component can now be added to a Lightning App Page to visualize the contact records.

## Usage

1. Clone this repository to your local development environment.
2. Deploy the Apex class (`ContactController`) to your Salesforce org.
3. Deploy the Lightning web component (`contactList`) to your Salesforce org.
4. Create a Lightning App Page and add the `contactList` component to visualize contact records.



![image](https://github.com/chandiomasroor636/SFDX/assets/32571219/8aa25ac7-6e1c-498e-80e3-b533408acded)
