#Student-form
<!doctype html>
<html>
 <head>
  <h1 align="center">STUDENTS DETAIL</h1> 
  <script>
     function myfun()
     {
       var x=document.getElementById("R").value;
       var y=document.getElementById("N").value;
       var z=document.getElementById("E").value;
       if(x=="")
       {
         alert("Please fill your roll no");
         return;
       }
      else if(y=="")
       {
         alert("Please fill your name");
         return;
       }
      else if(z=="")
       {
         alert("Please fill your mail id");
         return;
       }
       else
       {
       var t= document.getElementById("mytable");
       var r=t.insertRow(-1);
       var c1=r.insertCell(0);
       var c2=r.insertCell(1);
       var c3=r.insertCell(2);
       c1.innerHTML=x;
       c2.innerHTML=y;
       c3.innerHTML=z;
       return;
       }
     }
   </script> 
   </head>
 <body text align="center">
  <table border="2" align="center" id="mytable"> 
   <tbody> 
    <tr> 
     <th>ROLL NO</th> 
     <th>NAME</th> 
     <th>MAIL ID</th> 
    </tr> 
   </tbody> 
  </table> 
  <form> 
   <br> 
   <br> 
   <br> 
   <br> 
   <br> 
   <br> 
   <p2>
     Roll No: 
   </p2> 
   <br> 
   <input type="text" id="R" name="rollno" placeholder="Enter your roll no" size="10"> 
   <br> 
   <br> 
   <p3>
     Name: 
    <br> 
    <input type="text" id="N" name="username" placeholder="Enter your name" size="20"> 
   </p3> 
   <br> 
   <br> 
   <p4>
     E-mail ID: 
    <br> 
    <input type="text" id="E" name="mail" placeholder="Enter your mail id" size="25"> 
   </p4> 
   <br> 
   <br> 
   <br> 
   <button type="button" onclick=" myfun();"> CLICK ME!&#128525</button> 
  </form> 
 </body>
</html>
