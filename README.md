
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Евгений & Алёна | 14.06.2025</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Montserrat:wght@300;400&display=swap" rel="stylesheet">
    <style>
        :root {
            --gold: #d4af37;
            --rose: #f8d7da;
            --dark: #333;
        }
        body {
            font-family: 'Montserrat', sans-serif;
            margin: 0;
            padding: 0;
            background: #fff9fb;
            color: var(--dark);
            overflow-x: hidden;
        }
        .heart {
            color: #ff6b6b;
        }
        header {
            background: linear-gradient(rgba(0,0,0,0.3), rgba(0,0,0,0.3)), url('https://images.unsplash.com/photo-1519225421980-715cb0215aed?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
        }
        h1 {
            font-family: 'Playfair Display', serif;
            font-size: 4rem;
            margin: 0;
            animation: fadeIn 2s;
        }
        .date {
            font-size: 1.8rem;
            margin: 20px 0;
            letter-spacing: 3px;
            animation: fadeIn 2s 0.5s both;
        }
        .names {
            display: flex;
            align-items: center;
            gap: 20px;
            margin-bottom: 30px;
            animation: fadeIn 2s 1s both;
        }
        .names span {
            font-size: 2rem;
        }
        .timer {
            display: flex;
            gap: 15px;
            margin: 40px 0;
            animation: fadeIn 2s 1.5s both;
        }
        .timer-item {
            background: rgba(255,255,255,0.2);
            padding: 15px;
            border-radius: 5px;
            min-width: 80px;
        }
        .timer-number {
            font-size: 2rem;
            font-weight: bold;
        }        
        section {
            padding: 80px 20px;
            max-width: 1000px;
            margin: 0 auto;
        }       
        .section-title {
            font-family: 'Playfair Display', serif;
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 50px;
            color: var(--gold);
        }        
        .program {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 30px;
        }        
        .program-item {
            flex: 1;
            min-width: 250px;
            text-align: center;
            padding: 30px;
            background: white;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }        
        .program-item:hover {
            transform: translateY(-10px);
        }       
        .program-item h3 {
            color: var(--gold);
        }        
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 40px;
        }        
        .gallery img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px;
            transition: transform 0.3s;
            cursor: pointer;
        }        
        .gallery img:hover {
            transform: scale(1.05);
        }        
        .rsvp {
            background: var(--rose);
            padding: 50px 20px;
            text-align: center;
        }        
        .rsvp-form {
            max-width: 500px;
            margin: 0 auto;
        }       
        .form-group {
            margin-bottom: 20px;
            text-align: left;
        }       
        input, textarea, select {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-family: inherit;
        }       
        button {
            background: var(--gold);
            color: white;
            border: none;
            padding: 15px 40px;
            font-size: 1rem;
            border-radius: 50px;
            cursor: pointer;
            transition: background 0.3s;
        }        
        button:hover {
            background: #c9a227;
        }   
        footer {
            text-align: center;
            padding: 30px;
            background: var(--dark);
            color: white;
        }        
        .contacts {
            margin-top: 20px;
            font-size: 1.1rem;
        }       
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }    
        @media (max-width: 768px) {
            h1 {
                font-size: 2.5rem;
            }         
            .names {
                flex-direction: column;
                gap: 5px;
            }            
            .timer {
                flex-wrap: wrap;
                justify-content: center;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Евгений <span class="heart">❤</span> Алёна</h1>
        <div class="date">14 ИЮНЯ 2025</div>
        <div class="names">
            <span>Евгений</span>
            <span class="heart">❤</span>
            <span>Алёна</span>
        </div>
        <div class="timer" id="timer">
            <div class="timer-item">
                <div class="timer-number" id="days">00</div>
                <div>дней</div>
            </div>
            <div class="timer-item">
                <div class="timer-number" id="hours">00</div>
                <div>часов</div>
            </div>
            <div class="timer-item">
                <div class="timer-number" id="minutes">00</div>
                <div>минут</div>
            </div>
            <div class="timer-item">
                <div class="timer-number" id="seconds">00</div>
                <div>секунд</div>
            </div>
        </div>
    </header>    
    <section id="about">
        <h2 class="section-title">Наша история</h2>
        <p style="text-align: center; max-width: 700px; margin: 0 auto; line-height: 1.6;">
            Мы рады пригласить вас на нашу свадьбу, которая состоится 14 июня 2025 года. 
            Этот день станет началом нашей новой жизни вместе, и нам очень хочется разделить 
            эту радость с вами — нашими родными и друзьями.
        </p>
    </section>   
    <section id="program">
        <h2 class="section-title">Программа дня</h2>
        <div class="program">
            <div class="program-item">
                <h3>Церемония</h3>
                <p>15:30</p>
                <p>ЗАГС Прикубанского округа</p>
            </div>
            <div class="program-item">
                <h3>Фуршет и выездная регистрация</h3>
                <p>17:00</p>
                <p>Частный дом</p>
            </div>
            <div class="program-item">
                <h3>Банкет</h3>
                <p>18:00</p>
                <p>Частный дом</p>
            </div>
        </div>
    </section> 
    <section id="location">
        <h2 class="section-title">Место проведения</h2>
        <div style="text-align: center; margin-bottom: 30px;">
            <p><strong>Банкет и фуршет:</strong></p>
            <p>г. Краснодар, ул. Светлая, 65</p>
            <p>(Частный дом)</p>
        </div>
        <iframe 
            src="https://yandex.ru/map-widget/v1/?um=constructor%3A8a5d5e5e5e5e5e5e5e5e5e5e5e5e5e5&amp;source=constructor" 
            width="100%" 
            height="400" 
            frameborder="0"
            style="border-radius: 10px;"
        ></iframe>
    </section> 
    <section id="gallery">
        <h2 class="section-title">Наши моменты</h2>
        <div class="gallery">
            <img src="https://images.unsplash.com/photo-1518621736915-f3b1c41bfd00?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Фото 1">
            <img src="https://images.unsplash.com/photo-1519225421980-715cb0215aed?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Фото 2">
            <img src="https://images.unsplash.com/photo-1523438885200-e635ba2c371e?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Фото 3">
            <img src="https://images.unsplash.com/photo-1518895949257-7621c3c786d7?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Фото 4">
        </div>
    </section>  
    <section class="rsvp" id="rsvp">
        <h2 class="section-title">Подтвердите участие</h2>
        <form class="rsvp-form" id="weddingForm">
            <div class="form-group">
                <label for="name">Ваше имя</label>
                <input type="text" id="name" required>
            </div>
            <div class="form-group">
                <label for="guests">Количество гостей</label>
                <select id="guests">
                    <option value="1">1</option>
                    <option value="2">2</option>
                    <option value="3">3</option>
                    <option value="4">4</option>
                    <option value="5+">5+</option>
                </select>
            </div>
            <div class="form-group">
                <label for="message">Ваши пожелания</label>
                <textarea id="message" rows="4"></textarea>
            </div>
            <button type="submit">Подтвердить</button>
        </form>
    </section>   
    <footer>
        <p>С любовью, Евгений и Алёна</p>
        <div class="contacts">
            <p>По всем вопросам: 8 (905) 402-50-10 </p>                    
        </div>
    </footer>  
    <script>
        // Таймер до свадьбы
        function updateTimer() {
            const weddingDate = new Date('June 14, 2025 15:30:00').getTime();
            const now = new Date().getTime();
            const diff = weddingDate - now;            
            const days = Math.floor(diff / (1000 * 60 * 60 * 24));
            const hours = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
            const seconds = Math.floor((diff % (1000 * 60)) / 1000);            
            document.getElementById('days').textContent = days.toString().padStart(2, '0');
            document.getElementById('hours').textContent = hours.toString().padStart(2, '0');
            document.getElementById('minutes').textContent = minutes.toString().padStart(2, '0');
            document.getElementById('seconds').textContent = seconds.toString().padStart(2, '0');
        } 
        setInterval(updateTimer, 1000);
        updateTimer();
        // Отправка в Telegram
        document.getElementById('weddingForm').addEventListener('submit', async function(e) {
            e.preventDefault();
            const name = document.getElementById('name').value;
            const guests = document.getElementById('guests').value;
            const message = document.getElementById('message').value;     
            const botToken = '+79054025010';
            const chatId = '483128250'; // Замените на ваш chat_id 
            const text = `🎉 Новый отклик на свадьбу!\nИмя: ${name}\nГостей: ${guests}\nПожелания: ${message || 'нет'}\n\nНе забудьте перезвонить: 8 (905) 402-50-10`;     
            try {
                await fetch(`https://api.telegram.org/bot${botToken}/sendMessage?chat_id=${chatId}&text=${encodeURIComponent(text)}`);
                alert('Спасибо! Ваше участие подтверждено. Ждём вас 14 июня!');
                this.reset();
            } catch (error) {
                alert('Ошибка отправки. Пожалуйста, свяжитесь с нами по телефону.');
                console.error(error);
            }
        });
    </script>
</body>
</html>
