<script type="text/javascript">
        var gk_isXlsx = false;
        var gk_xlsxFileLookup = {};
        var gk_fileData = {};
        function filledCell(cell) {
          return cell !== '' && cell != null;
        }
        function loadFileData(filename) {
        if (gk_isXlsx && gk_xlsxFileLookup[filename]) {
            try {
                var workbook = XLSX.read(gk_fileData[filename], { type: 'base64' });
                var firstSheetName = workbook.SheetNames[0];
                var worksheet = workbook.Sheets[firstSheetName];

                // Convert sheet to JSON to filter blank rows
                var jsonData = XLSX.utils.sheet_to_json(worksheet, { header: 1, blankrows: false, defval: '' });
                // Filter out blank rows (rows where all cells are empty, null, or undefined)
                var filteredData = jsonData.filter(row => row.some(filledCell));

                // Heuristic to find the header row by ignoring rows with fewer filled cells than the next row
                var headerRowIndex = filteredData.findIndex((row, index) =>
                  row.filter(filledCell).length >= filteredData[index + 1]?.filter(filledCell).length
                );
                // Fallback
                if (headerRowIndex === -1 || headerRowIndex > 25) {
                  headerRowIndex = 0;
                }

                // Convert filtered JSON back to CSV
                var csv = XLSX.utils.aoa_to_sheet(filteredData.slice(headerRowIndex)); // Create a new sheet from filtered array of arrays
                csv = XLSX.utils.sheet_to_csv(csv, { header: 1 });
                return csv;
            } catch (e) {
                console.error(e);
                return "";
            }
        }
        return gk_fileData[filename] || "";
        }
        </script><!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ananas_Vitalya - Король The Strongest Battlegrounds</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        @keyframes glow {
            0% { text-shadow: 0 0 10px #ffd700; }
            50% { text-shadow: 0 0 20px #ffd700, 0 0 30px #ff4500; }
            100% { text-shadow: 0 0 10px #ffd700; }
        }
        .animate-fadeIn {
            animation: fadeIn 1s ease-out;
        }
        .animate-glow {
            animation: glow 2s infinite;
        }
        .hover-scale {
            transition: transform 0.3s ease;
        }
        .hover-scale:hover {
            transform: scale(1.05);
        }
    </style>
</head>
<body class="bg-gray-900 text-white font-sans">
    <!-- Header -->
    <header class="bg-gradient-to-r from-blue-600 to-red-600 py-16 text-center">
        <h1 class="text-5xl md:text-6xl font-bold animate-fadeIn animate-glow">
            Ananas_Vitalya
        </h1>
        <p class="mt-4 text-xl md:text-2xl animate-fadeIn delay-200">
            Я — ЛЕГЕНДА <span class="text-yellow-300">The Strongest Battlegrounds</span> 🔥
        </p>
        <p class="mt-2 text-lg animate-fadeIn delay-300">
            Roblox ID: <span class="font-bold">Ananas_Vitalya (4476830117)</span>
        </p>
        <div class="mt-6 flex justify-center items-center space-x-4 animate-fadeIn delay-400">
            <span class="text-lg bg-green-500 text-white px-4 py-2 rounded-full flex items-center">
                <svg class="w-5 h-5 mr-2" fill="currentColor" viewBox="0 0 24 24">
                    <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10-4.48 10-10S17.52 2 12 2zm-1 15.5l-5-5 1.41-1.41L11 14.67l6.59-6.59L19 9.5l-8 8z"/>
                </svg>
                Verified Badge
            </span>
            <span class="text-lg bg-blue-500 text-white px-4 py-2 rounded-full">
                Maturity: Mild
            </span>
        </div>
    </header>

    <!-- About Ananas_Vitalya -->
    <section class="py-16 px-4 md:px-16 bg-gray-800">
        <div class="max-w-6xl mx-auto">
            <h2 class="text-4xl font-bold text-center mb-8 animate-fadeIn">
                Я — Ananas_Vitalya, ПАДИТЕ НИЦ! 😎
            </h2>
            <div class="flex flex-col md:flex-row items-center">
                <img src="https://via.placeholder.com/300x300.png?text=Ananas_Vitalya+Avatar" alt="Ananas_Vitalya Avatar" class="w-64 h-64 rounded-full mb-8 md:mb-0 md:mr-8 hover-scale">
                <div class="text-lg animate-fadeIn delay-200">
                    <p>
                        Слушайте сюда, нубы! Я — <strong>Ananas_Vitalya</strong> (ID: <strong>4476830117</strong>), и я РАЗРЫВАЮ всех в <em>The Strongest Battlegrounds</em>! 😈 Мои комбо такие чёткие, что противники просто в шоке падают, а мои ультимейты — это чистый АРТ! Воин, Техногений, да хоть кто — я всех их юзаю на МАКСИМУМ! Я не просто играю, я УНИЧТОЖАЮ, понял?
                    </p>
                    <p class="mt-4">
                        У меня Verified Badge, это как корона на моей голове! 😎 Я — топ-1, легенда, которую все знают. Захожу в игру, и все уже бегут прятаться, потому что знают: Ananas_Vitalya пришёл, и щас будет ЖЕСТЬ! Хочешь попробовать меня завалить? Пфф, удачи, лол, ты даже не близко! Ищи меня в Roblox, но готовься к тому, что я тебя размажу за секунду. 😏
                    </p>
                    <p class="mt-4">
                        Я уже набил тыщи побед, мои скиллы — это просто космос! Каждый бой — это шоу, где я главный герой. Нубы плачут, просят пощады, но я такой: "Сорри, братишка, это не мой стиль!" 😆 Если хочешь хоть чуть-чуть стать как я, учись у короля, но знай: до моего уровня тебе как до луны пешком!
                    </p>
                    <a href="https://www.roblox.com/users/4476830117/profile" target="_blank" class="mt-6 inline-block bg-blue-600 text-white px-6 py-3 rounded-lg hover:bg-blue-700 hover-scale">
                        Кланяйся Ananas_Vitalya в Roblox
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- About The Strongest Battlegrounds -->
    <section class="py-16 px-4 md:px-16 bg-gray-900">
        <div class="max-w-6xl mx-auto">
            <h2 class="text-4xl font-bold text-center mb-8 animate-fadeIn">
                The Strongest Battlegrounds — МОЯ АРЕНА! 💪
            </h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div class="animate-fadeIn delay-200">
                    <img src="https://via.placeholder.com/500x300.png?text=The+Strongest+Battlegrounds" alt="The Strongest Battlegrounds" class="w-full rounded-lg hover-scale">
                </div>
                <div class="text-lg animate-fadeIn delay-400">
                    <p>
                        <strong>The Strongest Battlegrounds</strong> — это не просто игра, это место, где я, Ananas_Vitalya, показываю ВСЕМ, кто тут босс! 😎 Сделали её крутые ребята из <em>Yielding Arts</em>, и она тупо порвала Roblox: 12.6 миллиардов посещений на май 2025, плюс награда за <em>Лучший файтинг</em> на Roblox Innovation Awards 2024. Вдохновлена <em>One-Punch Man</em>, и это чистый кайф!
                    </p>
                    <p class="mt-4">
                        В игре куча персов, у каждого свои фишки, и я их всех размотал! Заряжаешь ультимейты, делаешь комбо, и противники падают, как мухи. Maturity: Mild, так что даже мелкие могут зайти, но реально побеждают только имбы вроде меня. 😏 Хочешь зайти? Ок, но не ной, когда я тебя урою в первом же бою!
                    </p>
                    <p class="mt-4">
                        Тут всё просто: или ты со мной, или ты в нокауте. Я уже знаю каждый угол карты, каждую атаку, и мои противники просто не успевают понять, что их разнесло. Эта игра — мой трон, и я на нём сижу с короной! Если думаешь, что можешь тягаться с королём, то давай, попробуй, но я предупреждал! 😆
                    </p>
                    <a href="https://www.roblox.com/games/10449761463/The-Strongest-Battlegrounds" target="_blank" class="mt-6 inline-block bg-red-600 text-white px-6 py-3 rounded-lg hover:bg-red-700 hover-scale">
                        Залетай в Мою Арену
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Call to Action -->
    <section class="bg-gradient-to-r from-blue-600 to-red-600 py-16 text-center">
        <h2 class="text-4xl font-bold mb-4 animate-fadeIn">
            КТО СМЕЛЫЙ ПРОТИВ КОРОЛЯ?! 😈
        </h2>
        <p class="text-xl mb-8 animate-fadeIn delay-200">
            Ananas_Vitalya (4476830117) — это имя, которое боятся все в <em>The Strongest Battlegrounds</em>! Залетай в Roblox, ищи меня и готовься к разносу! 😎 Нубы, не трындите, а пробуйте, но я вас уже предупредил: Я — ИМБА!
        </p>
        <div class="flex justify-center space-x-4">
            <a href="https://www.roblox.com/games/10449761463/The-Strongest-Battlegrounds" target="_blank" class="bg-white text-blue-600 px-8 py-4 rounded-lg font-bold hover:bg-gray-200 hover-scale animate-fadeIn delay-400">
                Играть Щас
            </a>
            <a href="https://www.roblox.com/users/4476830117/profile" target="_blank" class="bg-white text-blue-600 px-8 py-4 rounded-lg font-bold hover:bg-gray-200 hover-scale animate-fadeIn delay-400">
                Найти Ananas_Vitalya
            </a>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 py-8 text-center">
        <p class="text-lg animate-fadeIn">
            Сделано для БОГА Ananas_Vitalya (4476830117) | Powered by <a href="https://www.roblox.com" target="_blank" class="text-blue-400 hover:underline">Roblox</a> & <a href="https://yieldingarts.com" target="_blank" class="text-blue-400 hover:underline">Yielding Arts</a>
        </p>
        <p class="mt-2 text-sm">
            The Strongest Battlegrounds - Maturity: Mild | Verified Badge Icon
        </p>
    </footer>
</body>
</html>
