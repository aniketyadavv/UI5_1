## Application Details
|               |
| ------------- |
|**Generation Date and Time**<br>Sat Jul 18 2026 17:21:52 GMT+0000 (Coordinated Universal Time)|
|**App Generator**<br>SAP Fiori Application Generator|
|**App Generator Version**<br>1.28.0|
|**Generation Platform**<br>SAP Business Application Studio|
|**Template Used**<br>Basic V2|
|**Service Type**<br>OData URL|
|**Service URL**<br>https://services.odata.org/V3/Northwind/Northwind.svc|
|**Module Name**<br>zproject1|
|**Application Title**<br>Fiori Application |
|**Namespace**<br>com.sap|
|**UI5 Theme**<br>sap_horizon|
|**UI5 Version**<br>1.150.0|
|**Enable TypeScript**<br>False|
|**Add Eslint configuration**<br>True, see https://www.npmjs.com/package/@sap-ux/eslint-plugin-fiori-tools#rules for the eslint rules.|

## zproject1

An SAP Fiori application using northwing odata service.

### Starting the generated app

-   This app has been generated using the SAP Fiori tools - App Generator, as part of the SAP Fiori tools suite.  To launch the generated application, run the following from the generated application root folder:

```
    npm start
```

- It is also possible to run the application using mock data that reflects the OData Service URL supplied during application generation.  In order to run the application with Mock Data, run the following from the generated app root folder:

```
    npm run start-mock
```

#### Pre-requisites:

1. Active NodeJS LTS (Long Term Support) version and associated supported NPM version.  (See https://nodejs.org)

<br>

Were using UI5 Demo kit to generate the List Item. here's the code:
```
<List id="_IDGenList1"
		items="{/Customers}"
		headerText="Customers Details">
		    <ObjectListItem id="_IDGenObjectListItem"
			title="{CustomerID}"
			type="Active"
			press=".onListItemPress"
			number="{Phone}"
			numberUnit="{Fax}">
			<!-- <firstStatus>
				<ObjectStatus
					text="{Status}"
					state="{
						path: 'Status',
						formatter: '.formatter.status'
					}" />
			</firstStatus> -->
			<ObjectAttribute id="_IDGenObjectAttribute" text="{CompanyName} {ContactName}" />
			<ObjectAttribute id="_IDGenObjectAttribute1" text="{Address}, {City}, {PostalCode}, {Country}" />
		    </ObjectListItem>
	    </List>
```

UI5 control through Layout editor.
<img width="1836" height="872" alt="image" src="https://github.com/user-attachments/assets/d1158f8e-511c-41ef-9a03-b9b19c5a3bc1" />

