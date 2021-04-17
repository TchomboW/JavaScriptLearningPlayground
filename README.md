# JavaScriptLearningPlayground

<!DOCTYPE html>
<html>
  <head>
  </head>
  <body>
    
  <p>Usage of this and combination of class as an example how "this" is used </p>

  <p id = "demo777"></p>
  <p id = "demo778"></p>
  <p id = "demo779"></p>
   
    <script> 
    class LuxCars {
      constructor(carname, caryear, carmake, carmodel, carcolor){
        this.carname = carname; //making carname can be used by otehr ids
        this.caryear = caryear; //it also mean that carmake is universal that can used by other ids
        this.carmake = carmake; 
        this.carmodel = carmodel;
        this.carcolor = carcolor;
    }
    carAge() {
      let cardate = new Date();
      return cardate.getFullYear() -this.caryear;
    }
  }
  

    let Car1 = new LuxCars("Ford", 2020, "USA", "Mustang", "Bule"); //make a new value for car1 using the predefined this.
    document.getElementById("demo777").innerHTML = 
    Car1.carname + " " + 
    Car1.caryear + " " + 
    Car1.carmake + " " + 
    Car1.carmodel + " " + 
    Car1.carmodel + " " + 
    Car1.carcolor + " " + 
    Car1.carAge() + " " + "years old."; 

    let Car2 = new LuxCars("BMW", 2010, "Germany", "K45", "Silver");
    document.getElementById("demo778").innerHTML = 
    Car2.carname + " " + 
    Car2.caryear + " " + 
    Car2.carmake + " " + 
    Car2.carmodel + " " + 
    Car2.carcolor + " " + 
    Car2.carAge() + " " + "years old.";

    let Car3 = new LuxCars("Mercedes", 2021, "Germany", "S-class", "Black");
    document.getElementById("demo779").innerHTML =  
    Car3.carname + " " + 
    Car3.caryear + " " + 
    Car3.carmake + " " + 
    Car3.carmodel + " " + 
    Car3.carcolor + " " + 
    Car3.carAge() + " " + "years old.";
    
    </script>
    

  


  

  </body>





</html>
