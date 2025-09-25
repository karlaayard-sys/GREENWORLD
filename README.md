<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Our Green Planet</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #e0f2fe;
            color: #1e40af;
        }
        .section-content {
            display: none;
        }
        .section-content.active {
            display: block;
        }
        .btn-green {
            background-color: #34d399;
            color: white;
            padding: 0.75rem 1.5rem;
            border-radius: 9999px;
            font-weight: bold;
            transition: transform 0.2s, box-shadow 0.2s;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        .btn-green:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 8px rgba(0, 0, 0, 0.15);
        }
        .game-card {
            background-color: white;
            border-radius: 1.5rem;
            box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s;
        }
        .game-card:hover {
            transform: scale(1.05) rotate(2deg);
        }
    </style>
</head>
<body class="p-4 sm:p-8">
    <div class="max-w-7xl mx-auto bg-white rounded-3xl shadow-xl p-4 sm:p-8 min-h-[90vh]">
        
        <!-- Header & Navigation -->
        <header class="text-center mb-12">
            <h1 class="text-4xl sm:text-6xl font-extrabold text-blue-800">Our Green Planet 🌍</h1>
            <p class="mt-2 text-xl sm:text-2xl text-green-600">Let's learn about climate change and protect our world!</p>
            <nav class="mt-8 flex flex-wrap justify-center gap-2 sm:gap-4 text-sm sm:text-base">
                <button onclick="showSection('home')" class="btn-green">Home</button>
                <button onclick="showSection('weather-climate')" class="btn-green">Weather & Climate</button>
                <button onclick="showSection('what-is')" class="btn-green">What is Climate Change?</button>
                <button onclick="showSection('causes')" class="btn-green">Causes</button>
                <button onclick="showSection('effects')" class="btn-green">Effects</button>
                <button onclick="showSection('solutions')" class="btn-green">Solutions</button>
                <button onclick="showSection('games')" class="btn-green">Play Games!</button>
                <button onclick="showSection('final-project')" class="btn-green">Final Project</button>
            </nav>
        </header>

        <!-- Home Section -->
        <div id="home" class="section-content active text-center">
            <div class="bg-blue-100 p-6 sm:p-12 rounded-2xl">
                <h2 class="text-3xl sm:text-5xl font-bold text-blue-700">Welcome, Future Eco-Heroes!</h2>
                <p class="mt-4 text-lg sm:text-xl text-blue-600">Explore fun facts, exciting games, and amazing ideas to help our planet. We can all make a difference!</p>
                
            </div>
        </div>

        <!-- Weather & Climate Section -->
        <div id="weather-climate" class="section-content text-center">
            <h2 class="text-3xl font-bold text-blue-700 mb-4">Weather vs. Climate</h2>
            <div class="bg-green-50 p-6 rounded-2xl">
                <p class="text-lg text-green-800">Weather is what you see outside right now—is it sunny or rainy? Climate is the average weather over a long time in one place. Think of it like this: your mood today is your weather, but your personality is your climate!</p>
                
            </div>
        </div>

        <!-- What is Climate Change Section -->
        <div id="what-is" class="section-content text-center">
            <h2 class="text-3xl font-bold text-blue-700 mb-4">What is Climate Change?</h2>
            <div class="bg-green-50 p-6 rounded-2xl">
                <p class="text-lg text-green-800">Climate change means our planet's climate is getting warmer. This is caused by the sun's heat getting trapped in the atmosphere, like a blanket around the Earth. Scientists say this is happening faster than ever before because of human activities.</p>
                
            </div>
        </div>

        <!-- Causes Section -->
        <div id="causes" class="section-content text-center">
            <h2 class="text-3xl font-bold text-blue-700 mb-4">Causes of Climate Change</h2>
            <div class="bg-green-50 p-6 rounded-2xl">
                <p class="text-lg text-green-800">Many things we do every day add to climate change. Burning things like oil and gas for cars and electricity releases gases. Cutting down forests is a problem too, because trees help clean the air. These gases make the Earth's "blanket" thicker.</p>
                
            </div>
        </div>

        <!-- Effects Section -->
        <div id="effects" class="section-content text-center">
            <h2 class="text-3xl font-bold text-blue-700 mb-4">Effects of Climate Change</h2>
            <div class="bg-green-50 p-6 rounded-2xl">
                <p class="text-lg text-green-800">A warmer Earth can cause big problems! Ice at the North and South Poles is melting, which makes sea levels rise. This can cause floods. It also changes where animals can live and can make storms stronger and more dangerous.</p>
                
            </div>
        </div>

        <!-- Solutions Section -->
        <div id="solutions" class="section-content text-center">
            <h2 class="text-3xl font-bold text-blue-700 mb-4">Solutions for a Healthier Planet</h2>
            <div class="bg-green-50 p-6 rounded-2xl">
                <p class="text-lg text-green-800">The good news is we can help! We can use less energy, like turning off lights when we leave a room. We can also walk or bike instead of taking a car. Recycling and planting new trees are also super important ways to make a difference!</p>
                
            </div>
        </div>

        <!-- Games Section -->
        <div id="games" class="section-content text-center">
            <h2 class="text-3xl font-bold text-blue-700 mb-6">Play Our Eco-Games!</h2>
            <div id="game-container" class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
                <div class="game-card p-6 cursor-pointer" onclick="runGame('la-oca')">
                    <i class="fa-solid fa-dice fa-2x text-blue-500"></i>
                    <h3 class="font-bold text-xl mt-2">La Oca del Clima</h3>
                    <p class="text-gray-600 mt-1">A fun board game to learn about climate actions.</p>
                </div>
                <div class="game-card p-6 cursor-pointer" onclick="runGame('climate-challenge')">
                    <i class="fa-solid fa-leaf fa-2x text-green-500"></i>
                    <h3 class="font-bold text-xl mt-2">Climate Challenge</h3>
                    <p class="text-gray-600 mt-1">Make big decisions to save the planet!</p>
                </div>
                <div class="game-card p-6 cursor-pointer" onclick="runGame('mission-1-5')">
                    <i class="fa-solid fa-vote-yea fa-2x text-red-500"></i>
                    <h3 class="font-bold text-xl mt-2">Mission 1.5</h3>
                    <p class="text-gray-600 mt-1">Vote for the best climate solutions.</p>
                </div>
                <div class="game-card p-6 cursor-pointer" onclick="runGame('recicla-gana')">
                    <i class="fa-solid fa-recycle fa-2x text-yellow-500"></i>
                    <h3 class="font-bold text-xl mt-2">Recicla y Gana</h3>
                    <p class="text-gray-600 mt-1">Recycling trivia: test your knowledge!</p>
                </div>
                <div class="game-card p-6 cursor-pointer" onclick="runGame('extincion')">
                    <i class="fa-solid fa-skull fa-2x text-gray-500"></i>
                    <h3 class="font-bold text-xl mt-2">¡Extinción!</h3>
                    <p class="text-gray-600 mt-1">Save the dinosaurs by matching cards.</p>
                </div>
                <div class="game-card p-6 cursor-pointer" onclick="runGame('bitoku')">
                    <i class="fa-solid fa-heart fa-2x text-pink-500"></i>
                    <h3 class="font-bold text-xl mt-2">Bitoku</h3>
                    <p class="text-gray-600 mt-1">Protect nature and save the spirits.</p>
                </div>
                <div class="game-card p-6 cursor-pointer" onclick="runGame('paleo')">
                    <i class="fa-solid fa-tree fa-2x text-lime-500"></i>
                    <h3 class="font-bold text-xl mt-2">Paleo</h3>
                    <p class="text-gray-600 mt-1">Cooperate to manage resources.</p>
                </div>
                <div class="game-card p-6 cursor-pointer" onclick="runGame('memorama')">
                    <i class="fa-solid fa-brain fa-2x text-purple-500"></i>
                    <h3 class="font-bold text-xl mt-2">Memorama</h3>
                    <p class="text-gray-600 mt-1">A memory game with climate words.</p>
                </div>
                <div class="game-card p-6 cursor-pointer" onclick="runGame('true-false')">
                    <i class="fa-solid fa-check-double fa-2x text-teal-500"></i>
                    <h3 class="font-bold text-xl mt-2">True/False Quiz</h3>
                    <p class="text-gray-600 mt-1">Is it true or false? You decide!</p>
                </div>
                <div class="game-card p-6 cursor-pointer" onclick="runGame('multiple-choice')">
                    <i class="fa-solid fa-question fa-2x text-orange-500"></i>
                    <h3 class="font-bold text-xl mt-2">Multiple Choice</h3>
                    <p class="text-gray-600 mt-1">Choose the right answer to win!</p>
                </div>
            </div>
            
            <!-- Game Display Area -->
            <div id="game-display" class="mt-8 p-6 bg-blue-50 rounded-2xl shadow-inner hidden">
                <button onclick="hideGame()" class="btn-green float-right">Back to Games</button>
                <h3 id="game-title" class="text-2xl font-bold text-blue-700 mb-4"></h3>
                <div id="game-area"></div>
            </div>
        </div>

        <!-- Final Project Section -->
        <div id="final-project" class="section-content text-center">
            <h2 class="text-3xl font-bold text-blue-700 mb-4">Your Final Project: My Climate Action Plan</h2>
            <div class="bg-green-50 p-6 rounded-2xl">
                <p class="text-lg text-green-800 mb-4">Think about all the things you learned. What is one thing you can do to help our planet? Write your plan below and share it with your family and friends!</p>
                <textarea class="w-full h-40 p-4 rounded-xl border-2 border-green-300 text-gray-800" placeholder="My plan is to..."></textarea>
            </div>
        </div>
        
    </div>

    <!-- Alert/Modal Box for Messages -->
    <div id="modal" class="fixed inset-0 bg-gray-600 bg-opacity-50 overflow-y-auto h-full w-full hidden">
        <div class="relative top-20 mx-auto p-5 border w-96 shadow-lg rounded-md bg-white text-center">
            <div id="modal-content" class="mt-3 text-center"></div>
            <div class="items-center px-4 py-3">
                <button id="close-modal" class="btn-green w-full">OK</button>
            </div>
        </div>
    </div>

    <script>
        // Global variables for game logic
        let score = 0;
        let gameData = {};
        let cardPairs = [];
        let flippedCards = [];
        let matchedPairs = 0;
        let boardState = [];
        let playerPosition = 0;
        let gameScore = 0;

        // Utility function to show a custom modal
        function showModal(message) {
            const modal = document.getElementById('modal');
            const modalContent = document.getElementById('modal-content');
            modalContent.innerHTML = `<p class="text-lg font-semibold">${message}</p>`;
            modal.style.display = "block";
        }
        document.getElementById('close-modal').onclick = function() {
            document.getElementById('modal').style.display = "none";
        };

        // Section management
        function showSection(id) {
            const sections = document.querySelectorAll('.section-content');
            sections.forEach(sec => sec.classList.remove('active'));
            document.getElementById(id).classList.add('active');
            hideGame();
        }

        function runGame(gameId) {
            const gameDisplay = document.getElementById('game-display');
            const gameTitle = document.getElementById('game-title');
            const gameArea = document.getElementById('game-area');

            gameDisplay.classList.remove('hidden');
            gameArea.innerHTML = ''; // Clear previous game
            gameScore = 0;
            score = 0;
            matchedPairs = 0;

            switch(gameId) {
                case 'la-oca':
                    gameTitle.textContent = "La Oca del Clima";
                    runLaOca();
                    break;
                case 'climate-challenge':
                    gameTitle.textContent = "Climate Challenge";
                    runClimateChallenge();
                    break;
                case 'mission-1-5':
                    gameTitle.textContent = "Mission 1.5";
                    runMission15();
                    break;
                case 'recicla-gana':
                    gameTitle.textContent = "Recicla y Gana";
                    runReciclaYGana();
                    break;
                case 'extincion':
                    gameTitle.textContent = "¡Extinción!";
                    runExtincion();
                    break;
                case 'bitoku':
                    gameTitle.textContent = "Bitoku";
                    runBitoku();
                    break;
                case 'paleo':
                    gameTitle.textContent = "Paleo";
                    runPaleo();
                    break;
                case 'memorama':
                    gameTitle.textContent = "Memorama";
                    runMemorama();
                    break;
                case 'true-false':
                    gameTitle.textContent = "True/False Quiz";
                    runTrueFalse();
                    break;
                case 'multiple-choice':
                    gameTitle.textContent = "Multiple Choice Challenge";
                    runMultipleChoice();
                    break;
            }
        }

        function hideGame() {
            document.getElementById('game-display').classList.add('hidden');
            document.getElementById('game-area').innerHTML = '';
        }

        // --- Game Logic Functions ---

        // La Oca del Clima
        function runLaOca() {
            const gameArea = document.getElementById('game-area');
            playerPosition = 0;
            gameArea.innerHTML = `
                <div class="text-center">
                    <p class="text-xl">Your current space: <span id="oca-position" class="font-bold">1</span></p>
                    <button onclick="rollDice()" class="btn-green my-4">Roll Dice!</button>
                    <p id="oca-message" class="text-lg mt-2 font-semibold text-blue-800"></p>
                    <div id="oca-board" class="grid grid-cols-5 gap-2 mt-4 max-w-lg mx-auto p-4 bg-lime-200 rounded-lg"></div>
                </div>
            `;
            const board = document.getElementById('oca-board');
            boardState = [
                "Start!", "Go to school on your bike. Move 2 spaces!", "Left the lights on. Go back 1 space.", "Recycled a bottle. Move 1 space!", "Left the water running. Go back to start!",
                "Planted a tree. Move to space 10!", "Used a reusable bag. Move 2 spaces!", "Threw a can in the trash. Go back 3 spaces.", "Turned off the TV. Move 1 space!", "Finished!"
            ];
            boardState.forEach((text, index) => {
                const space = document.createElement('div');
                space.className = `p-2 text-xs sm:text-sm text-center border-2 rounded-lg ${index === 0 ? 'bg-green-400' : index === 9 ? 'bg-blue-400' : 'bg-white'}`;
                space.textContent = index + 1;
                space.id = `oca-space-${index}`;
                board.appendChild(space);
            });
            updateOcaBoard();
        }

        function rollDice() {
            const roll = Math.floor(Math.random() * 4) + 1;
            const messageEl = document.getElementById('oca-message');
            messageEl.textContent = `You rolled a ${roll}!`;

            let newPosition = playerPosition + roll;
            if (newPosition >= boardState.length) {
                newPosition = boardState.length - 1;
            }

            playerPosition = newPosition;

            updateOcaBoard();
            setTimeout(() => {
                const actionMessage = boardState[playerPosition];
                showModal(actionMessage);
                if (actionMessage.includes("Go back 1 space")) playerPosition -= 1;
                if (actionMessage.includes("Go back 3 spaces")) playerPosition -= 3;
                if (actionMessage.includes("Move 2 spaces")) playerPosition += 2;
                if (actionMessage.includes("Move to space 10")) playerPosition = 9;
                if (actionMessage.includes("Go back to start")) playerPosition = 0;
                
                if (playerPosition >= 9) {
                    showModal("You won! You've reached the end and are a true eco-hero!");
                }
                updateOcaBoard();
            }, 1000);
        }

        function updateOcaBoard() {
            const board = document.getElementById('oca-board');
            board.querySelectorAll('div').forEach((space, index) => {
                space.classList.remove('border-blue-500', 'border-4');
                if (index === playerPosition) {
                    space.classList.add('border-blue-500', 'border-4');
                }
            });
            document.getElementById('oca-position').textContent = playerPosition + 1;
        }

        // Climate Challenge
        function runClimateChallenge() {
            gameData = {
                questions: [
                    {
                        text: "A big factory wants to open in your town. It will bring jobs but also a lot of pollution. What do you do?",
                        choices: [
                            { text: "Welcome the factory. We need the jobs.", score: -5 },
                            { text: "Ask the company to use clean energy.", score: +10 },
                            { text: "Try to stop the factory completely.", score: +5 }
                        ]
                    },
                    {
                        text: "Your parents want a new car. You have two choices. What do you pick?",
                        choices: [
                            { text: "A big gas car.", score: -10 },
                            { text: "A small, fuel-efficient car.", score: +5 },
                            { text: "An electric car.", score: +15 }
                        ]
                    },
                    {
                        text: "Your school is throwing away a lot of food. What should you do?",
                        choices: [
                            { text: "Do nothing, it's not your problem.", score: -5 },
                            { text: "Start a campaign to compost the food scraps.", score: +10 },
                            { text: "Write a letter to the principal about food waste.", score: +5 }
                        ]
                    }
                ],
                currentQuestion: 0,
                score: 50 // starting score
            };
            displayClimateChallengeQuestion();
        }

        function displayClimateChallengeQuestion() {
            const gameArea = document.getElementById('game-area');
            const q = gameData.questions[gameData.currentQuestion];
            if (!q) {
                gameArea.innerHTML = `<h3 class="text-2xl font-bold">Game Over!</h3><p class="text-xl mt-2">Your final score: ${gameData.score}/100</p>`;
                return;
            }
            gameArea.innerHTML = `<div class="p-6 bg-white rounded-xl shadow-md">
                <p class="text-xl mb-4 font-semibold">${q.text}</p>
                <div class="flex flex-col gap-4">
                    ${q.choices.map((choice, index) =>
                        `<button onclick="chooseClimateChallenge(${index})" class="btn-green w-full">${choice.text}</button>`
                    ).join('')}
                </div>
            </div>`;
        }
        
        function chooseClimateChallenge(choiceIndex) {
            const q = gameData.questions[gameData.currentQuestion];
            gameData.score += q.choices[choiceIndex].score;
            gameData.currentQuestion++;
            displayClimateChallengeQuestion();
        }

        // Mission 1.5
        function runMission15() {
            gameData = {
                solutions: [
                    { name: "Solar Power", description: "Use the sun's energy to make electricity.", impact: "High" },
                    { name: "Planting Trees", description: "Grow new forests to absorb carbon.", impact: "Medium" },
                    { name: "Recycling", description: "Turn old things into new ones.", impact: "Medium" },
                    { name: "Public Transport", description: "Use buses and trains to reduce car pollution.", impact: "High" }
                ],
                votes: {}
            };
            gameData.solutions.forEach(sol => gameData.votes[sol.name] = 0);
            displayMission15Solutions();
        }

        function displayMission15Solutions() {
            const gameArea = document.getElementById('game-area');
            gameArea.innerHTML = `<p class="text-xl mb-4">Vote for the best climate solution!</p>
                <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                    ${gameData.solutions.map(sol =>
                        `<div class="p-4 bg-white rounded-lg shadow-md text-center">
                            <h4 class="font-bold text-lg">${sol.name}</h4>
                            <p class="text-sm text-gray-600">${sol.description}</p>
                            <button onclick="voteMission15('${sol.name}')" class="btn-green mt-2">Vote! (<span id="votes-${sol.name}">0</span>)</button>
                        </div>`
                    ).join('')}
                </div>`;
        }

        function voteMission15(solutionName) {
            gameData.votes[solutionName]++;
            document.getElementById(`votes-${solutionName}`).textContent = gameData.votes[solutionName];
        }

        // Recicla y Gana
        function runReciclaYGana() {
            gameData = {
                questions: [
                    { q: "What is a single-use plastic?", a: "A plastic item used only once, like a soda bottle.", wrong: ["A super-strong plastic.", "A plastic that can't be recycled."] },
                    { q: "Where does a glass jar go?", a: "In the recycling bin.", wrong: ["In the trash can.", "In the compost."] },
                    { q: "What does 'reduce, reuse, recycle' mean?", a: "To use less, find new uses for things, and turn old things into new ones.", wrong: ["To use more, buy new things, and throw everything away.", "To save money and time."] }
                ],
                currentQuestion: 0,
                score: 0
            };
            displayReciclaYGanaQuestion();
        }

        function displayReciclaYGanaQuestion() {
            const gameArea = document.getElementById('game-area');
            const q = gameData.questions[gameData.currentQuestion];
            if (!q) {
                gameArea.innerHTML = `<h3 class="text-2xl font-bold">Game Over!</h3><p class="text-xl mt-2">Your score: ${gameData.score}/${gameData.questions.length}</p>`;
                return;
            }
            const choices = shuffleArray([q.a, ...q.wrong]);
            gameArea.innerHTML = `<div class="p-6 bg-white rounded-xl shadow-md">
                <p class="text-xl mb-4 font-semibold">${q.q}</p>
                <div class="flex flex-col gap-4">
                    ${choices.map(choice =>
                        `<button onclick="checkReciclaYGana('${choice}', '${q.a}')" class="btn-green w-full">${choice}</button>`
                    ).join('')}
                </div>
            </div>`;
        }

        function checkReciclaYGana(answer, correctAnswer) {
            if (answer === correctAnswer) {
                gameData.score++;
                showModal("Correct! Great job!");
            } else {
                showModal(`Oops, that's wrong. The correct answer was: ${correctAnswer}`);
            }
            gameData.currentQuestion++;
            setTimeout(displayReciclaYGanaQuestion, 2000);
        }

        // ¡Extinción!
        function runExtincion() {
            cardPairs = ['dino1', 'dino1', 'dino2', 'dino2', 'dino3', 'dino3', 'dino4', 'dino4', 'dino5', 'dino5', 'dino6', 'dino6'];
            cardPairs = shuffleArray(cardPairs);
            flippedCards = [];
            matchedPairs = 0;

            const gameArea = document.getElementById('game-area');
            gameArea.innerHTML = `
                <p class="text-xl mb-4">Match the dinosaur cards to save them from extinction!</p>
                <div id="extincion-board" class="grid grid-cols-4 gap-4 max-w-lg mx-auto"></div>
            `;
            const board = document.getElementById('extincion-board');
            cardPairs.forEach((pair, index) => {
                const card = document.createElement('div');
                card.className = 'w-20 h-28 bg-blue-300 rounded-lg shadow-md cursor-pointer flex items-center justify-center text-5xl text-white font-bold transition-transform transform rotate-y-180';
                card.dataset.pair = pair;
                card.dataset.index = index;
                card.textContent = '🦖';
                card.onclick = () => flipCard(card);
                board.appendChild(card);
            });
        }

        function flipCard(card) {
            if (flippedCards.length < 2 && !card.classList.contains('bg-green-500')) {
                card.classList.remove('bg-blue-300');
                card.classList.add('bg-white', 'text-gray-800');
                card.textContent = card.dataset.pair.replace('dino', '🦕'); // Simple visual change
                flippedCards.push(card);

                if (flippedCards.length === 2) {
                    setTimeout(checkMatch, 1000);
                }
            }
        }

        function checkMatch() {
            const [card1, card2] = flippedCards;
            if (card1.dataset.pair === card2.dataset.pair) {
                card1.classList.add('bg-green-500', 'text-white');
                card2.classList.add('bg-green-500', 'text-white');
                matchedPairs++;
                if (matchedPairs === cardPairs.length / 2) {
                    showModal("You saved all the dinosaurs! Great job!");
                }
            } else {
                card1.classList.remove('bg-white', 'text-gray-800');
                card1.classList.add('bg-blue-300', 'text-white');
                card1.textContent = '🦖';
                card2.classList.remove('bg-white', 'text-gray-800');
                card2.classList.add('bg-blue-300', 'text-white');
                card2.textContent = '🦖';
            }
            flippedCards = [];
        }

        // Bitoku
        function runBitoku() {
            const gameArea = document.getElementById('game-area');
            score = 0;
            gameArea.innerHTML = `
                <h3 class="text-2xl font-bold mb-4">Help the spirits of nature clean the forest!</h3>
                <p class="text-xl">Score: <span id="bitoku-score" class="font-bold">0</span></p>
                <div id="bitoku-forest" class="mt-4 p-4 bg-green-200 rounded-xl relative overflow-hidden min-h-[300px]"></div>
            `;
            setInterval(spawnPollutant, 1000);
        }

        function spawnPollutant() {
            const forest = document.getElementById('bitoku-forest');
            if (forest.childElementCount > 20) return; // Prevent too many items
            const pollutant = document.createElement('div');
            pollutant.className = 'w-8 h-8 bg-red-500 rounded-full absolute cursor-pointer shadow-md';
            pollutant.style.top = `${Math.random() * 90}%`;
            pollutant.style.left = `${Math.random() * 90}%`;
            pollutant.onclick = () => {
                score++;
                document.getElementById('bitoku-score').textContent = score;
                pollutant.remove();
            };
            forest.appendChild(pollutant);
        }

        // Paleo
        function runPaleo() {
            gameData = { resources: { wood: 0, stone: 0, food: 0 } };
            const gameArea = document.getElementById('game-area');
            gameArea.innerHTML = `
                <h3 class="text-2xl font-bold mb-4">Cooperate to build a sustainable home!</h3>
                <p class="text-xl">Gather resources to build your home. Click the buttons to collect!</p>
                <div class="flex justify-center gap-8 my-6">
                    <div class="text-center">
                        <i class="fa-solid fa-tree fa-4x text-lime-500"></i>
                        <p class="text-xl font-bold mt-2">Wood: <span id="paleo-wood">0</span></p>
                        <button onclick="collectResource('wood')" class="btn-green mt-2">Collect Wood</button>
                    </div>
                    <div class="text-center">
                        <i class="fa-solid fa-mountain fa-4x text-gray-500"></i>
                        <p class="text-xl font-bold mt-2">Stone: <span id="paleo-stone">0</span></p>
                        <button onclick="collectResource('stone')" class="btn-green mt-2">Collect Stone</button>
                    </div>
                    <div class="text-center">
                        <i class="fa-solid fa-apple-alt fa-4x text-red-500"></i>
                        <p class="text-xl font-bold mt-2">Food: <span id="paleo-food">0</span></p>
                        <button onclick="collectResource('food')" class="btn-green mt-2">Collect Food</button>
                    </div>
                </div>
                <div class="mt-8 text-center">
                    <button onclick="buildHome()" class="btn-green text-2xl p-4">Build Home (10 wood, 10 stone, 5 food)</button>
                </div>
            `;
        }
        function collectResource(resource) {
            gameData.resources[resource]++;
            document.getElementById(`paleo-${resource}`).textContent = gameData.resources[resource];
        }
        function buildHome() {
            if (gameData.resources.wood >= 10 && gameData.resources.stone >= 10 && gameData.resources.food >= 5) {
                showModal("Congratulations! You built a sustainable home!");
                runPaleo(); // Reset for a new game
            } else {
                showModal("You don't have enough resources yet. Keep collecting!");
            }
        }

        // Memorama
        function runMemorama() {
            const concepts = ['Recycle', 'Solar', 'Wind', 'Water', 'Forest', 'Pollution', 'Ozone', 'Carbon'];
            const cardValues = concepts.concat(concepts);
            gameData = { cards: shuffleArray(cardValues), flipped: [], matched: [] };
            const gameArea = document.getElementById('game-area');
            gameArea.innerHTML = `<h3 class="text-2xl font-bold mb-4">Match the climate concepts!</h3>
                <div id="memorama-board" class="grid grid-cols-4 gap-4"></div>`;
            const board = document.getElementById('memorama-board');
            gameData.cards.forEach((value, index) => {
                const card = document.createElement('div');
                card.className = 'p-4 bg-blue-300 rounded-lg shadow-md cursor-pointer h-24 flex items-center justify-center font-bold text-center';
                card.dataset.value = value;
                card.dataset.index = index;
                card.textContent = '?';
                card.onclick = () => flipMemoramaCard(card);
                board.appendChild(card);
            });
        }
        function flipMemoramaCard(card) {
            if (gameData.flipped.length < 2 && !gameData.matched.includes(card.dataset.index)) {
                card.textContent = card.dataset.value;
                card.style.backgroundColor = 'white';
                gameData.flipped.push(card);
                if (gameData.flipped.length === 2) {
                    setTimeout(checkMemoramaMatch, 1000);
                }
            }
        }
        function checkMemoramaMatch() {
            const [card1, card2] = gameData.flipped;
            if (card1.dataset.value === card2.dataset.value) {
                gameData.matched.push(parseInt(card1.dataset.index), parseInt(card2.dataset.index));
                card1.style.backgroundColor = '#34d399';
                card2.style.backgroundColor = '#34d399';
                if (gameData.matched.length === gameData.cards.length) {
                    showModal("You matched all the pairs! You have an amazing memory!");
                }
            } else {
                card1.textContent = '?';
                card1.style.backgroundColor = '#93c5fd';
                card2.textContent = '?';
                card2.style.backgroundColor = '#93c5fd';
            }
            gameData.flipped = [];
        }

        // True/False Quiz
        function runTrueFalse() {
            gameData = {
                questions: [
                    { q: "Cutting down trees helps fight climate change.", a: false },
                    { q: "Recycling a plastic bottle saves energy.", a: true },
                    { q: "Only grown-ups can help save the planet.", a: false },
                    { q: "Solar panels use energy from the sun.", a: true }
                ],
                currentQuestion: 0,
                score: 0
            };
            displayTrueFalseQuestion();
        }
        function displayTrueFalseQuestion() {
            const gameArea = document.getElementById('game-area');
            const q = gameData.questions[gameData.currentQuestion];
            if (!q) {
                gameArea.innerHTML = `<h3 class="text-2xl font-bold">Quiz Finished!</h3><p class="text-xl mt-2">Your score: ${gameData.score}/${gameData.questions.length}</p>`;
                return;
            }
            gameArea.innerHTML = `<div class="p-6 bg-white rounded-xl shadow-md">
                <p class="text-xl mb-4 font-semibold">${q.q}</p>
                <div class="flex justify-center gap-4">
                    <button onclick="checkTrueFalse(true)" class="btn-green">True</button>
                    <button onclick="checkTrueFalse(false)" class="btn-green">False</button>
                </div>
            </div>`;
        }
        function checkTrueFalse(answer) {
            const q = gameData.questions[gameData.currentQuestion];
            if (answer === q.a) {
                gameData.score++;
                showModal("Correct!");
            } else {
                showModal("Wrong answer.");
            }
            gameData.currentQuestion++;
            setTimeout(displayTrueFalseQuestion, 2000);
        }

        // Multiple Choice Challenge
        function runMultipleChoice() {
            gameData = {
                questions: [
                    { q: "What is the name of the 'blanket' of gases that traps heat around the Earth?", choices: ["The Ozone Layer", "The Atmosphere", "The Greenhouse Effect", "The Climate Zone"], a: "The Greenhouse Effect" },
                    { q: "Which of these is a clean energy source?", choices: ["Coal", "Oil", "Wind", "Gas"], a: "Wind" },
                    { q: "What is one way to help reduce your carbon footprint?", choices: ["Leave lights on all day.", "Drive a car everywhere you go.", "Buy a lot of new things.", "Ride your bike or walk."], a: "Ride your bike or walk." }
                ],
                currentQuestion: 0,
                score: 0
            };
            displayMultipleChoiceQuestion();
        }
        function displayMultipleChoiceQuestion() {
            const gameArea = document.getElementById('game-area');
            const q = gameData.questions[gameData.currentQuestion];
            if (!q) {
                gameArea.innerHTML = `<h3 class="text-2xl font-bold">Quiz Finished!</h3><p class="text-xl mt-2">Your score: ${gameData.score}/${gameData.questions.length}</p>`;
                return;
            }
            const choices = shuffleArray(q.choices);
            gameArea.innerHTML = `<div class="p-6 bg-white rounded-xl shadow-md">
                <p class="text-xl mb-4 font-semibold">${q.q}</p>
                <div class="flex flex-col gap-4">
                    ${choices.map(choice =>
                        `<button onclick="checkMultipleChoice('${choice}', '${q.a}')" class="btn-green w-full">${choice}</button>`
                    ).join('')}
                </div>
            </div>`;
        }
        function checkMultipleChoice(answer, correctAnswer) {
            if (answer === correctAnswer) {
                gameData.score++;
                showModal("You got it right!");
            } else {
                showModal(`Not quite. The correct answer was: ${correctAnswer}`);
            }
            gameData.currentQuestion++;
            setTimeout(displayMultipleChoiceQuestion, 2000);
        }

        // Fisher-Yates shuffle algorithm for arrays
        function shuffleArray(array) {
            for (let i = array.length - 1; i > 0; i--) {
                const j = Math.floor(Math.random() * (i + 1));
                [array[i], array[j]] = [array[j], array[i]];
            }
            return array;
        }

    </script>
</body>
</html>
