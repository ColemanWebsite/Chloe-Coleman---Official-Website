<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chloe Coleman - Official Website</title>
    <style>
        /* Alap dizájn */
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
        }

        nav {
            background-color: #333;
            color: white;
            padding: 10px;
            text-align: center;
        }

        nav a {
            color: white;
            padding: 10px;
            text-decoration: none;
        }

        nav a:hover {
            background-color: #575757;
        }

        #language-select {
            margin-left: 20px;
            padding: 5px;
        }

        .tab-content {
            display: none;
            margin-top: 20px;
        }

        .tab-content.active {
            display: block;
        }

        .movie-description {
            margin-top: 20px;
        }

        .movie-button {
            background-color: #4CAF50;
            color: white;
            padding: 10px;
            margin: 5px;
            border: none;
            cursor: pointer;
        }

        .movie-button:hover {
            background-color: #45a049;
        }

        .quiz-button {
            background-color: #4CAF50;
            color: white;
            padding: 10px;
            margin-top: 20px;
            border: none;
            cursor: pointer;
        }

        .quiz-button:hover {
            background-color: #45a049;
        }

        .quiz-container {
            margin-top: 20px;
        }

        .question {
            margin-bottom: 10px;
            background-color: rgba(0, 0, 0, 0.6); /* Átlátszó fekete háttér */
            color: white;
            padding: 10px;
            border-radius: 5px;
        }

        .comment {
            background-color: #f1f1f1;
            padding: 10px;
            margin: 5px 0;
        }

        /* Filmek megjelenítése */
        .movie-title {
            font-size: 20px;
            font-weight: bold;
            margin: 5px;
            cursor: pointer;
        }

        .movie-details {
            display: none;
            padding: 10px;
            background-color: #f4f4f4;
            border-radius: 5px;
            margin-top: 10px;
        }

        .movie-title:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>

<nav>
    <a href="#" onclick="showTab('home')">Home</a>
    <a href="#" onclick="showTab('movies')">Movies</a>
    <a href="#" onclick="showTab('quiz')">Quiz</a>
    <a href="#" onclick="showTab('comments')">Comments</a>
    <select id="language-select" onchange="changeLanguage()">
        <option value="en">English</option>
        <option value="hu">Hungarian</option>
        <option value="de">German</option>
        <option value="es">Spanish</option>
        <option value="ru">Russian</option>
    </select>
</nav>

<div id="home" class="tab-content active">
    <h1 id="home-title">Welcome to Chloe Coleman's Official Website</h1>
    <p id="home-text">Explore Chloe's movies, quizzes, and more!</p>
</div>

<div id="movies" class="tab-content">
    <h2 id="movies-title">Movies</h2>
    <div>
        <div class="movie-title" onclick="toggleMovieDetails('my-spy')">My Spy: The Eternal City</div>
        <div id="movie-my-spy" class="movie-details">
            <p><strong>My Spy: The Eternal City</strong></p>
            <p>This action-packed comedy follows a spy on a mission to protect a family...</p>
            <iframe src="https://www.youtube.com/embed/examplevideo" width="560" height="315"></iframe>
            <p><a href="https://example.com/watch-my-spy">Watch Now</a></p>
        </div>

        <div class="movie-title" onclick="toggleMovieDetails('gunpowder')">Gunpowder</div>
        <div id="movie-gunpowder" class="movie-details">
            <p><strong>Gunpowder</strong></p>
            <p>This historical drama tells the story of the Gunpowder Plot...</p>
            <iframe src="https://www.youtube.com/embed/examplevideo" width="560" height="315"></iframe>
            <p><a href="https://example.com/watch-gunpowder">Watch Now</a></p>
        </div>

        <div class="movie-title" onclick="toggleMovieDetails('big-time')">Big Time</div>
        <div id="movie-big-time" class="movie-details">
            <p><strong>Big Time</strong></p>
            <p>Chloe plays the role of a rising star in this dramatic tale...</p>
            <iframe src="https://www.youtube.com/embed/examplevideo" width="560" height="315"></iframe>
            <p><a href="https://example.com/watch-big-time">Watch Now</a></p>
        </div>

        <div class="movie-title" onclick="toggleMovieDetails('tv-show')">TV Show: A New Beginning</div>
        <div id="movie-tv-show" class="movie-details">
            <p><strong>TV Show: A New Beginning</strong></p>
            <p>A new series where Chloe plays a young detective...</p>
            <iframe src="https://www.youtube.com/embed/examplevideo" width="560" height="315"></iframe>
            <p><a href="https://example.com/watch-tv-show">Watch Now</a></p>
        </div>
    </div>
</div>

<div id="quiz" class="tab-content">
    <h2 id="quiz-title">Chloe Coleman Quiz</h2>
    <div class="quiz-container">
        <!-- Kvíz kérdések -->
        <div class="question">
            <p>1. When was Chloe Coleman born?</p>
            <input type="radio" name="q1" value="1999"> December 15, 1999<br>
            <input type="radio" name="q1" value="2008"> November 23, 2008<br>
            <input type="radio" name="q1" value="2000"> January 10, 2000<br>
        </div>
        <div class="question">
            <p>2. What is Chloe's most famous movie?</p>
            <input type="radio" name="q2" value="My Spy"> My Spy<br>
            <input type="radio" name="q2" value="Gunpowder"> Gunpowder<br>
            <input type="radio" name="q2" value="Big Time"> Big Time<br>
        </div>
        <div class="question">
            <p>3. In which year did Chloe star in 'My Spy'?</p>
            <input type="radio" name="q3" value="2018"> 2018<br>
            <input type="radio" name="q3" value="2020"> 2020<br>
            <input type="radio" name="q3" value="2019"> 2019<br>
        </div>
        <div class="question">
            <p>4. In which TV series did Chloe appear in 2021?</p>
            <input type="radio" name="q4" value="A New Beginning"> A New Beginning<br>
            <input type="radio" name="q4" value="The Detective"> The Detective<br>
            <input type="radio" name="q4" value="Spy Adventure"> Spy Adventure<br>
        </div>
        <div class="question">
            <p>5. What is Chloe's birthday?</p>
            <input type="radio" name="q5" value="December 15, 2008"> December 15, 2008<br>
            <input type="radio" name="q5" value="November 23, 2008"> November 23, 2008<br>
            <input type="radio" name="q5" value="January 10, 2008"> January 10, 2008<br>
        </div>
        <!-- További 5 kérdés hozzáadása -->
        <div class="question">
            <p>6. In which country was Chloe born?</p>
            <input type="radio" name="q6" value="USA"> USA<br>
            <input type="radio" name="q6" value="Canada"> Canada<br>
            <input type="radio" name="q6" value="UK"> UK<br>
        </div>
        <div class="question">
            <p>7. What was Chloe's first movie?</p>
            <input type="radio" name="q7" value="My Spy"> My Spy<br>
            <input type="radio" name="q7" value="Big Time"> Big Time<br>
            <input type="radio" name="q7" value="Gunpowder"> Gunpowder<br>
        </div>
        <div class="question">
            <p>8. Which genre does Chloe prefer for her roles?</p>
            <input type="radio" name="q8" value="Comedy"> Comedy<br>
            <input type="radio" name="q8" value="Drama"> Drama<br>
            <input type="radio" name="q8" value="Action"> Action<br>
        </div>
        <div class="question">
            <p>9. What is Chloe's favorite color?</p>
            <input type="radio" name="q9" value="Blue"> Blue<br>
            <input type="radio" name="q9" value="Red"> Red<br>
            <input type="radio" name="q9" value="Green"> Green<br>
        </div>
        <div class="question">
            <p>10. What kind of music does Chloe enjoy?</p>
            <input type="radio" name="q10" value="Pop"> Pop<br>
            <input type="radio" name="q10" value="Rock"> Rock<br>
            <input type="radio" name="q10" value="Jazz"> Jazz<br>
        </div>

        <button class="quiz-button" onclick="submitQuiz()">Submit</button>
    </div>
    <p id="quiz-result"></p>
</div>

<div id="comments" class="tab-content">
    <h2 id="comments-title">Comments</h2>
    <textarea id="comment-text" rows="4" cols="50"></textarea><br>
    <button onclick="submitComment()">Submit Comment</button>
    <div id="comments-list"></div>
</div>

<script>
    let language = 'en';

    function showTab(tabName) {
        const tabs = document.querySelectorAll('.tab-content');
        tabs.forEach(tab => tab.classList.remove('active'));
        document.getElementById(tabName).classList.add('active');
    }

    function changeLanguage() {
        const langSelect = document.getElementById('language-select');
        language = langSelect.value;
        updateText();
    }

    function updateText() {
        const translations = {
            en: {
                homeTitle: 'Welcome to Chloe Coleman\'s Official Website',
                homeText: 'Explore Chloe\'s movies, quizzes, and more!',
                moviesTitle: 'Movies',
                quizTitle: 'Chloe Coleman Quiz',
                commentsTitle: 'Comments',
                quizQuestions: {
                    q1: 'When was Chloe Coleman born?',
                    q2: 'What is Chloe\'s most famous movie?',
                    q3: 'In which year did Chloe star in \'My Spy\'?',
                    q4: 'In which TV series did Chloe appear in 2021?',
                    q5: 'What is Chloe\'s birthday?',
                    q6: 'In which country was Chloe born?',
                    q7: 'What was Chloe\'s first movie?',
                    q8: 'Which genre does Chloe prefer for her roles?',
                    q9: 'What is Chloe\'s favorite color?',
                    q10: 'What kind of music does Chloe enjoy?'
                }
            },
            hu: {
                homeTitle: 'Üdvözöljük Chloe Coleman hivatalos weboldalán',
                homeText: 'Fedezze fel Chloe filmjeit, kvízeit és még sok mást!',
                moviesTitle: 'Filmek',
                quizTitle: 'Chloe Coleman Kvíz',
                commentsTitle: 'Hozzászólások',
                quizQuestions: {
                    q1: 'Mikor született Chloe Coleman?',
                    q2: 'Mi Chloe legismertebb filmje?',
                    q3: 'Melyik évben szerepelt Chloe a "My Spy" filmben?',
                    q4: 'Melyik tévésorozatban szerepelt Chloe 2021-ben?',
                    q5: 'Mi Chloe születésnapja?',
                    q6: 'Melyik országban született Chloe?',
                    q7: 'Mi Chloe első filmje?',
                    q8: 'Milyen műfajt kedvel Chloe a szerepeiben?',
                    q9: 'Mi Chloe kedvenc színe?',
                    q10: 'Milyen zenét szeret Chloe?'
                }
            }
        };

        const selectedLanguage = translations[language];

        // Updating text content
        document.getElementById('home-title').innerText = selectedLanguage.homeTitle;
        document.getElementById('home-text').innerText = selectedLanguage.homeText;
        document.getElementById('movies-title').innerText = selectedLanguage.moviesTitle;
        document.getElementById('quiz-title').innerText = selectedLanguage.quizTitle;
        document.getElementById('comments-title').innerText = selectedLanguage.commentsTitle;

        // Update quiz questions
        document.querySelectorAll('.question').forEach((question, index) => {
            const questionNumber = index + 1;
            const questionText = selectedLanguage.quizQuestions[`q${questionNumber}`];
            question.querySelector('p').innerText = `${questionNumber}. ${questionText}`;
        });
    }

    function toggleMovieDetails(movieId) {
        const movieDetails = document.getElementById(`movie-${movieId}`);
        if (movieDetails.style.display === "none" || movieDetails.style.display === "") {
            movieDetails.style.display = "block";
        } else {
            movieDetails.style.display = "none";
        }
    }

    function submitQuiz() {
        let score = 0;
        const answers = {
            q1: '2008',
            q2: 'My Spy',
            q3: '2020',
            q4: 'A New Beginning',
            q5: 'November 23, 2008',
            q6: 'USA',
            q7: 'My Spy',
            q8: 'Comedy',
            q9: 'Blue',
            q10: 'Pop'
        };

        for (let question in answers) {
            const selectedAnswer = document.querySelector(`input[name="${question}"]:checked`);
            if (selectedAnswer && selectedAnswer.value === answers[question]) {
                score++;
            }
        }

        document.getElementById('quiz-result').innerText = `Your score: ${score} / 10`;
    }

    function submitComment() {
        const commentText = document.getElementById('comment-text').value;
        if (commentText) {
            const newComment = document.createElement('div');
            newComment.classList.add('comment');
            newComment.innerText = commentText;
            document.getElementById('comments-list').appendChild(newComment);
            document.getElementById('comment-text').value = '';
        }
    }

    // Initialize with the default language
    updateText();
</script>

</body>
</html>
