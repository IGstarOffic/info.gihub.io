<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Мой Сайт</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" integrity="sha512-9usAa10IRO0HhonpyAIVpjrylPvoDwiPUiKdWk5t3PyolY1cOd4DSE0Ga+ri4AuTroPR5aQvXU9xC6qOPnzFeg==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <style>
        body {
            font-family: 'Open Sans', sans-serif;
            background: linear-gradient(to bottom, #e0eafc, #673ab7); /* Gradient background */
            margin: 0;
            padding: 0;
            line-height: 1.6;
            color: #333;
            display: flex;
            flex-direction: column;
            align-items: center;
            min-height: 100vh;
            overflow-x: hidden; /* Prevent horizontal scroll */
        }

        .container {
            background-color: rgba(255, 255, 255, 0.9); /* Semi-transparent white */
            border-radius: 12px;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
            padding: 40px;
            width: 80%;
            max-width: 800px;
            margin-bottom: 40px;
            transition: all 0.3s ease; /* Smooth transitions */
            transform: translateY(0);
        }

        .container:hover {
            transform: translateY(-5px); /* Slight lift on hover */
            box-shadow: 0 12px 25px rgba(0, 0, 0, 0.3);
        }

        h1, h2 {
            color: #4a148c; /* Darker purple */
            margin-bottom: 20px;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.1);
            font-weight: 700; /* Bold font */
        }

        a {
            color: #7b1fa2; /* Lighter purple */
            text-decoration: none;
            transition: color 0.3s ease;
        }

        a:hover {
            text-decoration: underline;
            color: #ba68c8; /* Even lighter purple */
        }

        .bot-item {
            border: 1px solid #ddd;
            padding: 20px;
            border-radius: 8px;
            margin-bottom: 20px;
            background-color: #f9f9f9;
            transition: transform 0.2s ease;
        }

        .bot-item:hover {
            transform: scale(1.02); /* Slight zoom on hover */
        }

        .bot-item h3 {
            color: #7b1fa2;
            margin-bottom: 10px;
        }

        footer {
            text-align: center;
            margin-top: 40px;
            color: #eee;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.3);
        }

        /* Keyframes for subtle animations */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes slideInLeft {
            from { transform: translateX(-100%); }
            to { transform: translateX(0); }
        }

        /* Apply animations */
        body {
            animation: fadeIn 1s ease-out;
        }

        .container:nth-child(odd) {
            animation: slideInLeft 1s ease-out;
        }

        /* Add Font Awesome Icons */
        .bot-item a { /* убрал ::before для корректной работы с иконкой */
            /* Ничего не меняем, просто поправляем код */
        }

        .container h1::before {
            content: '\f007'; /* User icon */
            font-family: FontAwesome;
            margin-right: 10px;
            color: #4a148c;
        }

        .container h2::before {
            content: '\f12e'; /* Bot icon */
            font-family: FontAwesome;
            margin-right: 10px;
            color: #4a148c;
        }
        .bot-item h3::before {
            content: '\f12e'; /* Bot icon */
            font-family: FontAwesome;
            margin-right: 5px;
            color: #7b1fa2;
        }

        .bot-item a::before {
            content: '\f1d8'; /* Telegram icon */
            font-family: FontAwesome;
            margin-right: 5px;
            color: #7b1fa2;
        }

    </style>
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>

    <div class="container">
        <h1>Всем привет!</h1>
        <p>Здесь информация обо мне и моих ботах!</p>
    </div>

    <div class="container">
        <h2>Обо мне</h2>
        <p>Я - разработчик ботов. Мне нравится создавать полезные и интересные инструменты для людей. Моя цель - автоматизировать рутинные задачи, упростить доступ к информации и сделать повседневную жизнь более эффективной. Я всегда ищу новые способы улучшить функциональность и удобство использования моих ботов, чтобы они приносили максимальную пользу.</p>
    </div>

    <div class="container">
        <h2>Мои боты</h2>

        <div class="bot-item">
            <h3>Бот 1: english-for-kids | video</h3>
            <p>Привет👋! Я покажу тебе английские видео!</p>
            <a href="http://t.me//EnglishForKidsVideoBot"> Запустить</a>
        </div>

    </div>

    <footer>
        <p>©2025 IGstarOffic</p>
    </footer>

</body>
</html>
