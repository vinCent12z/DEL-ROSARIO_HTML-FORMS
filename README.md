# DEL-ROSARIO_HTML-FORMS

html 

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Home Page</title>
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
    <title>Be our Speaker</title>
    <link rel="stylesheet" href="vincent.css"/>
</head>
<body>
    <header class="speaker-form-header">
        <h1>Speaker Submission</h1>

        <p>
            <em>Want to speak at our online conference? </em>
        </p>
    </header>

    <form action="" method="get" class="speaker-form">
        <div class='form-row'>
            <label for='full-name'>Name</label>
            <input id='full-name' name='full-name' type='text'/>
        </div>

        <div class='form-row'>
            <label for='email'>Email</label>
            <input id='email' name='email' type='email' placeholder='iskolar@pup.edu.ph'/>
        </div>

        <fieldset class='legacy-form-row'>
            <legend>Type of Talk</legend>
            <input id='seminar-type-1' name='seminar-type' type='radio' value='main-stage' checked/>
            <label for='seminar-type-1' class='radio-label'>Main Stage</label>

            <input id='seminar-type-2' name='seminar-type' type='radio' value='workshop'/>
            <label for='seminar-type-2' class='radio-label'>Workshop</label>
        </fieldset>

        <div class='form-row'>
            <label for='t-shirt'>T-Shirt Size</label>
            <select id='t-shirt' name='t-shirt'>
            <option value='xs'>Extra Small</option>
            <option value='s'>Small</option>
            <option value='m'>Medium</option>
            <option value='l'>Large</option>
            </select>
        </div>

        <div class='form-row'>
            <label for='abstract'>Abstract</label>
            <textarea id='abstract' name='abstract'></textarea>
            <div class='instructions'>Describe your talk in 500 words or less</div>
        </div>
           
        <div class='form-row'>
            <label class='checkbox-label' for='available'>
            <input id='available'
            name='available'
            type='checkbox'
            value='is-available'/>
            <span>Im actually available the date of the talk</span>
            </label>
        </div>
    </form>
</body>
</html>
=============================================================================================================================

vincent.css

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  
  body {
    color: #5D6063;
    background-color: #EAEDF0;
    font-family: "Helvetica", "Arial", sans-serif;
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
  
  .speaker-form {
    background-color: #F6F7F8;
    border: 1px solid #D6D9DC;
    border-radius: 3px;
  
    width: 80%;
    padding: 50px;
    margin: 0 0 40px 0;
  }
  
  .speaker-form-header h1 {
    font-size: 30px;
    margin-bottom: 20px;
  }
  
  .form-row {
    margin-bottom: 40px;
    display: flex;
    justify-content: flex-start;
    flex-direction: column;
    flex-wrap: wrap;
  }
  
  .form-row input[type='text'], 
  .form-row input[type='email'] {
    background-color: #FFFFFF;
    border: 1px solid #D6D9DC;
    border-radius: 3px;
    width: 100%;
    padding: 7px;
    font-size: 14px;
  }
  
  .form-row input[type='text']:invalid, 
  .form-row input[type='email']:invalid {
    border: 1px solid #D55C5F;
    color: #D55C5F;
    box-shadow: none;
  }
  
  .legacy-form-row {
    border: none;
    margin-bottom: 40px;
  }
  
  .legacy-form-row legend {
    margin-bottom: 15px;
  }
  
  .legacy-form-row .radio-label {
    display: block;
    font-size: 14px;
    padding: 0 20px 0 10px;
  }
  
  .legacy-form-row input[type='radio'] {
    margin-top: 2px;
  }
  
  .legacy-form-row .radio-label, 
  .legacy-form-row input[type='radio'] {
    float: left;
  }
  
  .form-row select {
    width: 100%;
    padding: 5px;
    font-size: 14px;
    -webkit-appearance: none;
  }
  
  .form-row textarea {
    font-family: "Helvetica", "Arial", sans-serif;
    font-size: 14px;
    border: 1px solid #D6D9DC;
    border-radius: 3px;
    min-height: 200px;
    margin-bottom: 10px;
    padding: 7px;
    resize: none;
  }
  
  .form-row .instructions {
    color: #999999;
    font-size: 14px;
    margin-bottom: 30px;
  }
   
  .form-row .checkbox-label {
    margin-bottom: 0;
  }
   
  
  @media only screen and (min-width: 700px) {
    .speaker-form-header,
    .speaker-form {
        width: 600px;
    }
  
    .form-row {
        flex-direction: row;
        align-items: flex-start;
        margin-bottom: 20px;
    }
  
    .form-row input[type='text'], 
    .form-row input[type='email'],
    .form-row select,
    .form-row textarea {
        width: 250px;
        height: initial;
    }
  
    .form-row label {
        text-align: right;
        width: 120px;
        margin-top: 7px;
        padding-right: 20px;
    }
  
    .legacy-form-row {
        margin-bottom: 10px;
    }
  
    .legacy-form-row legend {
        width: 120px;
        text-align: right;
        padding-right: 20px;
    }
  
    .legacy-form-row legend {
        float: left;
    }
  
    .form-row .instructions {
        margin-left: 120px;
    }
    
    .form-row .checkbox-label {
        margin-left: 120px;
        width: auto;
    }
  }
