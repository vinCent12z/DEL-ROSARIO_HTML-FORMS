# DEL-ROSARIO_HTML-FORMS

html 

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Website</title>
</head>
<body>
    <h1>Welcome to my Website</h1>
    <p><a href="speaker-submission.html">We are looking for a speaker, Join here!</a></p>
</body>
</html>
================================================================================================

speaker submission

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css"/>
    <title>Be our speaker.</title>
</head>
<body>
    <header class="speaker-form-header"><h1>Speaker Submission</h1><p>
        <em>
            Want to speaker to our conference? Fill out this form.
        </em>
    </p>
</header>

 <form action="" method="" class="speaker-form">
    ,<div class='form-row'><label for='full-name'> Name</label><input id='full-name' name='full-name' type='text'/></div>
 </form>

</body>
</html>
=============================================================================================================================

CSS

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    color: #5D6063;
    background-color: #EAEDF0;
    font-family: "Helvetica", "Arial" ,sans-serif;
    font-size: 16px;
    line-height: 1.3;

    display: flex;
    flex-direction: column;
    align-items: center;
}

.speaker-form-header {
    text-align: center;
    background-color: #F6F7F8;
    border: 1px solid #D6D9DC;
    border-radius: 3px;

    width: 80%;
    margin: 40px 0;
    padding: 50px;
}

.speaker-form-header h1 {
    font-size: 30px;
    margin-bottom: 20px;
}

.speaker-form {
    background-color: #F6F7F8;
    border: 1px solid #D6D9DC;
    border-radius: 3px;

    width: 80%;
    padding: 50px;
    margin: 0 0 40px 0;
}

.form-row {
    margin-bottom: 40px;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
}

.form-row input[type='text'] {
    background-color: #FFFFFF;
    border: 1px solid #D6D9DC;
    border-radius: 3px;
    width: 100%;
    padding: 7px;
    font-size: 14px;
}
.form-row LABEL {
    margin-bottom: 15px;
}

@media only screen and (min-width: 700px) {
    .speaker-form-header
    .speaker-form {
        width: 600px;
    }
}
.form-row {
    flex-direction: row;
    align-items: flex-start;
    margin-bottom: 20px;
}
.speaker-form input[type='text'] {
    width: 250px;
    height: initial;
}
.form-row label {
    text-align: right;
    width: 120px;
    margin-top: 7px;
    padding-right: 20px;
 }
