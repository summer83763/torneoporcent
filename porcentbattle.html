<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Torneo Percentage Quest - Secundaria</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Space+Grotesk:wght@300;400;600;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Space Grotesk', sans-serif;
            background: linear-gradient(135deg, #0a0a0a 0%, #1a1a2e 25%, #16213e 50%, #0f3460 75%, #1a1a2e 100%);
            min-height: 100vh;
            overflow-x: hidden;
            position: relative;
        }

        body::before {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: 
                radial-gradient(circle at 20% 50%, rgba(120, 119, 198, 0.3) 0%, transparent 50%),
                radial-gradient(circle at 80% 20%, rgba(255, 119, 198, 0.3) 0%, transparent 50%),
                radial-gradient(circle at 40% 80%, rgba(120, 255, 198, 0.3) 0%, transparent 50%);
            pointer-events: none;
            z-index: -1;
        }

        .stars {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }

        .star {
            position: absolute;
            width: 2px;
            height: 2px;
            background: white;
            border-radius: 50%;
            animation: twinkle 3s infinite;
        }

        @keyframes twinkle {
            0%, 100% { opacity: 0.3; transform: scale(1); }
            50% { opacity: 1; transform: scale(1.2); }
        }

        .game-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            position: relative;
            z-index: 1;
        }

        .game-header {
            text-align: center;
            margin-bottom: 30px;
            position: relative;
        }

        .game-title {
            font-family: 'Orbitron', monospace;
            font-size: 3rem;
            font-weight: 900;
            background: linear-gradient(45deg, #00f5ff, #ff00f5, #f5ff00, #00f5ff);
            background-size: 300% 300%;
            -webkit-background-clip: text;
            background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: gradientShift 3s ease-in-out infinite, glow 2s ease-in-out infinite alternate;
            text-shadow: 0 0 30px rgba(0, 245, 255, 0.5);
            margin-bottom: 10px;
        }

        @keyframes gradientShift {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }

        @keyframes glow {
            from { filter: drop-shadow(0 0 20px rgba(0, 245, 255, 0.5)); }
            to { filter: drop-shadow(0 0 40px rgba(255, 0, 245, 0.8)); }
        }

        .game-subtitle {
            font-size: 1.3rem;
            color: #a0a0ff;
            opacity: 0.9;
            margin-bottom: 20px;
            font-weight: 600;
        }

        .tournament-stats {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-bottom: 30px;
        }

        .stat-card {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 20px;
            padding: 25px;
            position: relative;
            overflow: hidden;
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .stat-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.1), transparent);
            transition: left 0.5s;
        }

        .stat-card:hover {
            transform: translateY(-5px) scale(1.02);
            border-color: rgba(0, 245, 255, 0.4);
            box-shadow: 0 20px 40px rgba(0, 245, 255, 0.2);
        }

        .stat-card:hover::before {
            left: 100%;
        }

        .stat-label {
            font-size: 0.9rem;
            color: #a0a0ff;
            margin-bottom: 10px;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .stat-value {
            font-family: 'Orbitron', monospace;
            font-size: 2rem;
            font-weight: 700;
            color: #00f5ff;
            text-shadow: 0 0 10px rgba(0, 245, 255, 0.5);
        }

        .timer-card {
            background: rgba(255, 255, 255, 0.08);
            backdrop-filter: blur(25px);
            border: 2px solid rgba(255, 215, 0, 0.3);
            border-radius: 25px;
            padding: 30px;
            margin-bottom: 20px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .timer-card.warning {
            border-color: rgba(255, 165, 0, 0.6);
            animation: warningPulse 1s infinite;
        }

        .timer-card.danger {
            border-color: rgba(255, 71, 87, 0.8);
            animation: dangerPulse 0.5s infinite;
        }

        @keyframes warningPulse {
            0%, 100% { box-shadow: 0 0 20px rgba(255, 165, 0, 0.3); }
            50% { box-shadow: 0 0 40px rgba(255, 165, 0, 0.6); }
        }

        @keyframes dangerPulse {
            0%, 100% { box-shadow: 0 0 30px rgba(255, 71, 87, 0.5); }
            50% { box-shadow: 0 0 60px rgba(255, 71, 87, 0.8); }
        }

        .timer-display {
            font-family: 'Orbitron', monospace;
            font-size: 4rem;
            font-weight: 900;
            color: #f5ff00;
            text-shadow: 0 0 20px rgba(245, 255, 0, 0.7);
            margin-bottom: 10px;
        }

        .timer-display.warning {
            color: #ffa500;
            text-shadow: 0 0 20px rgba(255, 165, 0, 0.7);
        }

        .timer-display.danger {
            color: #ff4757;
            text-shadow: 0 0 20px rgba(255, 71, 87, 0.7);
        }

        .question-counter {
            font-size: 1.2rem;
            color: #a0a0ff;
            margin-bottom: 15px;
        }

        .question-card {
            background: rgba(255, 255, 255, 0.08);
            backdrop-filter: blur(25px);
            border: 1px solid rgba(255, 255, 255, 0.15);
            border-radius: 25px;
            padding: 40px;
            margin-bottom: 30px;
            position: relative;
            overflow: hidden;
            box-shadow: 0 25px 50px rgba(0, 0, 0, 0.3);
        }

        .question-card::before {
            content: '';
            position: absolute;
            top: -2px;
            left: -2px;
            right: -2px;
            bottom: -2px;
            background: linear-gradient(45deg, #00f5ff, #ff00f5, #f5ff00, #00f5ff);
            background-size: 300% 300%;
            border-radius: 25px;
            z-index: -1;
            animation: borderGlow 3s linear infinite;
            opacity: 0.7;
        }

        @keyframes borderGlow {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }

        .question-text {
            font-size: 1.8rem;
            color: #ffffff;
            margin-bottom: 30px;
            line-height: 1.6;
            text-align: center;
            font-weight: 600;
        }

        .answers-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 20px;
            margin-bottom: 20px;
        }

        .answer-btn {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(15px);
            border: 2px solid rgba(255, 255, 255, 0.2);
            border-radius: 15px;
            padding: 25px;
            color: #ffffff;
            font-size: 1.3rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
            min-height: 80px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .answer-btn::before {
            content: '';
            position: absolute;
            top: 50%;
            left: 50%;
            width: 0;
            height: 0;
            background: radial-gradient(circle, rgba(0, 245, 255, 0.3) 0%, transparent 70%);
            transition: all 0.3s ease;
            transform: translate(-50%, -50%);
            border-radius: 50%;
        }

        .answer-btn:hover {
            transform: translateY(-3px) scale(1.02);
            border-color: #00f5ff;
            box-shadow: 0 15px 30px rgba(0, 245, 255, 0.3);
            color: #00f5ff;
        }

        .answer-btn:hover::before {
            width: 300px;
            height: 300px;
        }

        .answer-btn:active {
            transform: translateY(-1px);
        }

        .answer-btn.correct {
            background: rgba(46, 213, 115, 0.2);
            border-color: #2ed573;
            color: #2ed573;
            animation: correctPulse 0.6s ease;
        }

        .answer-btn.incorrect {
            background: rgba(255, 71, 87, 0.2);
            border-color: #ff4757;
            color: #ff4757;
            animation: incorrectShake 0.6s ease;
        }

        @keyframes correctPulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }

        @keyframes incorrectShake {
            0%, 100% { transform: translateX(0); }
            25% { transform: translateX(-8px); }
            75% { transform: translateX(8px); }
        }

        .feedback {
            text-align: center;
            font-size: 1.4rem;
            font-weight: 600;
            margin: 20px 0;
            opacity: 0;
            transform: translateY(20px);
            transition: all 0.5s ease;
        }

        .feedback.show {
            opacity: 1;
            transform: translateY(0);
        }

        .feedback.correct {
            color: #2ed573;
            text-shadow: 0 0 15px rgba(46, 213, 115, 0.5);
        }

        .feedback.incorrect {
            color: #ff4757;
            text-shadow: 0 0 15px rgba(255, 71, 87, 0.5);
        }

        .game-over {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.95);
            backdrop-filter: blur(30px);
            display: flex;
            align-items: center;
            justify-content: center;
            z-index: 2000;
            opacity: 0;
            visibility: hidden;
            transition: all 0.5s ease;
        }

        .game-over.show {
            opacity: 1;
            visibility: visible;
        }

        .game-over-content {
            text-align: center;
            transform: scale(0.8);
            transition: transform 0.5s cubic-bezier(0.68, -0.55, 0.265, 1.55);
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(20px);
            border: 2px solid rgba(255, 255, 255, 0.2);
            border-radius: 25px;
            padding: 50px;
        }

        .game-over.show .game-over-content {
            transform: scale(1);
        }

        .final-stats {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 20px;
            margin: 30px 0;
        }

        .final-stat {
            background: rgba(255, 255, 255, 0.05);
            border-radius: 15px;
            padding: 20px;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .final-stat-label {
            color: #a0a0ff;
            font-size: 0.9rem;
            margin-bottom: 5px;
        }

        .final-stat-value {
            color: #00f5ff;
            font-family: 'Orbitron', monospace;
            font-size: 1.5rem;
            font-weight: 700;
        }

        .restart-btn {
            background: linear-gradient(45deg, #667eea 0%, #764ba2 100%);
            border: none;
            border-radius: 15px;
            padding: 15px 40px;
            color: white;
            font-size: 1.2rem;
            font-weight: 600;
            cursor: pointer;
            margin-top: 20px;
            transition: all 0.3s ease;
        }

        .restart-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 15px 30px rgba(102, 126, 234, 0.4);
        }

        .start-screen {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.95);
            backdrop-filter: blur(30px);
            display: flex;
            align-items: center;
            justify-content: center;
            z-index: 3000;
            transition: all 0.5s ease;
        }

        .start-content {
            text-align: center;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(20px);
            border: 2px solid rgba(255, 255, 255, 0.2);
            border-radius: 25px;
            padding: 50px;
            max-width: 600px;
        }

        .start-title {
            font-family: 'Orbitron', monospace;
            font-size: 3rem;
            color: #f5ff00;
            margin-bottom: 20px;
            text-shadow: 0 0 30px rgba(245, 255, 0, 0.7);
        }

        .start-description {
            color: #ffffff;
            font-size: 1.2rem;
            margin-bottom: 30px;
            line-height: 1.6;
        }

        .start-btn {
            background: linear-gradient(45deg, #2ed573, #7bed9f);
            border: none;
            border-radius: 15px;
            padding: 20px 50px;
            color: white;
            font-size: 1.5rem;
            font-weight: 700;
            cursor: pointer;
            transition: all 0.3s ease;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        .start-btn:hover {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 20px 40px rgba(46, 213, 115, 0.4);
        }

        .streak-indicator {
            position: fixed;
            top: 20%;
            right: 5%;
            font-family: 'Orbitron', monospace;
            font-size: 1.2rem;
            color: #f5ff00;
            text-shadow: 0 0 15px rgba(245, 255, 0, 0.8);
            z-index: 1000;
            background: rgba(0, 0, 0, 0.3);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(245, 255, 0, 0.3);
            border-radius: 10px;
            padding: 15px;
            opacity: 0;
            transform: translateX(100px);
            transition: all 0.5s ease;
        }

        .streak-indicator.show {
            opacity: 1;
            transform: translateX(0);
        }

        @keyframes timeWarning {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }

        .time-warning {
            animation: timeWarning 0.5s infinite;
        }

        @media (max-width: 768px) {
            .game-title {
                font-size: 2rem;
            }
            
            .timer-display {
                font-size: 3rem;
            }
            
            .question-text {
                font-size: 1.4rem;
            }
            
            .answers-grid {
                grid-template-columns: 1fr;
            }
            
            .answer-btn {
                font-size: 1.1rem;
                padding: 20px;
            }
            
            .tournament-stats {
                grid-template-columns: repeat(2, 1fr);
            }
        }
    </style>
</head>
<body>
    <div class="stars"></div>
    
    <div class="start-screen" id="startScreen">
        <div class="start-content">
            <h1 class="start-title">TORNEO MATEMÁTICO</h1>
            <div class="start-description">
                <p><strong>¡Bienvenido al torneo de porcentajes!</strong></p>
                <p>• <strong>20 preguntas</strong> de matemáticas nivel secundaria</p>
                <p>• <strong>15 segundos</strong> por pregunta</p>
                <p>• Gana puntos por velocidad y precisión</p>
                <p>• ¡Compite por ser el mejor!</p>
            </div>
            <button class="start-btn" onclick="startGame()">¡COMENZAR TORNEO!</button>
        </div>
    </div>
    
    <div class="game-container" id="gameContainer" style="display: none;">
        <div class="game-header">
            <h1 class="game-title">TORNEO PERCENTAGE</h1>
            <p class="game-subtitle">Competencia Matemática Secundaria</p>
        </div>

        <div class="tournament-stats">
            <div class="stat-card">
                <div class="stat-label">Puntuación</div>
                <div class="stat-value" id="score">0</div>
            </div>
            <div class="stat-card">
                <div class="stat-label">Correctas</div>
                <div class="stat-value" id="correct">0</div>
            </div>
            <div class="stat-card">
                <div class="stat-label">Racha</div>
                <div class="stat-value" id="streak">0</div>
            </div>
            <div class="stat-card">
                <div class="stat-label">Precisión</div>
                <div class="stat-value" id="accuracy">100%</div>
            </div>
        </div>

        <div class="timer-card" id="timerCard">
            <div class="question-counter" id="questionCounter">Pregunta 1 de 20</div>
            <div class="timer-display" id="timerDisplay">15</div>
            <div style="color: #a0a0ff; font-size: 1rem;">segundos restantes</div>
        </div>

        <div class="question-card">
            <div class="question-text" id="questionText">Cargando pregunta...</div>
            <div class="answers-grid" id="answersGrid"></div>
            <div class="feedback" id="feedback"></div>
        </div>
    </div>

    <div class="streak-indicator" id="streakIndicator">
        <div>🔥 RACHA</div>
        <div id="streakCount" style="font-size: 1.5rem; margin-top: 5px;">0</div>
    </div>

    <div class="game-over" id="gameOver">
        <div class="game-over-content">
            <h2 style="font-family: 'Orbitron', monospace; font-size: 2.5rem; color: #f5ff00; margin-bottom: 20px;">¡TORNEO COMPLETADO!</h2>
            
            <div class="final-stats">
                <div class="final-stat">
                    <div class="final-stat-label">Puntuación Final</div>
                    <div class="final-stat-value" id="finalScore">0</div>
                </div>
                <div class="final-stat">
                    <div class="final-stat-label">Respuestas Correctas</div>
                    <div class="final-stat-value" id="finalCorrect">0/20</div>
                </div>
                <div class="final-stat">
                    <div class="final-stat-label">Precisión Final</div>
                    <div class="final-stat-value" id="finalAccuracy">0%</div>
                </div>
                <div class="final-stat">
                    <div class="final-stat-label">Mejor Racha</div>
                    <div class="final-stat-value" id="finalStreak">0</div>
                </div>
            </div>
            
            <div id="performanceMessage" style="font-size: 1.3rem; margin: 20px 0; font-weight: 600;"></div>
            
            <button class="restart-btn" onclick="restartGame()">Jugar de Nuevo</button>
        </div>
    </div>

    <script>
        // Game state
        let gameState = {
            score: 0,
            correct: 0,
            incorrect: 0,
            currentQuestion: 1,
            totalQuestions: 20,
            streak: 0,
            maxStreak: 0,
            timeLeft: 15,
            timer: null,
            answered: false,
            gameStarted: false
        };

        // Easy percentage questions for secondary level
        const easyQuestions = [
            {
                question: "¿Cuál es el 50% de 100?",
                correct: 50,
                options: [50, 25, 75, 40]
            },
            {
                question: "¿Cuál es el 25% de 80?",
                correct: 20,
                options: [20, 15, 25, 30]
            },
            {
                question: "¿Cuál es el 10% de 200?",
                correct: 20,
                options: [20, 10, 30, 25]
            },
            {
                question: "¿Cuál es el 20% de 150?",
                correct: 30,
                options: [30, 25, 35, 40]
            },
            {
                question: "¿Cuál es el 75% de 40?",
                correct: 30,
                options: [30, 25, 35, 20]
            },
            {
                question: "Si tienes 60 estudiantes y el 30% son chicas, ¿cuántas chicas hay?",
                correct: 18,
                options: [18, 20, 15, 12]
            },
            {
                question: "En una clase de 40 alumnos, el 25% faltó. ¿Cuántos faltaron?",
                correct: 10,
                options: [10, 8, 12, 15]
            },
            {
                question: "¿Cuál es el 15% de 120?",
                correct: 18,
                options: [18, 15, 20, 12]
            },
            {
                question: "Una pizza cuesta $80. Con 20% de descuento, ¿cuánto pagas?",
                correct: 64,
                options: [64, 60, 70, 56]
            },
            {
                question: "¿Cuál es el 40% de 90?",
                correct: 36,
                options: [36, 40, 30, 45]
            },
            {
                question: "¿Cuál es el 60% de 50?",
                correct: 30,
                options: [30, 25, 35, 20]
            },
            {
                question: "En un grupo de 80 personas, 20 son niños. ¿Qué porcentaje son niños?",
                correct: 25,
                options: [25, 20, 30, 15]
            },
            {
                question: "¿Cuál es el 35% de 60?",
                correct: 21,
                options: [21, 18, 24, 15]
            },
            {
                question: "Una camisa cuesta $120. Con 10% de descuento, ¿cuánto pagas?",
                correct: 108,
                options: [108, 110, 100, 105]
            },
            {
                question: "¿Cuál es el 80% de 25?",
                correct: 20,
                options: [20, 18, 22, 25]
            },
            {
                question: "De 200 libros, 50 son de ciencia. ¿Qué porcentaje son de ciencia?",
                correct: 25,
                options: [25, 20, 30, 15]
            },
            {
                question: "¿Cuál es el 45% de 80?",
                correct: 36,
                options: [36, 40, 32, 45]
            },
            {
                question: "Un examen vale 100 puntos. Si sacas el 85%, ¿cuántos puntos obtuviste?",
                correct: 85,
                options: [85, 80, 90, 75]
            },
            {
                question: "¿Cuál es el 30% de 70?",
                correct: 21,
                options: [21, 18, 24, 15]
            },
            {
                question: "En una encuesta a 100 personas, 65 prefieren pizza. ¿Qué porcentaje prefiere pizza?",
                correct: 65,
                options: [65, 60, 70, 55]
            }
        ];

        function createStars() {
            const starsContainer = document.querySelector('.stars');
            for (let i = 0; i < 100; i++) {
                const star = document.createElement('div');
                star.className = 'star';
                star.style.left = Math.random() * 100 + '%';
                star.style.top = Math.random() * 100 + '%';
                star.style.animationDelay = Math.random() * 3 + 's';
                starsContainer.appendChild(star);
            }
        }

        function startGame() {
            document.getElementById('startScreen').style.display = 'none';
            document.getElementById('gameContainer').style.display = 'block';
            
            gameState.gameStarted = true;
            gameState.currentQuestion = 1;
            
            updateUI();
            displayQuestion();
            startTimer();
        }

        function updateUI() {
            document.getElementById('score').textContent = gameState.score;
            document.getElementById('correct').textContent = gameState.correct;
            document.getElementById('streak').textContent = gameState.streak;
            
            const accuracy = gameState.currentQuestion > 1 ? 
                Math.round((gameState.correct / (gameState.currentQuestion - 1)) * 100) : 100;
            document.getElementById('accuracy').textContent = accuracy + '%';
            
            document.getElementById('questionCounter').textContent = 
                `Pregunta ${gameState.currentQuestion} de ${gameState.totalQuestions}`;
        }

        function displayQuestion() {
            if (gameState.currentQuestion > gameState.totalQuestions) {
                endGame();
                return;
            }

            const question = easyQuestions[Math.floor(Math.random() * easyQuestions.length)];
            gameState.currentQuestionData = question;
            gameState.answered = false;
            gameState.timeLeft = 15;

            document.getElementById('questionText').textContent = question.question;
            document.getElementById('feedback').className = 'feedback';

            const answersGrid = document.getElementById('answersGrid');
            answersGrid.innerHTML = '';

            // Shuffle options
            const shuffledOptions = [...question.options].sort(() => Math.random() - 0.5);

            shuffledOptions.forEach(option => {
                const btn = document.createElement('button');
                btn.className = 'answer-btn';
                btn.textContent = option;
                btn.onclick = () => selectAnswer(option, btn);
                answersGrid.appendChild(btn);
            });

            startTimer();
        }

        function startTimer() {
            clearInterval(gameState.timer);
            updateTimerDisplay();

            gameState.timer = setInterval(() => {
                gameState.timeLeft--;
                updateTimerDisplay();

                if (gameState.timeLeft <= 0) {
                    timeUp();
                }
            }, 1000);
        }

        function updateTimerDisplay() {
            const timerDisplay = document.getElementById('timerDisplay');
            const timerCard = document.getElementById('timerCard');
            
            timerDisplay.textContent = gameState.timeLeft;

            // Visual feedback based on time left
            timerDisplay.className = 'timer-display';
            timerCard.className = 'timer-card';

            if (gameState.timeLeft <= 5) {
                timerDisplay.className = 'timer-display danger';
                timerCard.className = 'timer-card danger';
            } else if (gameState.timeLeft <= 10) {
                timerDisplay.className = 'timer-display warning';
                timerCard.className = 'timer-card warning';
            }

            if (gameState.timeLeft <= 3 && gameState.timeLeft > 0) {
                timerCard.classList.add('time-warning');
            }
        }

        function selectAnswer(selected, btn) {
            if (gameState.answered) return;
            
            clearInterval(gameState.timer);
            gameState.answered = true;
            
            const correct = gameState.currentQuestionData.correct;
            const isCorrect = selected === correct;

            // Mark all buttons
            document.querySelectorAll('.answer-btn').forEach(button => {
                if (parseInt(button.textContent) === correct || parseFloat(button.textContent) === correct) {
                    button.classList.add('correct');
                } else if (button === btn && !isCorrect) {
                    button.classList.add('incorrect');
                }
                button.style.pointerEvents = 'none';
            });

            // Show feedback
            const feedback = document.getElementById('feedback');
            if (isCorrect) {
                gameState.correct++;
                gameState.streak++;
                gameState.maxStreak = Math.max(gameState.maxStreak, gameState.streak);
                
                // Calculate score based on time left (bonus for speed)
                const timeBonus = gameState.timeLeft * 2;
                const streakBonus = gameState.streak > 1 ? (gameState.streak - 1) * 5 : 0;
                const totalPoints = 100 + timeBonus + streakBonus;
                
                gameState.score += totalPoints;
                
                feedback.textContent = `¡Correcto! +${totalPoints} puntos`;
                if (gameState.streak > 1) {
                    feedback.textContent += ` 🔥 Racha x${gameState.streak}!`;
                }
                feedback.className = 'feedback correct show';
                
                createParticles(btn);
                
                if (gameState.streak > 1) {
                    showStreak(gameState.streak);
                }
            } else {
                gameState.incorrect++;
                gameState.streak = 0;
                feedback.textContent = `❌ Incorrecto. La respuesta era ${correct}`;
                feedback.className = 'feedback incorrect show';
            }

            updateUI();
            
            // Auto advance to next question after 2 seconds
            setTimeout(() => {
                gameState.currentQuestion++;
                displayQuestion();
                
                // Reset feedback
                setTimeout(() => {
                    document.getElementById('feedback').className = 'feedback';
                }, 100);
            }, 2000);
        }

        function timeUp() {
            if (gameState.answered) return;
            
            clearInterval(gameState.timer);
            gameState.answered = true;
            gameState.incorrect++;
            gameState.streak = 0;

            // Mark correct answer
            const correct = gameState.currentQuestionData.correct;
            document.querySelectorAll('.answer-btn').forEach(button => {
                if (parseInt(button.textContent) === correct || parseFloat(button.textContent) === correct) {
                    button.classList.add('correct');
                }
                button.style.pointerEvents = 'none';
            });

            const feedback = document.getElementById('feedback');
            feedback.textContent = `⏰ ¡Tiempo agotado! La respuesta era ${correct}`;
            feedback.className = 'feedback incorrect show';

            updateUI();

            // Auto advance to next question
            setTimeout(() => {
                gameState.currentQuestion++;
                displayQuestion();
                
                setTimeout(() => {
                    document.getElementById('feedback').className = 'feedback';
                }, 100);
            }, 2000);
        }

        function showStreak(streakCount) {
            const streakIndicator = document.getElementById('streakIndicator');
            document.getElementById('streakCount').textContent = streakCount;
            
            streakIndicator.classList.add('show');
            
            setTimeout(() => {
                streakIndicator.classList.remove('show');
            }, 3000);
        }

        function createParticles(element) {
            const rect = element.getBoundingClientRect();
            const colors = ['#00f5ff', '#ff00f5', '#f5ff00', '#2ed573'];
            
            for (let i = 0; i < 12; i++) {
                const particle = document.createElement('div');
                particle.style.position = 'fixed';
                particle.style.width = '8px';
                particle.style.height = '8px';
                particle.style.background = colors[Math.floor(Math.random() * colors.length)];
                particle.style.borderRadius = '50%';
                particle.style.pointerEvents = 'none';
                particle.style.zIndex = '9999';
                particle.style.left = rect.left + rect.width / 2 + Math.random() * 60 - 30 + 'px';
                particle.style.top = rect.top + rect.height / 2 + Math.random() * 60 - 30 + 'px';
                
                const animation = particle.animate([
                    { transform: 'translateY(0) scale(1)', opacity: 1 },
                    { transform: `translateY(-${100 + Math.random() * 100}px) scale(0)`, opacity: 0 }
                ], {
                    duration: 1000 + Math.random() * 500,
                    easing: 'ease-out'
                });
                
                document.body.appendChild(particle);
                
                animation.onfinish = () => particle.remove();
            }
        }

        function endGame() {
            clearInterval(gameState.timer);
            
            // Calculate final stats
            const finalAccuracy = Math.round((gameState.correct / gameState.totalQuestions) * 100);
            
            document.getElementById('finalScore').textContent = gameState.score;
            document.getElementById('finalCorrect').textContent = `${gameState.correct}/${gameState.totalQuestions}`;
            document.getElementById('finalAccuracy').textContent = finalAccuracy + '%';
            document.getElementById('finalStreak').textContent = gameState.maxStreak;
            
            // Performance message
            const performanceMsg = document.getElementById('performanceMessage');
            let message = '';
            let messageColor = '';
            
            if (finalAccuracy >= 90) {
                message = '🏆 ¡EXCELENTE! Eres un maestro de los porcentajes';
                messageColor = '#f5ff00';
            } else if (finalAccuracy >= 75) {
                message = '🌟 ¡MUY BIEN! Gran dominio de las matemáticas';
                messageColor = '#2ed573';
            } else if (finalAccuracy >= 60) {
                message = '👍 ¡BIEN HECHO! Sigue practicando';
                messageColor = '#00f5ff';
            } else if (finalAccuracy >= 40) {
                message = '📚 ¡BUEN INTENTO! La práctica hace al maestro';
                messageColor = '#ffa500';
            } else {
                message = '💪 ¡NO TE RINDAS! Cada error es una oportunidad de aprender';
                messageColor = '#ff4757';
            }
            
            performanceMsg.textContent = message;
            performanceMsg.style.color = messageColor;
            performanceMsg.style.textShadow = `0 0 15px ${messageColor}`;
            
            document.getElementById('gameOver').classList.add('show');
        }

        function restartGame() {
            // Reset game state
            gameState = {
                score: 0,
                correct: 0,
                incorrect: 0,
                currentQuestion: 1,
                totalQuestions: 20,
                streak: 0,
                maxStreak: 0,
                timeLeft: 15,
                timer: null,
                answered: false,
                gameStarted: false
            };
            
            // Hide game over screen
            document.getElementById('gameOver').classList.remove('show');
            
            // Show start screen
            document.getElementById('startScreen').style.display = 'flex';
            document.getElementById('gameContainer').style.display = 'none';
            
            // Clear any running timers
            clearInterval(gameState.timer);
        }

        // Initialize game
        document.addEventListener('DOMContentLoaded', () => {
            createStars();
        });

        // Keyboard shortcuts
        document.addEventListener('keydown', (e) => {
            if (!gameState.gameStarted || gameState.answered) return;
            
            const buttons = document.querySelectorAll('.answer-btn');
            if (e.key >= '1' && e.key <= '4') {
                const buttonIndex = parseInt(e.key) - 1;
                if (buttons[buttonIndex]) {
                    buttons[buttonIndex].click();
                }
            }
        });

        // Prevent page refresh during game
        window.addEventListener('beforeunload', (e) => {
            if (gameState.gameStarted && gameState.currentQuestion <= gameState.totalQuestions) {
                e.preventDefault();
                e.returnValue = '';
            }
        });
    </script>
</body>
</html>
