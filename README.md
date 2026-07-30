Notes for UI5:

MVC -> Model view controller
mvc design pattern is a wiidely used architecture for developing software apps. in SAPUI5 Fiori, we follow this pattern to create applications that are scalable, modular and maintainable.

model -> data
view -> display UI 
controller -> business logic

<img width="504" height="332" alt="image" src="https://github.com/user-attachments/assets/3845b74b-5a84-48d9-89b6-9aeabfbd06a8" />

## 📌 Steps to Create a Model

1. **Create a new JSON model**
   ```javascript
   var oModel = new sap.ui.model.json.JSONModel();
   ```

2. **Load or set data**
   ```javascript
   oModel.setData(oData);
   // or
   oModel.loadData("model/data.json");
   ```

3. **Register the model**

   **Application Level**
   ```javascript
   sap.ui.getCore().setModel(oModel);
   ```

   **View Level**
   ```javascript
   this.getView().setModel(oModel);
   ```

   **Control Level**
   ```javascript
   this.getView().byId("idControl").setModel(oModel);
   ```

4. **Bind the model to controls**
