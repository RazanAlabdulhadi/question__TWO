# question__TWO

<html>
<main>
<div class="pagewrap">
    <form class="form" id="form">
      <h3 class="form__title">Sing Up Form Example</h3>
      
      <div class="container">
      
            <label id="userLabel1" for="fname" class="container__label">First,Last Name*</label> 
             <input class="container__input" type="text" id="fname" name="fname" value="" required> 
           <input class="container__input" type="text" id="Lname" name="Lname" value="" required> 
   
      </div>
      
      <div class="container">
        <label id="userLabel3" for="org" class="container__label">Organization</label>
        <input class="container__input" type="text" id="org" name="org" value="" >
        
      </div>
      <div class="container">
        <label id="userLabel4" for="org" class="container__label">Email Address*</label>
        <input class="container__input" type="text" id="Email" name="Email" value="" required>
       
      </div>
       <div class="container">
        <label id="userLabel5" for="WorkPhone" class="container__label">Work Phone</label>
        <input class="container__input" type="text" id="WorkPhone" name="WorkPhone" value="" >
       
      </div>
  
      <div class="container">
        <label id="userLabel6" for="HPhone" class="container__label">Home Phone</label>
        <input class="container__input" type="text" id="HPhone" name="HPhone" value="" >
       
      </div>
  
       <div class="container">
        <label id="userLabel7" for="CPhone" class="container__label">Cell Phone</label>
        <input class="container__input" type="text" id="CPhone" name="CPhone" value="" >
        
      </div>
  
      <div class="container">
        <label id="userLabel8" for="fax" class="container__label">Fax</label>
        <input class="container__input" type="text" id="fax" name="fax" value="" >
       
      </div>
  
      <div class="container">
        <label id="userLabel9" for="add1" class="container__label">Address 1*</label>
        <input class="container__input" type="text" id="add1" name="add1" value="" required>
        
      </div>
  
      <div class="container">
        <label id="userLabel10" for="add2" class="container__label">Address 2</label>
        <input class="container__input" type="text" id="add2" name="add2" value="" >
       
      </div>
  
      <div class="container">
          <label id="userLabel11" for="city" class="container__label">City* </label>
          <input class="container__input" type="text" id="city" name="city" value="" >
          
        </div>
  
        <div class="container">
          <label id="userLabel12" for="SP" class="container__label">State Provioce </label>
          <input class="container__input" type="text" id="SP" name="SP" value="" >
         
        </div>
  
        <div class="container">
          <label id="userLabel13" for="zippstel" class="container__label">zip postal Code </label>
          <input class="container__input" type="text" id="SP" name="zippstel" value="" >
          
        </div>
  
        <div class="container">
          <label id="userLabel14" for="Country" class="container__label">Country* </label>
          <input class="container__input" type="text" id="Country" name="Country" value="" required>
          
        </div>
  
        <div class="container">
            <label id="userLabel15" for="requiredlabel" class="container__label">*.required fields </label>
            <button class="form__submit" id="submit" type="button" value="submit">Submit</button>            
          </div>
        </table>
    </form>
  </div>
</main>


<style>

h3 {

    display:inline-flex;

}
    input[type=text], select {
      
      padding: 12px 20px;
      margin: 8px 0;
      display: inline-block;
      border: 1px solid #ccc;
      border-radius: 4px;
      box-sizing: border-box;
    }
    
    input[type=submit] {
      width: 100%;
      background-color: #4CAF50;
      color: white;
      padding: 10px 10px;
      margin: 8px 0;
      border: none;
      border-radius: 4px;
      cursor: pointer;
    }
    
    input[type=submit]:hover {
      background-color: #45a049;
    }
    
    div {
      border-radius: 5px;
      background-color: #f2f2f2;
      padding: 20px;
    }
    .button {
  position: relative;
  background-color: #4CAF50;
  border: none;
  font-size: 28px;
  color: #FFFFFF;
  padding: 20px;
  width: 200px;
  text-align: center;
  transition-duration: 0.4s;
  text-decoration: none;
  overflow: hidden;
  cursor: pointer;
}

.button:after {
  content: "";
  background: #f1f1f1;
  display: block;
  position: absolute;
  padding-top: 300%;
  padding-left: 350%;
  margin-left: -20px !important;
  margin-top: -120%;
  opacity: 0;
  transition: all 0.8s
}

.button:active:after {
  padding: 0;
  margin: 0;
  opacity: 1;
  transition: 0s
}

#submit {
  position: relative;
  background-color: #4f90f1;
  border: none;
  font-size: 20px;
  color: #FFFFFF;
  padding: 15px;
  width: 150px;
  text-align: center;
  transition-duration: 0.4s;
  text-decoration: none;
  overflow: hidden;
  cursor: pointer;
}

.button #submit  :after {
  content: "";
  background: #f1f1f1;
  display: block;
  position: absolute;
  padding-top: 300%;
  padding-left: 350%;
  margin-left: -20px !important;
  margin-top: -120%;
  opacity: 0;
  transition: all 0.8s
}

.button:active:after {
  padding: 0;
  margin: 0;
  opacity: 1;
  transition: 0s
}
form {
 margin-left: 440px;


}
h3{

    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    font-size:50px;
    font-style: oblique;
    font-display:inherit;
    
}
    </style>


<script>

function validate() {
  var fname = document.getElementById('fname').value;
  var Lname = document.getElementById('Lname').value;
  var address1 = document.getElementById('add1').value;
  var city = document.getElementById('city').value;
  var Country = document.getElementById('Country').value;

      
    if (fname === "" || fname === null) {
      alert("First Name required");               
    }
    if (Lname === "" || Lname === null) {
        alert("Last Name required");  
    }
    if (address1 === "" || address1 === null) {
        alert("address1 required");  
    }
    if (city === "" || city === null) {
        alert("city required");  
    }
    if (Country === "" || Country === null) {
        alert("Country required");  
    }
  }
  var submit = document.getElementById('submit');
  submit.addEventListener('click', validate);


</script>
