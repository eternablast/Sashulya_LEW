<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>С Днём Рождения, Саша!</title>
    <style>
        @keyframes shimmer {
            0% { background-position: -1000px; }
            100% { background-position: 1000px; }
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }
        
        body {
            margin: 0;
            padding: 0;
            font-family: 'Arial', sans-serif;
            background: linear-gradient(45deg, #d4af37, #f9d74f, #c5a82f, #f9d74f, #d4af37);
            background-size: 1000% 1000%;
            animation: shimmer 8s ease infinite;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            color: #8b5a2b;
            text-align: center;
        }
        
        .container {
            max-width: 800px;
            width: 90%;
            padding: 30px;
            border-radius: 20px;
            background: rgba(255, 255, 255, 0.2);
            backdrop-filter: blur(10px);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3), 
                        0 0 20px rgba(255, 215, 0, 0.4),
                        0 0 40px rgba(255, 215, 0, 0.3);
            border: 2px solid rgba(255, 255, 255, 0.3);
            transform: translateY(0);
            animation: pulse 3s ease-in-out infinite;
        }
        
        h1 {
            font-size: 3.5rem;
            margin-bottom: 30px;
            text-shadow: 0 0 10px rgba(255, 215, 0, 0.8),
                         0 0 20px rgba(255, 215, 0, 0.6),
                         0 0 30px rgba(255, 215, 0, 0.4);
            color: #8b4513;
            font-weight: bold;
            letter-spacing: 2px;
            text-transform: uppercase;
        }
        
        .image-container {
            margin: 20px 0;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
            border: 3px solid rgba(255, 215, 0, 0.6);
            transition: transform 0.3s ease;
        }
        
        .image-container:hover {
            transform: scale(1.03);
        }
        
        img {
            width: 100%;
            height: auto;
            display: block;
        }
        
        .audio-container {
            margin-top: 30px;
            padding: 20px;
            background: rgba(255, 255, 255, 0.15);
            border-radius: 15px;
            border: 2px solid rgba(255, 215, 0, 0.4);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .audio-title {
            margin-bottom: 15px;
            color: #8b4513;
            font-size: 1.3rem;
            font-weight: bold;
        }
        
        audio {
            width: 100%;
        }
        
        .download-link {
            display: block;
            margin-top: 15px;
            color: #d4af37;
            text-decoration: underline;
            font-size: 0.9rem;
        }
        
        .sparkle {
            position: absolute;
            width: 10px;
            height: 10px;
            background: rgba(255, 255, 255, 0.8);
            border-radius: 50%;
            pointer-events: none;
            z-index: 1;
            box-shadow: 0 0 8px rgba(255, 215, 0, 0.8);
        }
        
        @media (max-width: 768px) {
            h1 {
                font-size: 2.5rem;
            }
            
            .container {
                padding: 20px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Саша, с днём рождения!</h1>
        
        <div class="image-container">
            <img src="https://i.pinimg.com/736x/fa/e4/cd/fae4cdcefb93e15f539dd39d7da7b514.jpg" alt="Поздравительное изображение">
        </div>
        
        <div class="audio-container">
