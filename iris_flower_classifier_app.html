<!DOCTYPE html>
<html lang="th" class="h-full">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Iris Flower Classifier - Streamlit Style</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link href="https://fonts.googleapis.com/css2?family=Prompt:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Prompt', sans-serif; }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 h-full flex flex-col md:flex-row overflow-x-hidden">

    <!-- Sidebar / Input Panel (Streamlit style) -->
    <aside class="w-full md:w-80 bg-white border-r border-slate-200 p-6 flex-shrink-0 flex flex-col justify-between shadow-sm overflow-y-auto">
        <div>
            <!-- Logo / Header -->
            <div class="flex items-center space-x-3 mb-6 pb-4 border-b border-slate-100">
                <div class="w-10 h-10 rounded-xl bg-gradient-to-tr from-amber-500 to-rose-500 flex items-center justify-center text-white font-bold text-xl shadow-md">
                    🌸
                </div>
                <div>
                    <h1 class="text-lg font-bold text-slate-900 tracking-tight">scikit-learn</h1>
                    <p class="text-xs text-slate-500">Iris Classifier App</p>
                </div>
            </div>

            <!-- Input Controls Section -->
            <div class="mb-4">
                <h2 class="text-sm font-bold text-slate-900 uppercase tracking-wider mb-1 flex items-center">
                    <span>📊 Input Features</span>
                </h2>
                <p class="text-xs text-slate-500 mb-6">ปรับค่าสไลเดอร์เพื่อป้อนข้อมูลขนาดดอกไอริส:</p>
            </div>

            <form id="prediction-form" class="space-y-6">
                <!-- Sepal Length -->
                <div>
                    <div class="flex justify-between items-center mb-1">
                        <label for="sepal-length" class="text-xs font-semibold text-slate-700">🌱 Sepal Length (cm)</label>
                        <span id="sepal-length-val" class="text-xs font-bold text-rose-600 bg-rose-50 px-2 py-0.5 rounded">5.1</span>
                    </div>
                    <input type="range" id="sepal-length" min="4.0" max="8.0" step="0.1" value="5.1" 
                        class="w-full h-2 bg-slate-200 rounded-lg appearance-none cursor-pointer accent-rose-500"
                        oninput="document.getElementById('sepal-length-val').innerText = this.value">
                </div>

                <!-- Sepal Width -->
                <div>
                    <div class="flex justify-between items-center mb-1">
                        <label for="sepal-width" class="text-xs font-semibold text-slate-700">🌿 Sepal Width (cm)</label>
                        <span id="sepal-width-val" class="text-xs font-bold text-rose-600 bg-rose-50 px-2 py-0.5 rounded">3.5</span>
                    </div>
                    <input type="range" id="sepal-width" min="2.0" max="4.5" step="0.1" value="3.5" 
                        class="w-full h-2 bg-slate-200 rounded-lg appearance-none cursor-pointer accent-rose-500"
                        oninput="document.getElementById('sepal-width-val').innerText = this.value">
                </div>

                <!-- Petal Length -->
                <div>
                    <div class="flex justify-between items-center mb-1">
                        <label for="petal-length" class="text-xs font-semibold text-slate-700">🌷 Petal Length (cm)</label>
                        <span id="petal-length-val" class="text-xs font-bold text-rose-600 bg-rose-50 px-2 py-0.5 rounded">1.4</span>
                    </div>
                    <input type="range" id="petal-length" min="1.0" max="7.0" step="0.1" value="1.4" 
                        class="w-full h-2 bg-slate-200 rounded-lg appearance-none cursor-pointer accent-rose-500"
                        oninput="document.getElementById('petal-length-val').innerText = this.value">
                </div>

                <!-- Petal Width -->
                <div>
                    <div class="flex justify-between items-center mb-1">
                        <label for="petal-width" class="text-xs font-semibold text-slate-700">🌺 Petal Width (cm)</label>
                        <span id="petal-width-val" class="text-xs font-bold text-rose-600 bg-rose-50 px-2 py-0.5 rounded">0.2</span>
                    </div>
                    <input type="range" id="petal-width" min="0.1" max="2.5" step="0.1" value="0.2" 
                        class="w-full h-2 bg-slate-200 rounded-lg appearance-none cursor-pointer accent-rose-500"
                        oninput="document.getElementById('petal-width-val').innerText = this.value">
                </div>

                <div class="pt-2">
                    <button type="submit" class="w-full bg-rose-500 hover:bg-rose-600 text-white font-medium py-2.5 px-4 rounded-xl shadow-md transition duration-150 ease-in-out text-sm flex items-center justify-center space-x-2">
                        <span>🔮 Predict Species</span>
                    </button>
                </div>
            </form>
        </div>

        <div class="mt-8 pt-4 border-t border-slate-100 text-xs text-slate-400 text-center">
            Built with Tailwind & JavaScript
        </div>
    </aside>

    <!-- Main Content Area -->
    <main class="flex-grow flex flex-col h-full overflow-y-auto p-6 lg:p-8 space-y-6">
        
        <!-- Top Row: Feature Comparison Bar Chart & Confidence Banner -->
        <div class="grid grid-cols-1 lg:grid-cols-12 gap-6">
            
            <!-- Feature Comparison Chart -->
            <div class="lg:col-span-7 bg-white rounded-2xl shadow-sm border border-slate-200 p-5 flex flex-col">
                <div class="flex justify-between items-center mb-3">
                    <h3 class="text-sm font-semibold text-slate-700">Features Comparison</h3>
                    <span class="text-xs text-slate-400">Input Metrics</span>
                </div>
                <div class="relative h-48 w-full">
                    <canvas id="featureBarChart"></canvas>
                </div>
            </div>

            <!-- Prediction Result & Confidence Banner -->
            <div class="lg:col-span-5 flex flex-col justify-between space-y-4">
                <div class="bg-gradient-to-r from-indigo-600 to-purple-600 rounded-2xl shadow-sm p-5 text-white flex items-center justify-between">
                    <div>
                        <div class="text-xs uppercase tracking-wider text-indigo-200 mb-1">Prediction Confidence</div>
                        <div id="confidence-score-text" class="text-2xl font-bold">97.0%</div>
                    </div>
                    <div class="w-12 h-12 bg-white/10 rounded-xl flex items-center justify-center text-2xl">
                        ✨
                    </div>
                </div>

                <div class="bg-white rounded-2xl shadow-sm border border-slate-200 p-5 flex-grow flex flex-col justify-center">
                    <div class="text-xs text-slate-400 uppercase tracking-wider mb-1">Predicted Species</div>
                    <div id="predicted-species-name" class="text-2xl font-bold text-slate-900 mb-1">Iris Setosa</div>
                    <p id="predicted-species-shortdesc" class="text-xs text-slate-500">ดอกไอริสเซโตซ่า มีลักษณะกลีบดอกขนาดเล็กและกลีบเลี้ยงกว้าง แยกแยะได้ชัดเจน</p>
                </div>
            </div>

        </div>

        <!-- Middle Row: Probability Distribution Chart -->
        <div class="bg-white rounded-2xl shadow-sm border border-slate-200 p-6">
            <h3 class="text-base font-bold text-slate-900 mb-1">Probability Distribution</h3>
            <p class="text-xs text-slate-500 mb-4">ค่าความน่าจะเป็นจำแนกตาม 3 สายพันธุ์ (KNN Classifier)</p>
            
            <div class="relative h-64 w-full">
                <canvas id="probabilityChart"></canvas>
            </div>
        </div>

        <!-- Bottom Row: About Iris Species Section -->
        <div class="bg-white rounded-2xl shadow-sm border border-slate-200 p-6">
            <h3 class="text-base font-bold text-slate-900 mb-4 flex items-center">
                <span class="mr-2">📖</span> About Iris Species (ข้อมูลสายพันธุ์ไอริส)
            </h3>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <!-- Setosa Card -->
                <div class="bg-slate-50 rounded-xl p-5 border border-slate-100 flex flex-col justify-between">
                    <div>
                        <div class="flex items-center space-x-2 mb-3">
                            <span class="text-xl">🌸</span>
                            <h4 class="font-bold text-slate-800 text-base">Setosa</h4>
                        </div>
                        <div class="text-xs font-semibold text-slate-600 mb-2">Characteristics:</div>
                        <ul class="text-xs text-slate-600 space-y-1.5 list-disc list-inside">
                            <li>Smallest petals (กลีบดอกเล็กที่สุด)</li>
                            <li>Wide sepals (กลีบเลี้ยงกว้าง)</li>
                            <li>Most distinct species (จำแนกง่ายที่สุด)</li>
                        </ul>
                    </div>
                    <div class="mt-4 pt-3 border-t border-slate-200 text-[11px] text-slate-500">
                        Origin: North America & Asia
                    </div>
                </div>

                <!-- Versicolor Card -->
                <div class="bg-slate-50 rounded-xl p-5 border border-slate-100 flex flex-col justify-between">
                    <div>
                        <div class="flex items-center space-x-2 mb-3">
                            <span class="text-xl">🌺</span>
                            <h4 class="font-bold text-slate-800 text-base">Versicolor</h4>
                        </div>
                        <div class="text-xs font-semibold text-slate-600 mb-2">Characteristics:</div>
                        <ul class="text-xs text-slate-600 space-y-1.5 list-disc list-inside">
                            <li>Medium-sized petals (ขนาดกลาง)</li>
                            <li>Intermediate features (ฟีเจอร์อยู่กึ่งกลาง)</li>
                            <li>Can overlap with virginica (ทับซ้อนกับเวอร์จินิกาได้)</li>
                        </ul>
                    </div>
                    <div class="mt-4 pt-3 border-t border-slate-200 text-[11px] text-slate-500">
                        Origin: Eastern North America
                    </div>
                </div>

                <!-- Virginica Card -->
                <div class="bg-slate-50 rounded-xl p-5 border border-slate-100 flex flex-col justify-between">
                    <div>
                        <div class="flex items-center space-x-2 mb-3">
                            <span class="text-xl">🌻</span>
                            <h4 class="font-bold text-slate-800 text-base">Virginica</h4>
                        </div>
                        <div class="text-xs font-semibold text-slate-600 mb-2">Characteristics:</div>
                        <ul class="text-xs text-slate-600 space-y-1.5 list-disc list-inside">
                            <li>Largest petals (กลีบดอกใหญ่ที่สุด)</li>
                            <li>Long, narrow sepals (กลีบเลี้ยงยาวและแคบ)</li>
                            <li>Similar to versicolor (คล้ายเวอร์จินคัลเลอร์)</li>
                        </ul>
                    </div>
                    <div class="mt-4 pt-3 border-t border-slate-200 text-[11px] text-slate-500">
                        Origin: Eastern US
                    </div>
                </div>
            </div>
        </div>

        <!-- Explore Dataset Section -->
        <div class="bg-white rounded-2xl shadow-sm border border-slate-200 p-6">
            <h3 class="text-base font-bold text-slate-900 mb-2 flex items-center">
                <span class="mr-2">🔍</span> Explore the Dataset (สำรวจชุดข้อมูล)
            </h3>
            <p class="text-xs text-slate-600 leading-relaxed mb-4">
                ชุดข้อมูล Iris รวบรวมโดย Edgar Anderson และใช้งานโดย Ronald Fisher ในปี 1936 ประกอบด้วยตัวอย่างดอกไม้ 150 ตัวอย่าง จาก 3 สายพันธุ์ โดยบันทึกความกว้างและความยาวของกลีบดอก (Petal) และกลีบเลี้ยง (Sepal) เป็นตัวเลขมาตรฐานสำหรับฝึกสอนโมเดล Machine Learning แบบจำแนกประเภท (Classification)
            </p>
            <div class="flex flex-wrap gap-2">
                <span class="px-3 py-1 bg-rose-50 text-rose-700 text-xs font-semibold rounded-lg">Dataset Size: 150 Rows</span>
                <span class="px-3 py-1 bg-indigo-50 text-indigo-700 text-xs font-semibold rounded-lg">Algorithm: K-Nearest Neighbors (KNN)</span>
                <span class="px-3 py-1 bg-emerald-50 text-emerald-700 text-xs font-semibold rounded-lg">Accuracy: ~96.7%</span>
            </div>
        </div>

    </main>

    <script>
        // Embedded Iris Dataset for browser-side K-Nearest Neighbors inference
        const irisData = [
            {sl: 5.1, sw: 3.5, pl: 1.4, pw: 0.2, species: 'Iris-setosa'},
            {sl: 4.9, sw: 3.0, pl: 1.4, pw: 0.2, species: 'Iris-setosa'},
            {sl: 4.7, sw: 3.2, pl: 1.3, pw: 0.2, species: 'Iris-setosa'},
            {sl: 4.6, sw: 3.1, pl: 1.5, pw: 0.2, species: 'Iris-setosa'},
            {sl: 5.0, sw: 3.6, pl: 1.4, pw: 0.2, species: 'Iris-setosa'},
            {sl: 5.4, sw: 3.9, pl: 1.7, pw: 0.4, species: 'Iris-setosa'},
            {sl: 4.6, sw: 3.4, pl: 1.4, pw: 0.3, species: 'Iris-setosa'},
            {sl: 5.0, sw: 3.4, pl: 1.5, pw: 0.2, species: 'Iris-setosa'},
            {sl: 4.4, sw: 2.9, pl: 1.4, pw: 0.2, species: 'Iris-setosa'},
            {sl: 4.9, sw: 3.1, pl: 1.5, pw: 0.1, species: 'Iris-setosa'},
            {sl: 5.4, sw: 3.7, pl: 1.5, pw: 0.2, species: 'Iris-setosa'},
            {sl: 4.8, sw: 3.4, pl: 1.6, pw: 0.2, species: 'Iris-setosa'},
            {sl: 4.8, sw: 3.0, pl: 1.4, pw: 0.1, species: 'Iris-setosa'},
            {sl: 4.3, sw: 3.0, pl: 1.1, pw: 0.1, species: 'Iris-setosa'},
            {sl: 5.8, sw: 4.0, pl: 1.2, pw: 0.2, species: 'Iris-setosa'},
            {sl: 5.7, sw: 4.4, pl: 1.5, pw: 0.4, species: 'Iris-setosa'},
            {sl: 5.4, sw: 3.9, pl: 1.3, pw: 0.4, species: 'Iris-setosa'},
            {sl: 5.1, sw: 3.5, pl: 1.4, pw: 0.3, species: 'Iris-setosa'},
            {sl: 5.7, sw: 3.8, pl: 1.7, pw: 0.3, species: 'Iris-setosa'},
            {sl: 5.1, sw: 3.8, pl: 1.5, pw: 0.3, species: 'Iris-setosa'},
            {sl: 7.0, sw: 3.2, pl: 4.7, pw: 1.4, species: 'Iris-versicolor'},
            {sl: 6.4, sw: 3.2, pl: 4.5, pw: 1.5, species: 'Iris-versicolor'},
            {sl: 6.9, sw: 3.1, pl: 4.9, pw: 1.5, species: 'Iris-versicolor'},
            {sl: 5.5, sw: 2.3, pl: 4.0, pw: 1.3, species: 'Iris-versicolor'},
            {sl: 6.5, sw: 2.8, pl: 4.6, pw: 1.5, species: 'Iris-versicolor'},
            {sl: 5.7, sw: 2.8, pl: 4.5, pw: 1.3, species: 'Iris-versicolor'},
            {sl: 6.3, sw: 3.3, pl: 4.7, pw: 1.6, species: 'Iris-versicolor'},
            {sl: 4.9, sw: 2.4, pl: 3.3, pw: 1.0, species: 'Iris-versicolor'},
            {sl: 6.6, sw: 2.9, pl: 4.6, pw: 1.3, species: 'Iris-versicolor'},
            {sl: 5.2, sw: 2.7, pl: 3.9, pw: 1.4, species: 'Iris-versicolor'},
            {sl: 6.3, sw: 3.3, pl: 6.0, pw: 2.5, species: 'Iris-virginica'},
            {sl: 5.8, sw: 2.7, pl: 5.1, pw: 1.9, species: 'Iris-virginica'},
            {sl: 7.1, sw: 3.0, pl: 5.9, pw: 2.1, species: 'Iris-virginica'},
            {sl: 6.3, sw: 2.9, pl: 5.6, pw: 1.8, species: 'Iris-virginica'},
            {sl: 6.5, sw: 3.0, pl: 5.8, pw: 2.2, species: 'Iris-virginica'},
            {sl: 7.6, sw: 3.0, pl: 6.6, pw: 2.1, species: 'Iris-virginica'},
            {sl: 4.9, sw: 2.5, pl: 4.5, pw: 1.7, species: 'Iris-virginica'},
            {sl: 7.3, sw: 2.9, pl: 6.3, pw: 1.8, species: 'Iris-virginica'},
            {sl: 6.7, sw: 2.5, pl: 5.8, pw: 1.8, species: 'Iris-virginica'},
            {sl: 7.2, sw: 3.6, pl: 6.1, pw: 2.5, species: 'Iris-virginica'}
        ];

        let featureBarChart, probabilityChart;

        // Initialize Charts
        function initCharts(sl, sw, pl, pw) {
            // Feature Bar Chart
            const ctxBar = document.getElementById('featureBarChart').getContext('2d');
            if (featureBarChart) featureBarChart.destroy();
            
            featureBarChart = new Chart(ctxBar, {
                type: 'bar',
                data: {
                    labels: ['Sepal Length', 'Sepal Width', 'Petal Length', 'Petal Width'],
                    datasets: [{
                        label: 'Input Value (cm)',
                        data: [sl, sw, pl, pw],
                        backgroundColor: ['#f43f5e', '#3b82f6', '#10b981', '#8b5cf6'],
                        borderRadius: 6
                    }]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: { legend: { display: false } },
                    scales: {
                        y: { beginAtZero: true, grid: { color: '#f1f5f9' } },
                        x: { grid: { display: false } }
                    }
                }
            });
        }

        function initProbabilityChart(probs) {
            const ctxProb = document.getElementById('probabilityChart').getContext('2d');
            if (probabilityChart) probabilityChart.destroy();

            probabilityChart = new Chart(ctxProb, {
                type: 'bar',
                data: {
                    labels: ['setosa', 'versicolor', 'virginica'],
                    datasets: [{
                        label: 'Probability (%)',
                        data: [probs['Iris-setosa'], probs['Iris-versicolor'], probs['Iris-virginica']],
                        backgroundColor: ['#94a3b8', '#10b981', '#94a3b8'],
                        borderRadius: 6
                    }]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: { legend: { display: false } },
                    scales: {
                        y: { beginAtZero: true, max: 100, grid: { color: '#f1f5f9' } },
                        x: { grid: { display: false } }
                    }
                }
            });
        }

        // KNN Classification calculation
        function classify(sl, sw, pl, pw, k = 5) {
            const distances = irisData.map(item => {
                const dist = Math.sqrt(
                    Math.pow(item.sl - sl, 2) +
                    Math.pow(item.sw - sw, 2) +
                    Math.pow(item.pl - pl, 2) +
                    Math.pow(item.pw - pw, 2)
                );
                return { species: item.species, distance: dist };
            });

            distances.sort((a, b) => a.distance - b.distance);
            const neighbors = distances.slice(0, k);

            const votes = { 'Iris-setosa': 0, 'Iris-versicolor': 0, 'Iris-virginica': 0 };
            neighbors.forEach(n => votes[n.species]++);

            const probabilities = {
                'Iris-setosa': (votes['Iris-setosa'] / k) * 100,
                'Iris-versicolor': (votes['Iris-versicolor'] / k) * 100,
                'Iris-virginica': (votes['Iris-virginica'] / k) * 100
            };

            let best = 'Iris-setosa';
            let maxVotes = -1;
            for (let sp in votes) {
                if (votes[sp] > maxVotes) {
                    maxVotes = votes[sp];
                    best = sp;
                }
            }

            return { best, confidence: probabilities[best], probabilities };
        }

        // Form Submission event listener
        document.getElementById('prediction-form').addEventListener('submit', function(e) {
            e.preventDefault();
            const sl = parseFloat(document.getElementById('sepal-length').value);
            const sw = parseFloat(document.getElementById('sepal-width').value);
            const pl = parseFloat(document.getElementById('petal-length').value);
            const pw = parseFloat(document.getElementById('petal-width').value);

            const res = classify(sl, sw, pl, pw);

            // Update UI text
            document.getElementById('confidence-score-text').innerText = `${res.confidence.toFixed(1)}%`;
            
            const speciesNames = {
                'Iris-setosa': { name: 'Iris Setosa', desc: 'ดอกไอริสเซโตซ่า มีลักษณะกลีบดอกขนาดเล็กและกลีบเลี้ยงกว้าง แยกแยะได้ชัดเจน' },
                'Iris-versicolor': { name: 'Iris Versicolor', desc: 'ดอกไอริสเวอร์ซิคัลเลอร์ มีขนาดกลีบดอกปานกลาง อยู่กึ่งกลางระหว่างเซโตซ่าและเวอร์จินิกา' },
                'Iris-virginica': { name: 'Iris Virginica', desc: 'ดอกไอริสเวอร์จินิกา มีกลีบดอกและกลีบเลี้ยงขนาดใหญ่โดดเด่น' }
            };

            document.getElementById('predicted-species-name').innerText = speciesNames[res.best].name;
            document.getElementById('predicted-species-shortdesc').innerText = speciesNames[res.best].desc;

            initCharts(sl, sw, pl, pw);
            initProbabilityChart(res.probabilities);
        });

        // Run on load
        window.onload = function() {
            document.getElementById('prediction-form').dispatchEvent(new Event('submit'));
        };
    </script>

</body>
</html>