# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨


<!DOCTYPE html>
<html>
    <head>
        <title>Assignment week 2</title>
    </head>
    <body>
        <!--multimedia video-->
        <h1>Motivational Video</h1>
        <video width="640" height="360" controls autoplay muted loop poster="pexels-pixabay-ball.jpg">
            <source src="Cristiano Ronaldo Speeach of reach.mp4" type="video/mp4">
            <source src="video.webm" type="video/webm">
            Your browser does not support the video tag.
          </video>
          <br><br>

          <!--an orderedlist-->
          <h2>Football Legends</h2>
          <ol type="i">
            <li>Diego Maradona</li>
            <li>Johan Cruyff</li>
            <li>Zlatan Ibrahimovic</li>
            <li>Didier Drogba</li>
            <li>Paul Pogba</li>
          </ol>
          <br><br>
          <img src="pexels-pixabay-ball.jpg" width="350" height="300">
          <br><br>
          
          <!--creating a table-->
          <h3>A table of five contacts</h3>
          <table border="1">
            <thead>
                <tr>
                    <th>Name</th>
                    <th>Address</th>
                    <th>Mobile</th>
                    <th>Email</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Chris Wood</td>
                    <td>Kiganjo, Thika</td>
                    <td>0712345678</td>
                    <td>wood34@gmail.com</td>
                </tr>
                <tr>
                    <td>Anthony Elanga</td>
                    <td>masai lodge, Rongai</td>
                    <td>0798765433</td>
                    <td>anto234@gmail.com</td>
                </tr>
                <tr>
                    <td>David Raya</td>
                    <td>karen c, Langata</td>
                    <td>0723456784</td>
                    <td>davi2345@gmail.com</td>
                </tr>
                <tr>
                    <td>Marcus Rashford</td>
                    <td>makongeni, Thika</td>
                    <td>0798765435</td>
                    <td>Marcus23@gmail.com</td>
                </tr>
                <tr>
                    <td>Kevin De Bruyne</td>
                    <td>ngara, Nairobi</td>
                    <td>0745678934</td>
                    <td>kevin23@gmail.com</td>
                </tr>
            </tbody>
          </table>


        <!--registration form--> 
          <h4>Registration Form</h4>
          <form action="/submit" method="post">
            <label for="name">Full Name:</label>
            <br>
            <input type="text" id="name" name="name" placeholder="Enter your full name" required>
            <br><br>
            <label for="email">Email Address:</label>
            <br>
            <input type="email" id="email" name="email" placeholder="example@gmail.com" required>
            <br><br>
            <label for="password">Password:</label>
            <br>
            <input type="password" id="password" name="password" placeholder="Minimum 6 characters" minlength="6" required>
            <br><br>
            <label for="dob">Date of Birth:</label>
            <br>
            <input type="date" id="dob" name="dob" required>
            <br><br>
            <label for="country">Select Country:</label>
            <br>
            <select id="country" name="country" required>
              <option value="">--select your country--</option>
              <option value="usa">United States</option>
              <option value="uk">United Kingdom</option>
              <option value="canada">Canada</option>
              <option value="india">India</option>
            </select>
            <br><br>
        
            <label>Gender:</label><br>
            <input type="radio" id="male" name="gender" value="male" required>
            <label for="male">Male</label>
            <br>
            <input type="radio" id="female" name="gender" value="female" required>
            <label for="female">Female</label>
            <br>
            <input type="radio" id="other" name="gender" value="other" required>
            <label for="other">Other</label>
            <br><br>
            <label>Hobbies:</label>
            <br>
            <input type="checkbox" id="reading" name="hobbies" value="Reading">
            <label for="reading">Reading</label>
            <br>
            <input type="checkbox" id="sports" name="hobbies" value="Sports">
            <label for="sports">Sports</label>
            <br>
        
            <input type="checkbox" id="music" name="hobbies" value="Music">
            <label for="music">Music</label>
            <br><br>
            <input type="submit" value="Register">
            <input type="reset" value="Clear">
        
          </form>
    </body>
</html>
