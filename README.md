<!DOCTYPE html>
<html>
    <head>
        <title>Student Form</title>
    </head>
    <body>
        <!--Create a form to collect student data-->
        <form id="Student_Form">
            <input type='text' id='sname' name='student_name' placeholder="Enter Student Name" required/><br>
            <input type="text" id="regno" name="regno" placeholder="Enter Registration Number" required/><br>
            <input type="number" id="phone" name="phone" placeholder="Enter phone Number" required/><br>
            <input type="number" id="sem" name="sem" placeholder="Enter your current semester" required/><br>
            <button type="submit">Submit</button>
        </form>
        <script>
            var form = document.getElementById('Student_Form'); // Corrected the ID case
            form.addEventListener('submit', function(event) {
                event.preventDefault();
                alert('Form Submitted');
                form.reset();
            });
        </script>   
    </body>
</html>
