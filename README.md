<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Climate Guardians - Earth's Guide</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #e0f2fe;
            color: #1a202c;
            line-height: 1.6;
        }
        .container {
            max-width: 900px;
            margin: auto;
        }
        .card {
            background-color: #ffffff;
            border-radius: 1.5rem;
            box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
            padding: 2rem;
            margin-bottom: 2rem;
        }
        .header {
            background: linear-gradient(135deg, #38a169, #3182ce);
            color: white;
            padding: 2.5rem 1rem;
            border-bottom-left-radius: 2rem;
            border-bottom-right-radius: 2rem;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        .lesson-nav {
            background-color: #63b3ed;
            padding: 1rem;
            border-radius: 1rem;
            margin-top: -1rem;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 0.5rem;
        }
        .lesson-nav-btn {
            background-color: #ffffff;
            color: #1a202c;
            padding: 0.5rem 1rem;
            border-radius: 9999px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
        }
        .lesson-nav-btn:hover {
            background-color: #f0f0f0;
            transform: translateY(-2px);
        }
        .lesson-section {
            display: none;
        }
        .lesson-section.active {
            display: block;
        }
        .game-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
        }
        .game-card {
            background-color: #f0f9ff;
            border: 2px solid #90cdf4;
            border-radius: 1rem;
            padding: 1.5rem;
            text-align: center;
            transition: all 0.3s ease;
        }
        .game-card:hover {
            transform: translateY(-5px) scale(1.03);
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.1);
        }
        .game-btn {
            background-color: #4c51bf;
            color: white;
            padding: 0.75rem 1.5rem;
            border-radius: 9999px;
            font-weight: bold;
            text-decoration: none;
            transition: background-color 0.3s;
            display: inline-block;
            margin-top: 1rem;
        }
        .game-btn:hover {
            background-color: #3b429f;
        }
        .game-container {
            border: 2px solid #ccc;
            border-radius: 1rem;
            padding: 1rem;
            background-color: #f9fafb;
            min-height: 400px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
        }
        .game-message {
            margin-top: 1rem;
            font-weight: 600;
            color: #2b6cb0;
        }
        .game-option {
            background-color: #bee3f8;
            padding: 0.75rem 1.5rem;
            border-radius: 9999px;
            cursor: pointer;
            transition: all 0.2s ease;
            margin: 0.5rem;
        }
        .game-option:hover {
            background-color: #90cdf4;
            transform: scale(1.05);
        }
        .icon {
            font-size: 3rem;
        }
    </style>
</head>
<body class="bg-gray-100 font-sans">

    <header class="header text-center">
        <h1 class="text-4xl md:text-5xl font-extrabold mb-2">Climate Guardians</h1>
        <p class="text-lg md:text-xl font-medium">Your Guide to a Healthy Earth</p>
    </header>

    <div class="container p-4">
        
        <nav class="lesson-nav my-8">
            <a href="#" class="lesson-nav-btn" onclick="showLesson('lesson1')">Lesson 1</a>
            <a href="#" class="lesson-nav-btn" onclick="showLesson('lesson2')">Lesson 2</a>
            <a href="#" class="lesson-nav-btn" onclick="showLesson('lesson3')">Lesson 3</a>
            <a href="#" class="lesson-nav-btn" onclick="showLesson('lesson4')">Lesson 4</a>
            <a href="#" class="lesson-nav-btn" onclick="showLesson('lesson5')">Lesson 5</a>
        </nav>

        <div id="lesson1" class="lesson-section active">
            <div class="card">
                <h2 class="text-2xl font-bold mb-4 text-center text-blue-600">Lesson 1: Introduction to Weather and Climate</h2>
                <div class="prose max-w-none">
                    <h3 class="text-xl font-semibold mt-4">Weather vs. Climate</h3>
                    <p><strong>Weather</strong> is what the atmosphere is doing today. It’s what you see outside your window. For example, "Today in Guadalajara, it is sunny and warm."</p>
                    <p><strong>Climate</strong> is the average weather over many years. It's what you expect a place to be like. For example, "The climate in Baja California is usually dry and sunny."</p>
                    <h3 class="text-xl font-semibold mt-4">Basic Weather Words</h3>
                    <p>Let's learn some key words:</p>
                    <ul class="list-disc list-inside">
                        <li><strong>Temperature:</strong> How hot or cold it is.</li>
                        <li><strong>Precipitation:</strong> Rain, snow, or hail.</li>
                        <li><strong>Wind:</strong> The movement of air.</li>
                        <li><strong>Sunny:</strong> When the sun is shining.</li>
                        <li><strong>Cloudy:</strong> When there are a lot of clouds.</li>
                        <li><strong>Rainy:</strong> When it is raining.</li>
                        <li><strong>Windy:</strong> When the wind is blowing.</li>
                        <li><strong>Hot:</strong> High temperature.</li>
                        <li><strong>Cold:</strong> Low temperature.</li>
                    </ul>
                </div>
            </div>
            <div class="card">
                <h3 class="text-2xl font-bold mb-4 text-center text-blue-600">Games for Lesson 1</h3>
                <div class="game-grid">
                    <div class="game-card">
                        <h4 class="text-lg font-bold">Climate Trivia</h4>
                        <p>Test your knowledge with these questions!</p>
                        <button class="game-btn" onclick="startGame('trivia')">Play</button>
                    </div>
                    <div class="game-card">
                        <h4 class="text-lg font-bold">Memory Match</h4>
                        <p>Match weather words with their pictures.</p>
                        <button class="game-btn" onclick="startGame('memory')">Play</button>
                    </div>
                    <div class="game-card">
                        <h4 class="text-lg font-bold">Word Scramble</h4>
                        <p>Unscramble climate-related words.</p>
                        <button class="game-btn" onclick="startGame('scramble')">Play</button>
                    </div>
                    <div class="game-card">
                        <h4 class="text-lg font-bold">Fill in the Blanks</h4>
                        <p>Complete the sentences with the correct word.</p>
                        <button class="game-btn" onclick="startGame('fillblanks')">Play</button>
                    </div>
                </div>
            </div>
        </div>

        <div id="lesson2" class="lesson-section">
            <div class="card">
                <h2 class="text-2xl font-bold mb-4 text-center text-blue-600">Lesson 2: What is Climate Change?</h2>
                <div class="prose max-w-none">
                    <p><strong>Climate Change</strong> is a long-term change in the Earth's average weather patterns. The Earth is getting warmer, and this is affecting our planet.</p>
                    <h3 class="text-xl font-semibold mt-4">The Earth is Getting Warmer</h3>
                    <p>This is called <strong>Global Warming</strong>. The Earth's temperature is rising, which can melt ice and cause big problems for animals and plants.</p>
                    <h3 class="text-xl font-semibold mt-4">Ecosystems</h3>
                    <p>An <strong>ecosystem</strong> is a community of living things (plants, animals) and their environment. Climate change can harm ecosystems. For example, warmer oceans can damage coral reefs, which are homes for many fish.</p>
                </div>
            </div>
            <div class="card">
                <h3 class="text-2xl font-bold mb-4 text-center text-blue-600">Games for Lesson 2</h3>
                <div class="game-grid">
                    <div class="game-card">
                        <h4 class="text-lg font-bold">True or False</h4>
                        <p>Is the statement about climate change true or false?</p>
                        <button class="game-btn" onclick="startGame('truefalse')">Play</button>
                    </div>
                    <div class="game-card">
                        <h4 class="text-lg font-bold">Climate Challenge</h4>
                        <p>A simple clicker game to save the planet!</p>
                        <button class="game-btn" onclick="startGame('challenge')">Play</button>
                    </div>
                    <div class="game-card">
                        <h4 class="text-lg font-bold">The Climate Goose</h4>
                        <p>Roll the dice and land on climate-themed challenges.</p>
                        <button class="game-btn" onclick="startGame('goose')">Play</button>
                    </div>
                    <div class="game-card">
                        <h4 class="text-lg font-bold">Word Search</h4>
                        <p>Find hidden words related to climate change.</p>
                        <button class="game-btn" onclick="startGame('wordsearch')">Play</button>
                    </div>
                </div>
            </div>
        </div>

        <div id="lesson3" class="lesson-section">
            <div class="card">
                <h2 class="text-2xl font-bold mb-4 text-center text-blue-600">Lesson 3: Causes of Climate Change</h2>
                <div class="prose max-w-none">
                    <p>The main cause of climate change is the increase of <strong>greenhouse gases</strong> in the atmosphere. These gases trap heat and make the Earth warmer.</p>
                    <h3 class="text-xl font-semibold mt-4">Pollution</h3>
                    <p>Burning fossil fuels (like gas in cars and factories) releases a gas called carbon dioxide. This gas is a big part of the greenhouse effect. In big cities like Mexico City, you can sometimes see this pollution as smog.</p>
                    <h3 class="text-xl font-semibold mt-4">Human Activities</h3>
                    <p>Other things people do also cause climate change, like cutting down trees (<strong>deforestation</strong>). Trees absorb carbon dioxide, so when we cut them down, more of this gas stays in the air.</p>
                </div>
            </div>
            <div class="card">
                <h3 class="text-2xl font-bold mb-4 text-center text-blue-600">Games for Lesson 3</h3>
                <div class="game-grid">
                    <div class="game-card">
                        <h4 class="text-lg font-bold">Recycle & Earn</h4>
                        <p>Sort items into the right recycling bin to earn points!</p>
                        <button class="game-btn" onclick="startGame('recycle')">Play</button>
                    </div>
                    <div class="game-card">
                        <h4 class="text-lg font-bold">Climate Strategy</h4>
                        <p>Make choices to reduce CO2 emissions.</p>
                        <button class="game-btn" onclick="startGame('strategy')">Play</button>
                    </div>
                    <div class="game-card">
                        <h4 class="text-lg font-bold">Carbon Footprint Calculator</h4>
                        <p>Answer questions to see your carbon footprint.</p>
                        <button class="game-btn" onclick="startGame('carbon')">Play</button>
                    </div>
                    <div class="game-card">
                        <h4 class="text-lg font-bold">Ecosystem Builder</h4>
                        <p>Build a healthy ecosystem by choosing the right elements.</p>
                        <button class="game-btn" onclick="startGame('ecosystem')">Play</button>
                    </div>
                </div>
            </div>
        </div>

        <div id="lesson4" class="lesson-section">
            <div class="card">
                <h2 class="text-2xl font-bold mb-4 text-center text-blue-600">Lesson 4: Effects of Climate Change</h2>
                <div class="prose max-w-none">
                    <h3 class="text-xl font-semibold mt-4">Melting Ice</h3>
                    <p>As the Earth gets warmer, glaciers and ice sheets melt. This causes the sea level to rise, which can flood coastal areas and harm people and animals.</p>
                    <h3 class="text-xl font-semibold mt-4">Impact on Animals and Plants</h3>
                    <p>Climate change is changing the homes of animals and plants. For example, some animals, like the monarch butterfly, have their migration patterns affected. Other plants, like some cacti in Mexico, are also at risk.</p>
                </div>
            </div>
            <div class="card">
                <h3 class="text-2xl font-bold mb-4 text-center text-blue-600">Games for Lesson 4</h3>
                <div class="game-grid">
                    <div class="game-card">
                        <h4 class="text-lg font-bold">Extinction!</h4>
                        <p>A game to save endangered animals.</p>
                        <button class="game-btn" onclick="startGame('extinction')">Play</button>
                    </div>
                    <div class="game-card">
                        <h4 class="text-lg font-bold">Mission 1.5</h4>
                        <p>A quick reaction game to keep the temperature below 1.5°C.</p>
                        <button class="game-btn" onclick="startGame('mission')">Play</button>
                    </div>
                    <div class="game-card">
                        <h4 class="text-lg font-bold">Rising Sea</h4>
                        <p>Help people and animals escape from rising sea levels.</p>
                        <button class="game-btn" onclick="startGame('risingsea')">Play</button>
                    </div>
                    <div class="game-card">
                        <h4 class="text-lg font-bold">What's the Effect?</h4>
                        <p>Match the cause with the correct climate effect.</p>
                        <button class="game-btn" onclick="startGame('matcheffect')">Play</button>
                    </div>
                </div>
            </div>
        </div>

        <div id="lesson5" class="lesson-section">
            <div class="card">
                <h2 class="text-2xl font-bold mb-4 text-center text-blue-600">Lesson 5: Solutions to Climate Change</h2>
                <div class="prose max-w-none">
                    <h3 class="text-xl font-semibold mt-4">Simple Actions</h3>
                    <p>You can help fight climate change! Simple actions like saving energy, walking or biking instead of driving, and eating local food can make a big difference.</p>
                    <h3 class="text-xl font-semibold mt-4">Reduce, Reuse, Recycle</h3>
                    <p>Remember the 3 R's! By <strong>reducing</strong> what you buy, <strong>reusing</strong> items, and <strong>recycling</strong>, you can help reduce pollution and save our planet.</p>
                    <h3 class="text-xl font-semibold mt-4">Protecting Ecosystems</h3>
                    <p>We can help our planet by planting trees, saving water, and supporting farms that protect the environment.</p>
                </div>
            </div>
            <div class="card">
                <h3 class="text-2xl font-bold mb-4 text-center text-blue-600">Games for Lesson 5</h3>
                <div class="game-grid">
                    <div class="game-card">
                        <h4 class="text-lg font-bold">Bitoku Adventure</h4>
                        <p>Help a spirit of nature collect seeds and plant trees.</p>
                        <button class="game-btn" onclick="startGame('bitoku')">Play</button>
                    </div>
                    <div class="game-card">
                        <h4 class="text-lg font-bold">Climate Race</h4>
                        <p>Answer questions to advance in this game.</p>
                        <button class="game-btn" onclick="startGame('race')">Play</button>
                    </div>
                    <div class="game-card">
                        <h4 class="text-lg font-bold">Eco-Challenge</h4>
                        <p>Complete daily eco-friendly actions.</p>
                        <button class="game-btn" onclick="startGame('ecochallenge')">Play</button>
                    </div>
                    <div class="game-card">
                        <h4 class="text-lg font-bold">Design a Community</h4>
                        <p>Design a sustainable city in this fun simulation.</p>
                        <button class="game-btn" onclick="startGame('community')">Play</button>
                    </div>
                </div>
            </div>
        </div>

        <div id="game-modal" class="fixed inset-0 bg-black bg-opacity-50 z-50 flex justify-center items-center p-4" style="display: none;">
            <div class="card w-full max-w-2xl relative">
                <div class="flex justify-between items-center mb-4">
                    <h3 id="game-title" class="text-2xl font-bold text-blue-600"></h3>
                    <button class="text-gray-500 hover:text-gray-800 text-3xl font-bold" onclick="closeGame()">
                        &times;
                    </button>
                </div>
                <div id="game-content" class="game-container">
                    <p>The game will be here.</p>
                </div>
            </div>
        </div>
        
    </div>

    <script>
        // Data for games
        const gameData = {
            trivia: [
                { question: "What is the day-to-day condition of the atmosphere?", answer: "Weather", options: ["Weather", "Climate", "Temperature"] },
                { question: "What is the average weather over many years?", answer: "Climate", options: ["Weather", "Climate", "Wind"] },
                { question: "What measures how hot or cold it is?", answer: "Temperature", options: ["Precipitation", "Temperature", "Wind"] },
                { question: "What is the movement of air?", answer: "Wind", options: ["Rain", "Wind", "Clouds"] },
                { question: "What is the main gas causing climate change?", answer: "Carbon dioxide", options: ["Oxygen", "Nitrogen", "Carbon dioxide"] }
            ],
            truefalse: [
                { question: "The Earth is getting warmer.", answer: true },
                { question: "Climate change is only caused by natural things.", answer: false },
                { question: "Cutting down trees helps fight climate change.", answer: false },
                { question: "Recycling helps reduce pollution.", answer: true },
                { question: "Melting ice makes the sea level go down.", answer: false }
            ],
            recycle: [
                { item: "Plastic bottle", bin: "Recycle Bin" },
                { item: "Apple core", bin: "Trash Bin" },
                { item: "Glass jar", bin: "Recycle Bin" },
                { item: "Old newspaper", bin: "Recycle Bin" },
                { item: "Used napkin", bin: "Trash Bin" }
            ],
            memory: [
                "Sunny", "Sunny", "Cloudy", "Cloudy", "Rainy", "Rainy", "Windy", "Windy",
                "Hot", "Hot", "Cold", "Cold", "Snowy", "Snowy", "Stormy", "Stormy"
            ],
            scramble: [
                { word: "CLIMATE", hint: "The average weather over many years." },
                { word: "WEATHER", hint: "What the atmosphere is doing today." },
                { word: "POLLUTION", hint: "Harmful things in the environment." },
                { word: "RECYCLE", hint: "To turn old items into new ones." },
                { word: "ECOSYSTEM", hint: "A community of living things and their environment." }
            ],
            fillblanks: [
                { sentence: "The Earth is getting ___ because of climate change.", word: "warmer" },
                { sentence: "Burning fossil fuels releases ___ into the air.", word: "carbon dioxide" },
                { sentence: "Cutting down trees is called ___.", word: "deforestation" },
                { sentence: "The three R's are Reduce, Reuse, and ___.", word: "Recycle" }
            ],
            goose: [
                "Start", "Advance 1 space", "Answer a question", "Lose a turn", "Advance 2 spaces", "Answer a question", "Lose a turn", "Advance 1 space", "Answer a question", "Win"
            ],
            wordsearch: ["CLIMATE", "WEATHER", "POLLUTION", "ECOSYSTEM", "GLOBAL", "WARMING"],
            carbon: [
                { question: "How often do you walk or bike?", impact: 10, options: ["Daily", "Weekly", "Never"], score: [10, 5, 0] },
                { question: "Do you turn off lights when you leave a room?", impact: 5, options: ["Always", "Sometimes", "Never"], score: [5, 2, 0] },
                { question: "Do you recycle at home?", impact: 10, options: ["Yes", "No"], score: [10, 0] }
            ],
            risingsea: { start: 10, end: 1, timer: 30 },
            matcheffect: [
                { cause: "Burning fossil fuels", effect: "Increased greenhouse gases" },
                { cause: "Deforestation", effect: "Less CO2 absorbed by trees" },
                { cause: "Melting glaciers", effect: "Rising sea levels" },
                { cause: "Global warming", effect: "Damage to ecosystems" }
            ],
            ecochallenge: [
                { action: "Recycle plastic bottles", points: 10 },
                { action: "Turn off lights", points: 5 },
                { action: "Use a reusable water bottle", points: 15 },
                { action: "Plant a small plant", points: 20 }
            ]
        };

        // Current game state
        let currentGameState = null;
        let gooseGame = {
            player: 0,
            board: ["Start", "Goose", "Question", "Turn Lost", "Goose", "Question", "Turn Lost", "Goose", "Question", "Win"],
            questions: gameData.trivia
        };

        function showLesson(lessonId) {
            document.querySelectorAll('.lesson-section').forEach(section => {
                section.classList.remove('active');
            });
            document.getElementById(lessonId).classList.add('active');
        }

        function startGame(gameId) {
            const gameModal = document.getElementById('game-modal');
            const gameTitle = document.getElementById('game-title');
            const gameContent = document.getElementById('game-content');
            
            gameContent.innerHTML = '';
            currentGameState = {
                id: gameId,
                score: 0,
                questionIndex: 0,
                items: [],
                matches: 0,
                flippedCards: [],
                lockBoard: false
            };

            switch (gameId) {
                case 'trivia':
                    gameTitle.textContent = 'Climate Trivia';
                    setupTriviaGame();
                    break;
                case 'memory':
                    gameTitle.textContent = 'Memory Match';
                    setupMemoryGame();
                    break;
                case 'truefalse':
                    gameTitle.textContent = 'True or False';
                    setupTrueFalseGame();
                    break;
                case 'challenge':
                    gameTitle.textContent = 'Climate Challenge';
                    setupClimateChallenge();
                    break;
                case 'recycle':
                    gameTitle.textContent = 'Recycle & Earn';
                    setupRecycleGame();
                    break;
                case 'strategy':
                    gameTitle.textContent = 'Climate Strategy';
                    setupStrategyGame();
                    break;
                case 'extinction':
                    gameTitle.textContent = 'Extinction!';
                    setupExtinctionGame();
                    break;
                case 'mission':
                    gameTitle.textContent = 'Mission 1.5';
                    setupMissionGame();
                    break;
                case 'bitoku':
                    gameTitle.textContent = 'Bitoku Adventure';
                    setupBitokuGame();
                    break;
                case 'race':
                    gameTitle.textContent = 'Climate Race';
                    setupClimateRace();
                    break;
                case 'scramble':
                    gameTitle.textContent = 'Word Scramble';
                    setupScrambleGame();
                    break;
                case 'fillblanks':
                    gameTitle.textContent = 'Fill in the Blanks';
                    setupFillBlanksGame();
                    break;
                case 'goose':
                    gameTitle.textContent = 'The Climate Goose';
                    setupGooseGame();
                    break;
                case 'wordsearch':
                    gameTitle.textContent = 'Word Search';
                    setupWordSearchGame();
                    break;
                case 'carbon':
                    gameTitle.textContent = 'Carbon Footprint Calculator';
                    setupCarbonGame();
                    break;
                case 'ecosystem':
                    gameTitle.textContent = 'Ecosystem Builder';
                    setupEcosystemGame();
                    break;
                case 'risingsea':
                    gameTitle.textContent = 'Rising Sea';
                    setupRisingSeaGame();
                    break;
                case 'matcheffect':
                    gameTitle.textContent = "What's the Effect?";
                    setupMatchEffectGame();
                    break;
                case 'ecochallenge':
                    gameTitle.textContent = 'Eco-Challenge';
                    setupEcoChallengeGame();
                    break;
                case 'community':
                    gameTitle.textContent = 'Design a Community';
                    setupCommunityGame();
                    break;
            }
            gameModal.style.display = 'flex';
        }

        function closeGame() {
            document.getElementById('game-modal').style.display = 'none';
        }

        // --- Game Logic Functions ---

        // Trivia Game
        function setupTriviaGame() {
            const gameContent = document.getElementById('game-content');
            gameContent.innerHTML = `
                <div class="text-center">
                    <p id="trivia-question" class="text-xl font-semibold mb-4"></p>
                    <div id="trivia-options" class="flex flex-wrap justify-center"></div>
                    <p id="trivia-feedback" class="game-message"></p>
                    <p class="mt-4">Score: <span id="trivia-score">0</span> / ${gameData.trivia.length}</p>
                </div>
            `;
            displayTriviaQuestion();
        }

        function displayTriviaQuestion() {
            if (currentGameState.questionIndex >= gameData.trivia.length) {
                document.getElementById('trivia-question').textContent = "Game Over!";
                document.getElementById('trivia-options').innerHTML = `<p>Your final score is: ${currentGameState.score}/${gameData.trivia.length}</p>`;
                return;
            }
            const questionData = gameData.trivia[currentGameState.questionIndex];
            document.getElementById('trivia-question').textContent = questionData.question;
            const optionsContainer = document.getElementById('trivia-options');
            optionsContainer.innerHTML = '';
            questionData.options.forEach(option => {
                const button = document.createElement('button');
                button.textContent = option;
                button.className = 'game-option';
                button.onclick = () => checkTriviaAnswer(option, questionData.answer);
                optionsContainer.appendChild(button);
            });
            document.getElementById('trivia-feedback').textContent = '';
        }

        function checkTriviaAnswer(selected, correct) {
            const feedback = document.getElementById('trivia-feedback');
            if (selected === correct) {
                feedback.textContent = "Correct! Great job!";
                feedback.style.color = '#38a169';
                currentGameState.score++;
            } else {
                feedback.textContent = `Incorrect. The correct answer is: ${correct}`;
                feedback.style.color = '#e53e3e';
            }
            document.getElementById('trivia-score').textContent = currentGameState.score;
            currentGameState.questionIndex++;
            setTimeout(displayTriviaQuestion, 1500);
        }

        // Memory Game
        function setupMemoryGame() {
            const gameContent = document.getElementById('game-content');
            gameContent.innerHTML = `<div id="memory-board" class="grid grid-cols-4 gap-4"></div>`;
            
            const board = document.getElementById('memory-board');
            let shuffledCards = [...gameData.memory].sort(() => 0.5 - Math.random());
            
            shuffledCards.forEach(item => {
                const card = document.createElement('div');
                card.classList.add('memory-card', 'bg-blue-300', 'p-4', 'text-center', 'rounded-lg', 'cursor-pointer', 'text-white', 'font-bold', 'text-2xl', 'flex', 'items-center', 'justify-center');
                card.style.height = '100px';
                card.dataset.item = item;
                card.textContent = '?';
                card.onclick = () => flipCard(card);
                board.appendChild(card);
            });
        }

        function flipCard(card) {
            if (currentGameState.lockBoard || card === currentGameState.flippedCards[0] || card.textContent !== '?') return;

            card.textContent = card.dataset.item;
            card.classList.remove('bg-blue-300');
            card.classList.add('bg-blue-500');
            currentGameState.flippedCards.push(card);

            if (currentGameState.flippedCards.length === 2) {
                currentGameState.lockBoard = true;
                checkForMatch();
            }
        }

        function checkForMatch() {
            const [firstCard, secondCard] = currentGameState.flippedCards;
            if (firstCard.dataset.item === secondCard.dataset.item) {
                firstCard.classList.add('bg-green-500');
                secondCard.classList.add('bg-green-500');
                currentGameState.matches++;
                if (currentGameState.matches === gameData.memory.length / 2) {
                    setTimeout(() => {
                        document.getElementById('memory-board').innerHTML = '<p class="text-center font-bold text-xl">Congratulations, you found all the matches!</p>';
                    }, 1000);
                }
                resetBoard();
            } else {
                setTimeout(() => {
                    firstCard.textContent = '?';
                    secondCard.textContent = '?';
                    firstCard.classList.remove('bg-blue-500');
                    secondCard.classList.remove('bg-blue-500');
                    firstCard.classList.add('bg-blue-300');
                    secondCard.classList.add('bg-blue-300');
                    resetBoard();
                }, 1000);
            }
        }

        function resetBoard() {
            currentGameState.flippedCards = [];
            currentGameState.lockBoard = false;
        }

        // True or False Game
        function setupTrueFalseGame() {
            const gameContent = document.getElementById('game-content');
            gameContent.innerHTML = `
                <div class="text-center">
                    <p id="tf-statement" class="text-xl font-semibold mb-4"></p>
                    <div class="flex justify-center space-x-4">
                        <button class="game-option" onclick="checkTrueFalseAnswer(true)">True</button>
                        <button class="game-option" onclick="checkTrueFalseAnswer(false)">False</button>
                    </div>
                    <p id="tf-feedback" class="game-message"></p>
                    <p class="mt-4">Score: <span id="tf-score">0</span> / ${gameData.truefalse.length}</p>
                </div>
            `;
            displayTrueFalseQuestion();
        }

        function displayTrueFalseQuestion() {
            if (currentGameState.questionIndex >= gameData.truefalse.length) {
                document.getElementById('tf-statement').textContent = "Game Over!";
                document.getElementById('tf-feedback').innerHTML = `<p>Your final score is: ${currentGameState.score}/${gameData.truefalse.length}</p>`;
                return;
            }
            const statementData = gameData.truefalse[currentGameState.questionIndex];
            document.getElementById('tf-statement').textContent = statementData.question;
            document.getElementById('tf-feedback').textContent = '';
        }

        function checkTrueFalseAnswer(selected) {
            const feedback = document.getElementById('tf-feedback');
            const statementData = gameData.truefalse[currentGameState.questionIndex];
            if (selected === statementData.answer) {
                feedback.textContent = "Correct! You got it right!";
                feedback.style.color = '#38a169';
                currentGameState.score++;
            } else {
                feedback.textContent = `Incorrect. The correct answer is: ${statementData.answer ? 'True' : 'False'}`;
                feedback.style.color = '#e53e3e';
            }
            document.getElementById('tf-score').textContent = currentGameState.score;
            currentGameState.questionIndex++;
            setTimeout(displayTrueFalseQuestion, 1500);
        }

        // Climate Challenge
        function setupClimateChallenge() {
            const gameContent = document.getElementById('game-content');
            gameContent.innerHTML = `
                <div class="text-center">
                    <p class="text-xl font-semibold mb-4">Click the clouds to reduce CO2!</p>
                    <div id="climate-target" class="text-6xl mb-4">☀️</div>
                    <p class="mb-4">CO2 Level: <span id="co2-level">100</span>%</p>
                    <button id="click-btn" class="game-btn">Click to Clean!</button>
                    <p id="challenge-message" class="game-message mt-4"></p>
                </div>
            `;
            const clickBtn = document.getElementById('click-btn');
            const co2LevelSpan = document.getElementById('co2-level');
            const message = document.getElementById('challenge-message');
            let co2Level = 100;
            let interval = setInterval(() => {
                co2Level += 1;
                co2LevelSpan.textContent = co2Level;
                if (co2Level >= 150) {
                    message.textContent = "The air is too polluted! Game over!";
                    message.style.color = '#e53e3e';
                    clickBtn.disabled = true;
                    clearInterval(interval);
                }
            }, 1000);

            clickBtn.onclick = () => {
                if (co2Level > 0) {
                    co2Level -= 10;
                    if (co2Level < 0) co2Level = 0;
                    co2LevelSpan.textContent = co2Level;
                    if (co2Level === 0) {
                        message.textContent = "You cleaned the air! Congratulations!";
                        message.style.color = '#38a169';
                        clickBtn.disabled = true;
                        clearInterval(interval);
                    }
                }
            };
        }

        // Recycle & Earn Game
        function setupRecycleGame() {
            const gameContent = document.getElementById('game-content');
            gameContent.innerHTML = `
                <div class="text-center">
                    <p class="text-xl font-semibold mb-4">Drag and drop the items into the correct bin!</p>
                    <p class="mb-4">Score: <span id="recycle-score">0</span></p>
                    <div id="recycle-bins" class="flex justify-center space-x-8 mt-8">
                        <div id="Recycle Bin" class="w-32 h-40 bg-green-500 rounded-lg flex items-center justify-center text-white font-bold text-lg" ondrop="drop(event)" ondragover="allowDrop(event)">
                            Recycle
                        </div>
                        <div id="Trash Bin" class="w-32 h-40 bg-red-500 rounded-lg flex items-center justify-center text-white font-bold text-lg" ondrop="drop(event)" ondragover="allowDrop(event)">
                            Trash
                        </div>
                    </div>
                    <div id="item-to-drag" class="mt-8">
                        <p id="drag-item-text" class="text-3xl p-4 bg-gray-200 rounded-lg cursor-grab" draggable="true" ondragstart="drag(event)"></p>
                    </div>
                    <p id="recycle-message" class="game-message mt-4"></p>
                </div>
            `;
            currentGameState.items = [...gameData.recycle];
            shuffleArray(currentGameState.items);
            displayRecycleItem();
        }

        function allowDrop(event) {
            event.preventDefault();
        }

        function drag(event) {
            event.dataTransfer.setData("text", event.target.textContent);
        }

        function drop(event) {
            event.preventDefault();
            const data = event.dataTransfer.getData("text");
            const draggedItem = gameData.recycle.find(item => item.item === data);
            const targetBin = event.target.id;
            const message = document.getElementById('recycle-message');

            if (draggedItem && draggedItem.bin === targetBin) {
                currentGameState.score += 10;
                message.textContent = 'Correct! +10 points';
                message.style.color = '#38a169';
            } else {
                message.textContent = 'Incorrect. Try again.';
                message.style.color = '#e53e3e';
            }
            document.getElementById('recycle-score').textContent = currentGameState.score;
            currentGameState.items.shift();
            setTimeout(displayRecycleItem, 1000);
        }

        function displayRecycleItem() {
            const itemText = document.getElementById('drag-item-text');
            if (currentGameState.items.length > 0) {
                itemText.textContent = currentGameState.items[0].item;
            } else {
                itemText.textContent = "Game Over!";
                document.getElementById('recycle-bins').style.display = 'none';
                itemText.draggable = false;
                document.getElementById('recycle-message').textContent = `Your final score is: ${currentGameState.score}`;
            }
        }

        // Strategy Game
        function setupStrategyGame() {
            const gameContent = document.getElementById('game-content');
            gameContent.innerHTML = `
                <div class="text-center">
                    <p class="text-xl font-semibold mb-4">Make a choice to reduce CO2 emissions!</p>
                    <p class="mb-4">CO2 Level: <span id="strategy-co2">100</span>%</p>
                    <div id="strategy-choices" class="flex flex-col space-y-4"></div>
                    <p id="strategy-message" class="game-message mt-4"></p>
                </div>
            `;
            currentGameState.co2 = 100;
            displayStrategyChoices();
        }

        function displayStrategyChoices() {
            const choicesContainer = document.getElementById('strategy-choices');
            const choices = [
                { text: "Walk instead of using the car.", reduction: 10 },
                { text: "Turn off the lights when you leave a room.", reduction: 5 },
                { text: "Use a reusable bag at the store.", reduction: 3 },
            ];
            choicesContainer.innerHTML = '';
            choices.forEach(choice => {
                const btn = document.createElement('button');
                btn.textContent = choice.text;
                btn.className = 'game-option';
                btn.onclick = () => selectStrategy(choice.reduction);
                choicesContainer.appendChild(btn);
            });
            document.getElementById('strategy-message').textContent = '';
        }

        function selectStrategy(reduction) {
            currentGameState.co2 -= reduction;
            if (currentGameState.co2 < 0) currentGameState.co2 = 0;
            document.getElementById('strategy-co2').textContent = currentGameState.co2;
            const message = document.getElementById('strategy-message');
            message.textContent = `You reduced CO2 by ${reduction} points!`;
            message.style.color = '#38a169';
            
            if (currentGameState.co2 <= 50) {
                 message.textContent = `You've reduced CO2 to a safe level! Congratulations!`;
                 document.getElementById('strategy-choices').innerHTML = '';
            }
        }

        // Extinction Game
        function setupExtinctionGame() {
            const gameContent = document.getElementById('game-content');
            const animals = ["🦥", "🐼", "🐻‍❄️", "🦋", "🦧"];
            gameContent.innerHTML = `
                <div class="text-center">
                    <p class="text-xl font-semibold mb-4">Click the animals to save them!</p>
                    <div id="animal-container" class="relative w-full h-80 border-2 border-gray-400 rounded-lg"></div>
                    <p id="extinction-message" class="game-message mt-4"></p>
                    <p>Animals Saved: <span id="animals-saved">0</span> / 5</p>
                </div>
            `;
            const container = document.getElementById('animal-container');
            let savedCount = 0;
            const savedSpan = document.getElementById('animals-saved');

            animals.forEach(animal => {
                const animalDiv = document.createElement('div');
                animalDiv.textContent = animal;
                animalDiv.className = 'absolute text-3xl cursor-pointer transition-all duration-300 transform';
                animalDiv.style.left = `${Math.random() * 90}%`;
                animalDiv.style.top = `${Math.random() * 90}%`;
                animalDiv.onclick = () => {
                    if (animalDiv.style.display !== 'none') {
                        animalDiv.style.display = 'none';
                        savedCount++;
                        savedSpan.textContent = savedCount;
                        if (savedCount === animals.length) {
                            document.getElementById('extinction-message').textContent = 'You saved all the animals! Victory!';
                            document.getElementById('extinction-message').style.color = '#38a169';
                        }
                    }
                };
                container.appendChild(animalDiv);
            });
        }

        // Mission 1.5 Game
        function setupMissionGame() {
            const gameContent = document.getElementById('game-content');
            gameContent.innerHTML = `
                <div class="text-center">
                    <p class="text-xl font-semibold mb-4">Stop the meter before it reaches 1.5°C!</p>
                    <div class="relative w-64 h-8 bg-gray-300 rounded-full mx-auto">
                        <div id="temp-bar" class="absolute h-8 bg-red-500 rounded-full transition-all duration-100 ease-linear" style="width: 0%;"></div>
                    </div>
                    <p class="text-lg mt-2"><span id="temp-reading">0</span>°C</p>
                    <button class="game-btn mt-4" onclick="stopTemp()">STOP</button>
                    <p id="mission-message" class="game-message mt-4"></p>
                </div>
            `;
            let temp = 0;
            const tempBar = document.getElementById('temp-bar');
            const tempReading = document.getElementById('temp-reading');
            let interval = setInterval(() => {
                temp += 0.1;
                tempBar.style.width = `${(temp / 2) * 100}%`;
                tempReading.textContent = temp.toFixed(1);
                if (temp >= 1.5) {
                    clearInterval(interval);
                    document.getElementById('mission-message').textContent = 'Oh no! The temperature went over 1.5°C. Try again!';
                    document.getElementById('mission-message').style.color = '#e53e3e';
                }
            }, 100);
            window.stopTemp = () => {
                clearInterval(interval);
                if (temp < 1.5) {
                    document.getElementById('mission-message').textContent = `You did it! You kept the temperature at ${temp.toFixed(1)}°C.`;
                    document.getElementById('mission-message').style.color = '#38a169';
                }
            };
        }
        
        // Bitoku Game
        function setupBitokuGame() {
            const gameContent = document.getElementById('game-content');
            gameContent.innerHTML = `
                <div class="text-center">
                    <p class="text-xl font-semibold mb-4">Help Bitoku collect seeds!</p>
                    <div id="bitoku-container" class="relative w-full h-80 border-2 border-gray-400 rounded-lg overflow-hidden">
                        <div id="bitoku-player" class="absolute text-3xl">🌿</div>
                        <p class="absolute top-2 left-2 font-bold">Seeds: <span id="bitoku-seeds">0</span></p>
                    </div>
                </div>
            `;
            const player = document.getElementById('bitoku-player');
            const container = document.getElementById('bitoku-container');
            const seedsSpan = document.getElementById('bitoku-seeds');
            
            let seeds = 0;
            let playerX = container.offsetWidth / 2;
            let playerY = container.offsetHeight / 2;

            function updatePlayerPosition() {
                player.style.left = `${playerX}px`;
                player.style.top = `${playerY}px`;
            }

            function createSeed() {
                const seed = document.createElement('div');
                seed.textContent = '🌰';
                seed.className = 'absolute text-lg cursor-pointer seed';
                seed.style.left = `${Math.random() * (container.offsetWidth - 20)}px`;
                seed.style.top = `${Math.random() * (container.offsetHeight - 20)}px`;
                seed.onclick = () => {
                    seed.remove();
                    seeds++;
                    seedsSpan.textContent = seeds;
                    if (seeds % 5 === 0) {
                        spawnTree();
                    }
                    createSeed();
                };
                container.appendChild(seed);
            }

            function spawnTree() {
                const tree = document.createElement('div');
                tree.textContent = '🌳';
                tree.className = 'absolute text-4xl';
                tree.style.left = `${Math.random() * (container.offsetWidth - 40)}px`;
                tree.style.top = `${Math.random() * (container.offsetHeight - 40)}px`;
                container.appendChild(tree);
            }
            
            for(let i = 0; i < 5; i++) {
                createSeed();
            }

            document.addEventListener('keydown', (e) => {
                const step = 10;
                if (e.key === 'ArrowUp' && playerY > 0) playerY -= step;
                if (e.key === 'ArrowDown' && playerY < container.offsetHeight - 30) playerY += step;
                if (e.key === 'ArrowLeft' && playerX > 0) playerX -= step;
                if (e.key === 'ArrowRight' && playerX < container.offsetWidth - 30) playerX += step;
                updatePlayerPosition();
            });

            // Touch controls
            let touchStartX = 0;
            let touchStartY = 0;
            container.addEventListener('touchstart', (e) => {
                touchStartX = e.touches[0].clientX;
                touchStartY = e.touches[0].clientY;
            });
            container.addEventListener('touchmove', (e) => {
                e.preventDefault();
                const touchEndX = e.touches[0].clientX;
                const touchEndY = e.touches[0].clientY;
                const dx = touchEndX - touchStartX;
                const dy = touchEndY - touchStartY;
                const step = 10;
                if (Math.abs(dx) > Math.abs(dy)) {
                    if (dx > 0 && playerX < container.offsetWidth - 30) playerX += step;
                    if (dx < 0 && playerX > 0) playerX -= step;
                } else {
                    if (dy > 0 && playerY < container.offsetHeight - 30) playerY += step;
                    if (dy < 0 && playerY > 0) playerY -= step;
                }
                updatePlayerPosition();
            });
            updatePlayerPosition();
        }

        // Climate Race Game
        function setupClimateRace() {
            const gameContent = document.getElementById('game-content');
            gameContent.innerHTML = `
                <div class="text-center">
                    <p class="text-xl font-semibold mb-4">Answer questions to win the Climate Race!</p>
                    <p class="mb-4">You are at space: <span id="race-position">1</span> / 10</p>
                    <div id="race-question-container"></div>
                </div>
            `;
            currentGameState.position = 1;
            displayRaceQuestion();
        }

        function displayRaceQuestion() {
            if (currentGameState.position > 10) {
                document.getElementById('race-question-container').innerHTML = '<p class="font-bold text-xl">Congratulations, you won the race!</p>';
                return;
            }
            const allQuestions = [...gameData.trivia, ...gameData.truefalse.map(q => ({ question: q.question, answer: q.answer ? 'True' : 'False', options: ['True', 'False'] }))];
            const questions = shuffleArray(allQuestions);
            const questionData = questions[0];
            const container = document.getElementById('race-question-container');
            container.innerHTML = `
                <p class="mb-4 text-lg">${questionData.question}</p>
                <div class="flex justify-center space-x-4">
                    ${questionData.options ? questionData.options.map(opt => `<button class="game-option" onclick="checkRaceAnswer('${opt}', '${questionData.answer}')">${opt}</button>`).join('') :
                        `<button class="game-option" onclick="checkRaceAnswer('true', 'True')">True</button><button class="game-option" onclick="checkRaceAnswer('false', 'False')">False</button>`
                    }
                </div>
            `;
        }
        
        function checkRaceAnswer(selected, correct) {
            let isCorrect = selected === correct;

            if (isCorrect) {
                currentGameState.position++;
                document.getElementById('race-position').textContent = currentGameState.position;
                document.getElementById('race-question-container').innerHTML = `<p class="game-message text-green-600">Correct! You advance one space.</p>`;
            } else {
                document.getElementById('race-question-container').innerHTML = `<p class="game-message text-red-600">Incorrect. You lose a turn.</p>`;
            }
            setTimeout(displayRaceQuestion, 1500);
        }

        // Word Scramble Game
        function setupScrambleGame() {
            const gameContent = document.getElementById('game-content');
            gameContent.innerHTML = `
                <div class="text-center">
                    <p class="text-xl font-semibold mb-4">Unscramble the word!</p>
                    <p id="scrambled-word" class="text-4xl font-bold mb-4"></p>
                    <p id="scramble-hint" class="text-sm text-gray-600 mb-4"></p>
                    <input type="text" id="scramble-input" class="p-2 border rounded-md text-center" placeholder="Enter your word">
                    <button class="game-btn mt-4" onclick="checkScrambleAnswer()">Check</button>
                    <p id="scramble-message" class="game-message mt-4"></p>
                    <p class="mt-4">Score: <span id="scramble-score">0</span></p>
                </div>
            `;
            currentGameState.scrambleIndex = 0;
            currentGameState.score = 0;
            displayScrambleWord();
        }

        function displayScrambleWord() {
            if (currentGameState.scrambleIndex >= gameData.scramble.length) {
                document.getElementById('scramble-message').textContent = `Game over! Final score: ${currentGameState.score}`;
                return;
            }
            const wordData = gameData.scramble[currentGameState.scrambleIndex];
            const scrambled = wordData.word.split('').sort(() => 0.5 - Math.random()).join('');
            document.getElementById('scrambled-word').textContent = scrambled.toUpperCase();
            document.getElementById('scramble-hint').textContent = `Hint: ${wordData.hint}`;
            document.getElementById('scramble-input').value = '';
            document.getElementById('scramble-message').textContent = '';
        }

        function checkScrambleAnswer() {
            const input = document.getElementById('scramble-input').value.toUpperCase();
            const correctWord = gameData.scramble[currentGameState.scrambleIndex].word.toUpperCase();
            const message = document.getElementById('scramble-message');

            if (input === correctWord) {
                message.textContent = 'Correct! Good job!';
                message.style.color = '#38a169';
                currentGameState.score += 10;
                document.getElementById('scramble-score').textContent = currentGameState.score;
                currentGameState.scrambleIndex++;
                setTimeout(displayScrambleWord, 1500);
            } else {
                message.textContent = 'Incorrect. Try again.';
                message.style.color = '#e53e3e';
            }
        }

        // Fill in the Blanks Game
        function setupFillBlanksGame() {
            const gameContent = document.getElementById('game-content');
            gameContent.innerHTML = `
                <div class="text-center">
                    <p class="text-xl font-semibold mb-4">Fill in the missing word!</p>
                    <p id="blanks-sentence" class="text-lg mb-4"></p>
                    <input type="text" id="blanks-input" class="p-2 border rounded-md text-center" placeholder="Enter the word">
                    <button class="game-btn mt-4" onclick="checkBlanksAnswer()">Check</button>
                    <p id="blanks-message" class="game-message mt-4"></p>
                    <p class="mt-4">Score: <span id="blanks-score">0</span></p>
                </div>
            `;
            currentGameState.blanksIndex = 0;
            currentGameState.score = 0;
            displayBlanksSentence();
        }

        function displayBlanksSentence() {
            if (currentGameState.blanksIndex >= gameData.fillblanks.length) {
                document.getElementById('blanks-message').textContent = `Game over! Final score: ${currentGameState.score}`;
                return;
            }
            const sentenceData = gameData.fillblanks[currentGameState.blanksIndex];
            const sentence = sentenceData.sentence.replace('___', '______'); // Visual placeholder
            document.getElementById('blanks-sentence').textContent = sentence;
            document.getElementById('blanks-input').value = '';
            document.getElementById('blanks-message').textContent = '';
        }

        function checkBlanksAnswer() {
            const input = document.getElementById('blanks-input').value.toLowerCase().trim();
            const correctWord = gameData.fillblanks[currentGameState.blanksIndex].word.toLowerCase();
            const message = document.getElementById('blanks-message');

            if (input === correctWord) {
                message.textContent = 'Correct! Awesome!';
                message.style.color = '#38a169';
                currentGameState.score += 10;
                document.getElementById('blanks-score').textContent = currentGameState.score;
                currentGameState.blanksIndex++;
                setTimeout(displayBlanksSentence, 1500);
            } else {
                message.textContent = 'Incorrect. Keep trying!';
                message.style.color = '#e53e3e';
            }
        }
        
        // The Climate Goose Game (La Oca del Clima)
        function setupGooseGame() {
            const gameContent = document.getElementById('game-content');
            gameContent.innerHTML = `
                <div class="text-center">
                    <p class="text-xl font-semibold mb-4">The Climate Goose</p>
                    <div id="goose-board" class="flex flex-wrap justify-center border-2 border-gray-400 rounded-lg p-2"></div>
                    <p class="mt-4">Player is on space: <span id="goose-position">1</span></p>
                    <button class="game-btn mt-4" onclick="rollDice()">Roll Dice</button>
                    <p id="goose-message" class="game-message mt-4"></p>
                </div>
            `;
            const boardContainer = document.getElementById('goose-board');
            gooseGame.board.forEach((space, index) => {
                const spaceDiv = document.createElement('div');
                spaceDiv.className = 'w-1/5 h-16 m-1 bg-blue-200 rounded-md flex items-center justify-center text-sm';
                spaceDiv.id = `goose-space-${index}`;
                spaceDiv.textContent = space;
                if (index === 0) spaceDiv.classList.add('bg-green-400', 'text-white');
                boardContainer.appendChild(spaceDiv);
            });
            updateGoosePosition();
        }

        function rollDice() {
            const diceRoll = Math.floor(Math.random() * 3) + 1;
            const message = document.getElementById('goose-message');
            message.textContent = `You rolled a ${diceRoll}!`;
            gooseGame.player += diceRoll;
            
            if (gooseGame.player >= gooseGame.board.length - 1) {
                gooseGame.player = gooseGame.board.length - 1;
                updateGoosePosition();
                setTimeout(() => {
                    message.textContent = "Congratulations! You won the game!";
                    document.querySelector('.game-btn').disabled = true;
                }, 1000);
            } else {
                updateGoosePosition();
                setTimeout(() => handleGooseSpace(gooseGame.player), 1000);
            }
        }

        function updateGoosePosition() {
            document.querySelectorAll('#goose-board > div').forEach(div => div.classList.remove('bg-green-400', 'text-white'));
            const playerSpace = document.getElementById(`goose-space-${gooseGame.player}`);
            if (playerSpace) {
                playerSpace.classList.add('bg-green-400', 'text-white');
            }
            document.getElementById('goose-position').textContent = gooseGame.player + 1;
        }

        function handleGooseSpace(index) {
            const spaceType = gooseGame.board[index];
            const message = document.getElementById('goose-message');
            if (spaceType === "Question") {
                const question = shuffleArray(gooseGame.questions)[0];
                const answer = prompt(`${question.question}\nOptions: ${question.options.join(', ')}`);
                if (answer && answer.toLowerCase() === question.answer.toLowerCase()) {
                    message.textContent = "Correct! You stay on this space.";
                } else {
                    message.textContent = "Incorrect. You go back 1 space.";
                    gooseGame.player--;
                    updateGoosePosition();
                }
            } else if (spaceType === "Turn Lost") {
                message.textContent = "You lost a turn! Oh no!";
            } else if (spaceType === "Goose") {
                message.textContent = "You're a fast learner! Advance 1 space!";
                gooseGame.player++;
                updateGoosePosition();
            }
        }

        // Word Search Game
        function setupWordSearchGame() {
            const gameContent = document.getElementById('game-content');
            gameContent.innerHTML = `
                <div class="text-center">
                    <p class="text-xl font-semibold mb-4">Find the words in the grid!</p>
                    <div id="word-list" class="flex flex-wrap justify-center gap-2 mb-4"></div>
                    <div id="word-search-grid" class="grid grid-cols-10 gap-1 mx-auto max-w-sm"></div>
                    <p id="word-search-message" class="game-message mt-4"></p>
                </div>
            `;
            const grid = document.getElementById('word-search-grid');
            const words = gameData.wordsearch;
            let foundWords = [];
            const allLetters = "ABCDEFGHIJKLMNOPQRSTUVWXYZ".split('');
            const wordGrid = Array(10).fill(null).map(() => Array(10).fill(null));

            function placeWord(word) {
                // Simplified placement for this example
                const direction = Math.random() > 0.5 ? 'horizontal' : 'vertical';
                if (direction === 'horizontal') {
                    const row = Math.floor(Math.random() * 10);
                    const startCol = Math.floor(Math.random() * (10 - word.length));
                    for (let i = 0; i < word.length; i++) {
                        wordGrid[row][startCol + i] = word[i];
                    }
                } else {
                    const col = Math.floor(Math.random() * 10);
                    const startRow = Math.floor(Math.random() * (10 - word.length));
                    for (let i = 0; i < word.length; i++) {
                        wordGrid[startRow + i][col] = word[i];
                    }
                }
            }

            words.forEach(word => placeWord(word));

            for (let i = 0; i < 100; i++) {
                const letterDiv = document.createElement('div');
                const row = Math.floor(i / 10);
                const col = i % 10;
                letterDiv.textContent = wordGrid[row][col] || allLetters[Math.floor(Math.random() * allLetters.length)];
                letterDiv.className = 'w-8 h-8 flex items-center justify-center bg-gray-200 rounded text-xs cursor-pointer hover:bg-yellow-200';
                grid.appendChild(letterDiv);
            }

            const wordList = document.getElementById('word-list');
            words.forEach(word => {
                const wordSpan = document.createElement('span');
                wordSpan.textContent = word;
                wordSpan.id = `word-${word}`;
                wordSpan.className = 'bg-blue-300 text-white px-2 py-1 rounded-full text-sm';
                wordList.appendChild(wordSpan);
            });

            // This is a simplified version, it just finds the word on click.
            let selection = '';
            grid.addEventListener('click', (e) => {
                if (e.target.tagName === 'DIV' && e.target.textContent.length === 1) {
                    selection += e.target.textContent;
                    document.getElementById('word-search-message').textContent = `Current selection: ${selection}`;
                    if (words.includes(selection)) {
                        document.getElementById('word-search-message').textContent = `Found "${selection}"!`;
                        document.getElementById(`word-${selection}`).classList.add('bg-green-500');
                        foundWords.push(selection);
                        selection = '';
                        if (foundWords.length === words.length) {
                             document.getElementById('word-search-message').textContent = 'Congratulations! You found all the words!';
                        }
                    } else if (selection.length > 10) { // Limit length to avoid infinite search
                        selection = '';
                    }
                }
            });
        }

        // Carbon Footprint Calculator Game
        function setupCarbonGame() {
            const gameContent = document.getElementById('game-content');
            gameContent.innerHTML = `
                <div class="text-center">
                    <p class="text-xl font-semibold mb-4">Calculate your carbon footprint!</p>
                    <p id="carbon-question" class="text-lg mb-4"></p>
                    <div id="carbon-options" class="flex flex-col space-y-2"></div>
                    <p id="carbon-score" class="text-2xl font-bold mt-4">Your Footprint: <span id="carbon-points">0</span></p>
                    <p id="carbon-message" class="game-message mt-4"></p>
                </div>
            `;
            currentGameState.score = 0;
            currentGameState.questionIndex = 0;
            displayCarbonQuestion();
        }

        function displayCarbonQuestion() {
            if (currentGameState.questionIndex >= gameData.carbon.length) {
                document.getElementById('carbon-question').textContent = 'Calculation complete!';
                document.getElementById('carbon-options').innerHTML = '';
                document.getElementById('carbon-message').textContent = 'Your carbon footprint is calculated based on your answers.';
                return;
            }
            const questionData = gameData.carbon[currentGameState.questionIndex];
            document.getElementById('carbon-question').textContent = questionData.question;
            const optionsContainer = document.getElementById('carbon-options');
            optionsContainer.innerHTML = '';
            questionData.options.forEach((option, index) => {
                const button = document.createElement('button');
                button.textContent = option;
                button.className = 'game-option';
                button.onclick = () => selectCarbonAnswer(questionData.score[index]);
                optionsContainer.appendChild(button);
            });
            document.getElementById('carbon-message').textContent = '';
        }

        function selectCarbonAnswer(score) {
            currentGameState.score += score;
            document.getElementById('carbon-points').textContent = currentGameState.score;
            document.getElementById('carbon-message').textContent = `You added ${score} points to your footprint!`;
            currentGameState.questionIndex++;
            setTimeout(displayCarbonQuestion, 1500);
        }

        // Ecosystem Builder
        function setupEcosystemGame() {
            const gameContent = document.getElementById('game-content');
            gameContent.innerHTML = `
                <div class="text-center">
                    <p class="text-xl font-semibold mb-4">Drag elements to build a healthy ecosystem!</p>
                    <div id="ecosystem-container" class="relative w-full h-80 border-2 border-gray-400 rounded-lg"></div>
                    <div id="ecosystem-elements" class="flex flex-wrap justify-center mt-4 gap-2">
                        <span draggable="true" ondragstart="drag(event)" class="text-3xl p-2 cursor-grab" data-item="sun">☀️</span>
                        <span draggable="true" ondragstart="drag(event)" class="text-3xl p-2 cursor-grab" data-item="tree">🌳</span>
                        <span draggable="true" ondragstart="drag(event)" class="text-3xl p-2 cursor-grab" data-item="water">💧</span>
                        <span draggable="true" ondragstart="drag(event)" class="text-3xl p-2 cursor-grab" data-item="bird">🐦</span>
                    </div>
                    <p id="ecosystem-message" class="game-message mt-4"></p>
                </div>
            `;
            const container = document.getElementById('ecosystem-container');
            container.ondrop = (e) => {
                e.preventDefault();
                const data = e.dataTransfer.getData("text/plain");
                const element = document.createElement('span');
                element.textContent = data;
                element.className = 'absolute text-3xl';
                element.style.left = `${e.clientX - container.getBoundingClientRect().left - 15}px`;
                element.style.top = `${e.clientY - container.getBoundingClientRect().top - 15}px`;
                container.appendChild(element);
                document.getElementById('ecosystem-message').textContent = `You added a ${data} to your ecosystem!`;
            };
            container.ondragover = allowDrop;
        }

        // Rising Sea Game
        function setupRisingSeaGame() {
            const gameContent = document.getElementById('game-content');
            const { start, end, timer } = gameData.risingsea;
            let currentLevel = start;
            let gameTimer = timer;

            gameContent.innerHTML = `
                <div class="text-center">
                    <p class="text-xl font-semibold mb-4">Help the houses and animals escape the rising sea!</p>
                    <div class="relative w-full h-80 bg-blue-300 rounded-lg overflow-hidden border-2 border-gray-400">
                        <div id="sea-level" class="absolute bottom-0 w-full bg-blue-600 transition-all duration-1000 ease-linear"></div>
                        <div id="house" class="absolute text-5xl bottom-10 left-1/4 transition-all duration-300">🏠</div>
                        <div id="animal" class="absolute text-3xl bottom-10 right-1/4 transition-all duration-300">🐻</div>
                        <p class="absolute top-2 right-2 text-xl font-bold">Time: <span id="rising-sea-timer">30</span>s</p>
                    </div>
                    <button class="game-btn mt-4" onclick="raiseLand()">Raise Land</button>
                    <p id="rising-sea-message" class="game-message mt-4"></p>
                </div>
            `;
            const seaLevelDiv = document.getElementById('sea-level');
            const houseDiv = document.getElementById('house');
            const animalDiv = document.getElementById('animal');

            function updateSeaLevel() {
                seaLevelDiv.style.height = `${(start - currentLevel) * 10}%`;
                if (currentLevel <= end) {
                    clearInterval(gameInterval);
                    document.getElementById('rising-sea-message').textContent = "The sea level reached the top! Game Over!";
                    document.getElementById('rising-sea-message').style.color = '#e53e3e';
                }
            }
            
            function updateTimer() {
                gameTimer--;
                document.getElementById('rising-sea-timer').textContent = gameTimer;
                if (gameTimer <= 0) {
                    clearInterval(gameInterval);
                    document.getElementById('rising-sea-message').textContent = "Time's up! You survived!";
                    document.getElementById('rising-sea-message').style.color = '#38a169';
                }
            }

            window.raiseLand = () => {
                currentLevel -= 1;
                if (currentLevel < end) currentLevel = end;
                houseDiv.style.bottom = `${(start - currentLevel) * 10 + 10}px`;
                animalDiv.style.bottom = `${(start - currentLevel) * 10 + 5}px`;
                updateSeaLevel();
            };

            const gameInterval = setInterval(() => {
                currentLevel -= 0.1;
                updateSeaLevel();
                updateTimer();
            }, 1000);
            updateSeaLevel();
        }

        // What's the Effect? Game
        function setupMatchEffectGame() {
            const gameContent = document.getElementById('game-content');
            gameContent.innerHTML = `
                <div class="text-center">
                    <p class="text-xl font-semibold mb-4">Match the cause with the correct effect!</p>
                    <div class="flex justify-around">
                        <div id="causes" class="flex flex-col space-y-4 p-4 border rounded-lg w-1/2">
                            <p class="font-bold">Causes</p>
                        </div>
                        <div id="effects" class="flex flex-col space-y-4 p-4 border rounded-lg w-1/2">
                            <p class="font-bold">Effects</p>
                        </div>
                    </div>
                    <p id="match-effect-message" class="game-message mt-4"></p>
                    <p>Matches: <span id="match-count">0</span> / ${gameData.matcheffect.length}</p>
                </div>
            `;
            const causesContainer = document.getElementById('causes');
            const effectsContainer = document.getElementById('effects');
            
            const shuffledCauses = shuffleArray(gameData.matcheffect.map(item => item.cause));
            const shuffledEffects = shuffleArray(gameData.matcheffect.map(item => item.effect));
            
            shuffledCauses.forEach(cause => {
                const causeDiv = document.createElement('div');
                causeDiv.textContent = cause;
                causeDiv.className = 'bg-blue-300 p-2 rounded-md cursor-pointer';
                causeDiv.setAttribute('draggable', true);
                causeDiv.ondragstart = (e) => e.dataTransfer.setData("text/plain", cause);
                causesContainer.appendChild(causeDiv);
            });

            shuffledEffects.forEach(effect => {
                const effectDiv = document.createElement('div');
                effectDiv.textContent = effect;
                effectDiv.className = 'bg-green-300 p-2 rounded-md cursor-pointer';
                effectDiv.ondrop = (e) => {
                    e.preventDefault();
                    const cause = e.dataTransfer.getData("text/plain");
                    const message = document.getElementById('match-effect-message');
                    const correctPair = gameData.matcheffect.find(item => item.cause === cause && item.effect === effect);
                    if (correctPair) {
                        message.textContent = 'Correct match!';
                        message.style.color = '#38a169';
                        const causeDiv = Array.from(causesContainer.children).find(c => c.textContent === cause);
                        causeDiv.style.visibility = 'hidden';
                        effectDiv.style.visibility = 'hidden';
                        currentGameState.score++;
                        document.getElementById('match-count').textContent = currentGameState.score;
                        if (currentGameState.score === gameData.matcheffect.length) {
                             message.textContent = 'Congratulations! You matched all pairs!';
                        }
                    } else {
                        message.textContent = 'Incorrect match. Try again.';
                        message.style.color = '#e53e3e';
                    }
                };
                effectDiv.ondragover = allowDrop;
                effectsContainer.appendChild(effectDiv);
            });
        }
        
        // Eco-Challenge Game
        function setupEcoChallengeGame() {
            const gameContent = document.getElementById('game-content');
            gameContent.innerHTML = `
                <div class="text-center">
                    <p class="text-xl font-semibold mb-4">Choose an action to earn points!</p>
                    <div id="challenge-list" class="flex flex-col space-y-4"></div>
                    <p class="mt-4">Your Score: <span id="eco-score">0</span></p>
                    <p id="eco-message" class="game-message mt-4"></p>
                </div>
            `;
            currentGameState.score = 0;
            const challengeList = document.getElementById('challenge-list');
            gameData.ecochallenge.forEach(challenge => {
                const button = document.createElement('button');
                button.textContent = challenge.action;
                button.className = 'game-option';
                button.onclick = () => {
                    currentGameState.score += challenge.points;
                    document.getElementById('eco-score').textContent = currentGameState.score;
                    document.getElementById('eco-message').textContent = `You earned ${challenge.points} points!`;
                };
                challengeList.appendChild(button);
            });
        }

        // Design a Community Game
        function setupCommunityGame() {
            const gameContent = document.getElementById('game-content');
            gameContent.innerHTML = `
                <div class="text-center">
                    <p class="text-xl font-semibold mb-4">Choose options to build a sustainable community!</p>
                    <div id="community-choices" class="flex flex-col space-y-4"></div>
                    <p class="mt-4">Sustainability Score: <span id="community-score">0</span></p>
                    <p id="community-message" class="game-message mt-4"></p>
                </div>
            `;
            currentGameState.score = 0;
            const choicesContainer = document.getElementById('community-choices');
            const choices = [
                { text: "Build a solar power plant.", points: 20 },
                { text: "Plant a community garden.", points: 15 },
                { text: "Add more bike lanes.", points: 10 },
                { text: "Use reusable materials for buildings.", points: 10 }
            ];
            
            choices.forEach(choice => {
                const button = document.createElement('button');
                button.textContent = choice.text;
                button.className = 'game-option';
                button.onclick = () => {
                    currentGameState.score += choice.points;
                    document.getElementById('community-score').textContent = currentGameState.score;
                    document.getElementById('community-message').textContent = `You added ${choice.points} points to your community's sustainability!`;
                };
                choicesContainer.appendChild(button);
            });
        }

        // Helper function
        function shuffleArray(array) {
            for (let i = array.length - 1; i > 0; i--) {
                const j = Math.floor(Math.random() * (i + 1));
                [array[i], array[j]] = [array[j], array[i]];
            }
            return array;
        }

        // Initialize
        showLesson('lesson1');
    </script>
</body>
</html>
