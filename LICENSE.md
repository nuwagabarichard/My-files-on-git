<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Quiz</title>
    <style>
      body{background-color:skyblue;}
    </style>
</head>
<body>
  
    <h3>Quiz</h3>
    <h4>RICHGATES FOUNDATION QUIZ</h4>
    <h5><p>WHAT DOES RICHGATES FOUNDATION DEAL IN?</p></h5>
    <button onclick="checkAnswer('donates')">A. donates</button>
    <button onclick="checkAnswer('shows love')">B. shows love</button>
    <button onclick="checkAnswer('spreads love')">C. spreads love</button>

    <p id="quizResult"></p>

    <script>
        let score = 0;

        function checkAnswer(answer) {
            if (answer === 'spreads love') {
                score++;
                document.getElementById('quizResult').innerText = `Correct! Your score is: ${score}`;
            } else {
                document.getElementById('quizResult').innerText = `Wrong answer! Your score is: ${score}`;
            }
        }
    </script>
</body>
</html>
