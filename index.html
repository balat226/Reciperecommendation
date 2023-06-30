<!DOCTYPE html>
<html>

<head>
  <title>Recipe Recommendation</title>
  <style>
    body {
      text-align: center;
      margin-top: 50px;
      font-family: Arial, sans-serif;
    }

    h1 {
      font-size: 24px;
      margin-bottom: 20px;
    }

    p {
      font-size: 18px;
      margin-bottom: 10px;
    }

    form {
      margin-bottom: 20px;
    }

    input[type="text"] {
      width: 300px;
      padding: 10px;
      margin: 5px;
    }

    button[type="submit"] {
      padding: 10px 20px;
      font-size: 16px;
    }

    #recommendation {
      margin-top: 20px;
      font-size: 18px;
      text-align: left;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    @media screen and (max-width: 480px) {
      input[type="text"] {
        width: 80%;
      }
    }
  </style>
</head>

<body>
  <h1>Get recipe recommendations based on the ingredients you have</h1>
  <p>Enter the ingredients you have and the cuisine for a recipe recommendation.</p>
  <form id="recipeForm">
    <input type="text" name="ingredient1" placeholder="Enter ingredient 1">
    <br>
    <input type="text" name="ingredient2" placeholder="Enter ingredient 2">
    <br>
    <input type="text" name="ingredient3" placeholder="Enter ingredient 3">
    <br>
    <input type="text" name="ingredient4" placeholder="Enter ingredient 4">
    <br>
    <input type="text" name="ingredient5" placeholder="Enter ingredient 5">
    <br>
    <input type="text" name="cuisine" placeholder="Enter the type of cuisine">
    <br>
    <br>
    <button type="submit">Submit</button>
  </form>
  <div id="recommendation">
  </div>
  <script>
    document.getElementById("recipeForm").addEventListener("submit", function (event) {
      event.preventDefault();

      var ingredients = [];
      var inputs = document.getElementsByTagName("input");
      for (var i = 0; i < inputs.length; i++) {
        if (inputs[i].value !== "") {
          ingredients.push(inputs[i].value);
        }
      }

      if (ingredients.length === 0) {
        alert("Please enter at least one ingredient.");
        return;
      }

      getRecipeRecommendation(ingredients);
    });

    function getRecipeRecommendation(ingredients) {
      var data = {
        "model": "gpt-3.5-turbo",
        "messages": [
          {
            "role": "user",
            "content": "Create a recipe using all of the following " + ingredients.join(" and ")
          }
        ]
      };

      fetch('https://api.openai.com/v1/chat/completions', {
        method: 'POST',
        headers: {
          'Content-Type': 'application/json',
          'Accept': 'application/json',
          'Authorization': 'Bearer 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'
        },
        body: JSON.stringify(data)
      })
        .then(response => response.json())
        .then(data => {
          var recommendation = data.choices[0].message.content;
          document.getElementById("recommendation").innerHTML = "<h2>Recipe Recommendation</h2><p>You may like:</p><p>" + recommendation + "</p>";

          // Clear input fields
          var inputs = document.getElementsByTagName("input");
          for (var i = 0; i < inputs.length; i++) {
            inputs[i].value = "";
          }
        })
        .catch(error => console.error(error));
    }
  </script>
</body>

</html>
