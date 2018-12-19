# Final-Walk-Through

Step 1 Create DB

- Create the DB and enter data w/script https://github.com/byu-is-403/syllabus/blob/master/entity-framework/using-sql.md  

Step 2 Connect DB

- open the Web.config file
- Modify connection string

<connectionStrings>
    <add name="BasketballContext" connectionString="Data Source=(localDB)\v11.0;Initial Catalog=Basketball;Integrated Security=True;Connect Timeout=15;Encrypt=False;TrustServerCertificate=False"
      providerName="System.Data.SqlClient" />
  </connectionStrings>
