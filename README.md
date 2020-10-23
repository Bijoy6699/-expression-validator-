@@ -41,16 +41,10 @@ let v = new validator(postcode.value);

if(result == true){

 p.innerHTML = `
       <p class="alert alert-success">
            ${postcode.value} is valid !</p>  `;
 p.innerHTML = `<p class="alert alert-success">${postcode.value} is valid !</p>`;
}
else{
    p.innerHTML = `
            <p class="alert alert-danger">
            ${postcode.value} is invalid postcode 
    <b> ex-2314 </b>
    ! </p>`;
    p.innerHTML = `<p class="alert alert-danger"> ${postcode.value} is invalid postcode <b> ex-2314 </b> ! </p>`;
}}
  e.preventDefault();
});
@@ -64,13 +58,11 @@ form1.addEventListener('submit',e=>{
        result = k.test(email.value);
        if(result == true){

             alert1.innerHTML = `
            <p class="alert alert-success">
             alert1.innerHTML = `<p class="alert alert-success">
            ${email.value} is valid ! </p>`;
            }
            else{
             alert1.innerHTML = `
            <p class="alert alert-danger">
             alert1.innerHTML = `<p class="alert alert-danger">
            ${email.value} is invalid email
                <b>ex- someone111@gamil.com </b>
                !</p> `;
@@ -86,17 +78,14 @@ form2.addEventListener('submit',e=>{
        result = n.test(phone.value);
        if(result == true){

            alert2.innerHTML = `
            <p class="alert alert-success">
            alert2.innerHTML = `<p class="alert alert-success">
            ${phone.value} is valid ! </p>`;
            }
            else{

             alert2.innerHTML = `
            <p class="alert alert-danger">
             alert2.innerHTML = `<p class="alert alert-danger">
            ${phone.value} is invalid phone number
                <b>ex- 8801728412345 </b>
                ! </p>`;
                <b>ex- 8801728412345 </b>! </p>`;
    }}
     e.preventDefault();
});
