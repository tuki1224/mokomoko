<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>キラキラとハートのマウスエフェクト</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            overflow: hidden; /* スクロールバーを隠す */
            background-color: #0d0d0d; /* 背景は暗め */
            height: 100vh;
        }

        /* 共通のパーティクルスタイル */
        .particle {
            position: absolute;
            pointer-events: none; /* マウス操作を邪魔しない */
            z-index: 9999;
            animation: fly-and-fade 1.2s forwards ease-out;
            will-change: transform, opacity; /* パフォーマンス最適化 */
        }

        /* キラキラ（丸）のスタイル */
        .sparkle {
            width: 7px;
            height: 7px;
            border-radius: 50%;
        }

        /* ハートのスタイル */
        .heart {
            font-size: 20px; /* ハートの大きさ */
            user-select: none;
            /* 初期の向きを少し変えるなど */
            transform: rotate(-10deg);
        }

        /* 飛び散って消えるアニメーション */
        @keyframes fly-and-fade {
            0% {
                transform: translate(0, 0) rotate(0deg) scale(1);
                opacity: 1;
            }
            100% {
                /* ランダムな方向に散る設定はJS側で行う */
                /* transformはJSで上書きされるため、ここでは主にアニメーションの進行を定義 */
                transform: translate(var(--dx), var(--dy)) rotate(var(--dr)) scale(0);
                opacity: 0;
            }
        }
    </style>
</head>
<body>

    <script>
        // マウスの移動イベントを検知
        document.addEventListener('mousemove', function(e) {
            // 一度に生成する粒子の数（キラキラとハートの合計）
            const particleCount = 4;

            for (let i = 0; i < particleCount; i++) {
                // ランダムで「キラキラ」か「ハート」を決める (50%ずつ)
                if (Math.random() > 0.5) {
                    createSparkle(e.pageX, e.pageY);
                } else {
                    createHeart(e.pageX, e.pageY);
                }
            }
        });

        // 基本的な設定を行う関数
        function setParticleAnimationDetails(el, x, y, sizeOffset) {
            el.classList.add('particle');

            // 出現位置をマウス位置の周囲に少しランダム化
            const offset = 10;
            const startX = x + (Math.random() - 0.5) * offset;
            const startY = y + (Math.random() - 0.5) * offset;

            el.style.left = startX + 'px';
            el.style.top = startY + 'px';

            // 飛び散る方向と回転をランダムに設定（CSS変数に渡す）
            const dx = (Math.random() - 0.5) * 150 + 'px'; // 飛び散る横幅
            const dy = (Math.random() - 0.5) * 150 + 'px'; // 飛び散る縦幅
            const dr = (Math.random() - 0.5) * 360 + 'deg'; // 回転

            el.style.setProperty('--dx', dx);
            el.style.setProperty('--dy', dy);
            el.style.setProperty('--dr', dr);

            // アニメーション終了後に要素を削除 (CSSのanimation-durationと合わせる)
            setTimeout(() => {
                el.remove();
            }, 1200);
        }

        // キラキラ（丸）を生成
        function createSparkle(x, y) {
            const sparkle = document.createElement('div');
            sparkle.classList.add('sparkle');

            // キラキラの色（ゴールド、白、パステル）
            const colors = ['#FFD700', '#FFFFFF', '#FF69B4', '#87CEEB'];
            const color = colors[Math.floor(Math.random() * colors.length)];
            
            sparkle.style.backgroundColor = color;
            // 光彩エフェクト
            sparkle.style.boxShadow = `0 0 8px ${color}, 0 0 15px ${color}`;

            setParticleAnimationDetails(sparkle, x, y);
            document.body.appendChild(sparkle);
        }

        // ハートを生成
        function createHeart(x, y) {
            const heart = document.createElement('div');
            heart.classList.add('heart');
            heart.innerText = '❤'; // ハートマーク

            // ハートの色（ピンク、赤、白）
            const colors = ['#FF1493', '#FF69B4', '#FFB6C1', '#FFFFFF', '#FF0000'];
            const color = colors[Math.floor(Math.random() * colors.length)];
            
            heart.style.color = color;
            // ハートにも少し光沢
            heart.style.textShadow = `0 0 5px ${color}, 0 0 10px ${color}`;

            setParticleAnimationDetails(heart, x, y);
            document.body.appendChild(heart);
        }
    </script>
</body>
</html>
