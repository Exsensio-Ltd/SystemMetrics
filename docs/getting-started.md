# Getting started
1. Add namespace:
  ```C#
  using OEESdk;
  ```
2. Create a property for the client and get the instance:
  ```C#
  private readonly OEEClient _oeeClient;
  ```
3. Get the instance of the client. By default the `GetInstance` method is using default Fiware url `http://localhost:1026` but it's possible to specify the custom url:
  ```C#
  _oeeClient = OEEClient.GetInstance();
  // or
  _oeeClient = OEEClient.GetInstance("http://153.34.42.73:1026");
  ```
4. use method `CreateEntityAsync` to create an entity of OEE metric:
  ```C#
  string breakTime = "01:00:00";
  string idealTime = "00:00:16.322";
  _oeeClient.CreateEntityAsync("Product Name", "Station Name", breakTime, idealTime));
  ```
