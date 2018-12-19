# Final-Walk-Through

# Step 1 Create DB

- Create the DB and enter data w/script https://github.com/byu-is-403/syllabus/blob/master/entity-framework/using-sql.md  

# Step 2 Connect DB

- Open the Web.config file
- Copy connection string from that DB and paste into connection string

`
<connectionStrings>
    <add name="BasketballContext" connectionString="Data Source=(localDB)\v11.0;Initial Catalog=Basketball;Integrated Security=True;Connect Timeout=15;Encrypt=False;TrustServerCertificate=False"
      providerName="System.Data.SqlClient" />
  </connectionStrings>
`
  
# Create Models

`
using System;
using System.Collections.Generic;
using System.ComponentModel.DataAnnotations;
using System.ComponentModel.DataAnnotations.Schema;
using System.Linq;
using System.Web;

namespace PlayBall.Models
{
    [Table("Player")]
    public class Player
    {
        [Key]
        public int playerID { get; set; }
        public String playerLastName { get; set; }
        public String playerFirstName { get; set; }
        public String positionCode { get; set; }
        public String teamID { get; set; }
    }
}
`
