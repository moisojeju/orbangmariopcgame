<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>오르방 슈퍼마리오</title>
    <link rel="stylesheet" href="orbang-mario.css">
</head>
<body>
    <div class="game-container">
        <div class="game-header">
            <div class="hud">
                <div class="hud-left">
                    <div>점수: <span id="score">0</span></div>
                    <div class="coins">코인: <span id="coins">0</span></div>
                </div>
                <div class="hud-center">
                    <div>월드 <span id="level">1-1</span></div>
                    <div class="character-name">오르방</div>
                </div>
                <div class="hud-right">
                    <div>생명: <span id="lives">3</span></div>
                    <div>시간: <span id="time">400</span></div>
                </div>
            </div>
        </div>
        
        <canvas id="gameCanvas" width="1000" height="600"></canvas>
        
        <div class="game-controls">
            <button id="startBtn">게임 시작</button>
            <button id="pauseBtn">일시정지</button>
            <button id="resetBtn">다시 시작</button>
        </div>
        
        <div class="instructions">
            <p>조작법: 화살표 키 또는 WASD로 이동, 스페이스바로 점프! 적을 밟아서 처치하고 코인을 모으세요!</p>
        </div>
        
        <div id="gameOver" class="game-over hidden">
            <h2>게임 오버!</h2>
            <p>오르방이 쓰러졌습니다...</p>
            <p>최종 점수: <span id="finalScore">0</span></p>
            <p>수집한 코인: <span id="finalCoins">0</span></p>
            <button id="restartBtn">다시 도전</button>
        </div>
        
        <div id="levelComplete" class="level-complete hidden">
            <h2>스테이지 클리어!</h2>
            <p>오르방이 해냈습니다!</p>
            <p>보너스 점수: <span id="bonusScore">0</span></p>
            <button id="nextLevelBtn">다음 스테이지</button>
        </div>
        
        <div id="powerUp" class="power-up-notification hidden">
            <h3>파워업!</h3>
            <p>오르방이 더 강해졌습니다!</p>
        </div>
    </div>
    
    <script src="orbang-mario.js"></script>
</body>
</html>
