<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Liên Quân Pro Academy 2026</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Oswald:wght@500;700&family=Roboto:wght@400;700&display=swap');
        body { background-color: #020617; color: #f1f5f9; font-family: 'Roboto', sans-serif; }
        h1, h2, h3 { font-family: 'Oswald', sans-serif; }
        .bg-gold-gradient { background: linear-gradient(135deg, #fbbf24, #d97706); }
        .card-custom { background: rgba(30, 41, 59, 0.6); border: 1px solid #1e293b; backdrop-filter: blur(12px); border-radius: 20px; transition: 0.3s; }
        .card-custom:hover { border-color: #fbbf24; transform: translateY(-3px); box-shadow: 0 10px 20px rgba(0,0,0,0.5); }
        .hidden { display: none; }
        .hero-img { width: 60px; height: 60px; border-radius: 50%; border: 2px solid #fbbf24; object-fit: cover; }
        .video-container { position: relative; padding-bottom: 56.25%; height: 0; border-radius: 15px; overflow: hidden; }
        .video-container iframe { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }
        .btn-option { background: #1e293b; padding: 12px; border-radius: 12px; width: 100%; text-align: left; border: 1px solid #334155; margin-bottom: 8px; transition: 0.2s; }
        .btn-option:hover { background: #334155; border-color: #fbbf24; }
    </style>
</head>
<body class="p-4 md:p-10">

    <div id="app" class="max-w-2xl mx-auto">
        <header id="header" class="text-center py-6">
            <h1 class="text-5xl font-bold text-transparent bg-clip-text bg-gold-gradient italic uppercase tracking-tighter">LIÊN QUÂN ACADEMY</h1>
            <p class="text-slate-400 text-xs mt-2 tracking-widest">HỆ THỐNG GIÁO ÁN CHIẾN THUẬT TOÀN DIỆN</p>
        </header>

        <div id="screen-home" class="grid grid-cols-2 gap-4 mt-6">
            <div class="card-custom p-6 text-center cursor-pointer" onclick="goTo('screen-intro')">
                <i class="fas fa-info-circle text-2xl mb-2 text-blue-400"></i><br>Giới Thiệu
            </div>
            <div class="card-custom p-6 text-center cursor-pointer" onclick="goTo('screen-heroes')">
                <i class="fas fa-user-shield text-2xl mb-2 text-red-500"></i><br>Tướng & Đồ
            </div>
            <div class="card-custom p-6 text-center cursor-pointer" onclick="goTo('screen-map')">
                <i class="fas fa-map-marked-alt text-2xl mb-2 text-green-400"></i><br>Bản Đồ
            </div>
            <div class="card-custom p-6 text-center cursor-pointer" onclick="goTo('screen-counter')">
                <i class="fas fa-fist-raised text-2xl mb-2 text-pink-500"></i><br>Khắc Chế
            </div>
            <div class="card-custom p-6 text-center cursor-pointer" onclick="goTo('screen-zata')">
                <i class="fas fa-wind text-2xl mb-2 text-yellow-400"></i><br>Học Zata
            </div>
            <div class="card-custom p-6 text-center cursor-pointer" onclick="goTo('screen-quiz')">
                <i class="fas fa-graduation-cap text-2xl mb-2 text-orange-400"></i><br>Trắc Nghiệm
            </div>
        </div>

        <div id="screen-intro" class="hidden">
            <button onclick="goTo('screen-home')" class="mb-4 text-blue-400 font-bold">← QUAY LẠI</button>
            <div class="card-custom p-6">
                <h2 class="text-2xl font-bold text-yellow-500 mb-4 italic">NHẬP MÔN LIÊN QUÂN</h2>
                <div class="space-y-3 text-sm text-slate-300">
                    <p><b>- Liên Quân Mobile:</b> Game MOBA 5v5 trên di động hàng đầu.</p>
                    <p><b>- Nhiệm vụ:</b> Phối hợp 5 người, phá trụ, ăn mục tiêu lớn để dứt điểm Nhà Chính.</p>
                    <p><b>- Thời gian:</b> 12 - 20 phút mỗi trận.</p>
                </div>
            </div>
        </div>

        <div id="screen-heroes" class="hidden">
            <button onclick="goTo('screen-home')" class="mb-4 text-blue-400 font-bold">← QUAY LẠI</button>
            <h2 class="text-2xl font-bold text-yellow-500 mb-6 italic text-center">TƯỚNG & TRANG BỊ META</h2>
            
            <div class="space-y-6">
                <div class="card-custom p-4 border-l-4 border-yellow-500">
                    <div class="flex items-center mb-4">
                        <img src="https://img.triethoc.edu.vn/uploads/2024/02/valhein-lien-quan-mobile.jpg" class="hero-img mr-4">
                        <div><h3 class="font-bold text-lg text-yellow-500">Valhein (Xạ Thủ/Phép)</h3><p class="text-[10px] text-gray-400">Ưu tiên: Tốc đánh & Xuyên phép</p></div>
                    </div>
                    <div class="text-[12px] space-y-1">
                        <p>⚔️ <b>Đồ tốt nhất:</b> Giày thuật sĩ, Thập tự kiếm, Vương miện Hecate, Trượng bùng nổ, Quyền trượng Rhea, Sách thánh.</p>
                        <p>💎 <b>Ngọc:</b> Đỏ Công phép, Tím Tốc đánh/chạy, Xanh Xuyên phép.</p>
                    </div>
                </div>
                <div class="card-custom p-4 border-l-4 border-blue-500">
                    <div class="flex items-center mb-4">
                        <img src="https://img.triethoc.edu.vn/uploads/2024/02/krixi-lien-quan-mobile.jpg" class="hero-img mr-4">
                        <div><h3 class="font-bold text-lg text-blue-400">Krixi (Pháp Sư)</h3><p class="text-[10px] text-gray-400">Ưu tiên: Công phép & Hồi chiêu</p></div>
                    </div>
                    <div class="text-[12px] space-y-1">
                        <p>⚔️ <b>Đồ tốt nhất:</b> Giày phù thủy, Trượng bùng nổ, Xuyên tâm lệnh, Vương miện, Sách thánh, Quả cầu băng sương.</p>
                        <p>💎 <b>Ngọc:</b> Đỏ Công phép, Tím Hút máu phép, Xanh Giảm hồi chiêu.</p>
                    </div>
                </div>
                <div class="card-custom p-4 border-l-4 border-green-500">
                    <div class="flex items-center mb-4">
                        <img src="https://img.triethoc.edu.vn/uploads/2024/02/thane-lien-quan-mobile.jpg" class="hero-img mr-4">
                        <div><h3 class="font-bold text-lg text-green-400">Thane (Hỗ Trợ)</h3><p class="text-[10px] text-gray-400">Ưu tiên: Máu & Kháng hiệu ứng</p></div>
                    </div>
                    <div class="text-[12px] space-y-1">
                        <p>🛡️ <b>Đồ tốt nhất:</b> Phụ trợ mở trói, Giày kiên cường, Giáp Gaia, Khiên huyền thoại, Sách truy hồn, Giáp hộ mệnh.</p>
                        <p>💎 <b>Ngọc:</b> Kim thân, Bảo vệ, Giảm hồi chiêu.</p>
                    </div>
                </div>
            </div>
        </div>

        <div id="screen-map" class="hidden">
            <button onclick="goTo('screen-home')" class="mb-4 text-blue-400 font-bold">← QUAY LẠI</button>
            <div class="card-custom p-4">
                <h2 class="text-2xl font-bold text-green-400 mb-4">CHIẾN THUẬT DI CHUYỂN</h2>
                <img src="https://cdn.tgdd.vn/Files/2020/09/16/1289945/ban-do-moi-va-nhung-thay-doi-moi-tai-lien-quan-mobile-mua-16-1.jpg" class="w-full rounded-xl mb-4 shadow-lg border border-slate-700">
                <div class="space-y-2 text-sm">
                    <p>🔥 <b>Rừng:</b> Kiểm soát Rồng (tăng vàng) và Tà Thần (tăng sức mạnh đẩy đường).</p>
                    <p>🔥 <b>Đảo đường:</b> Sau khi dọn lính xong, hãy di chuyển hỗ trợ đồng đội ở các đường khác.</p>
                </div>
            </div>
        </div>

        <div id="screen-counter" class="hidden">
            <button onclick="goTo('screen-home')" class="mb-4 text-blue-400 font-bold">← QUAY LẠI</button>
            <div class="space-y-4">
                <div class="card-custom p-5 border-l-4 border-red-500">
                    <h3 class="font-bold text-red-500 mb-3 italic underline">CÁCH PICK TƯỚNG KHẮC CHẾ</h3>
                    <ul class="text-xs space-y-2 text-slate-300 italic">
                        <li>- Gặp <b>Nakroth, Zata</b> (Cơ động): Chọn <b>Arum, Aleister</b>.</li>
                        <li>- Gặp <b>Taara, Veres</b> (Hồi máu): Chọn <b>Hayate</b> (Sát thương chuẩn).</li>
                    </ul>
                </div>
                <div class="card-custom p-5 border-l-4 border-blue-500">
                    <h3 class="font-bold text-blue-400 mb-3 italic underline">CÁCH LÊN ĐỒ KHẮC CHẾ</h3>
                    <ul class="text-xs space-y-2 text-slate-300">
                        <li>- Địch quá trâu: Lên <b>Kiếm Fafnir</b> hoặc <b>Kiếm Muramasa</b>.</li>
                        <li>- Địch hồi máu nhanh: Lên <b>Sách/Đao Truy Hồn</b>.</li>
                        <li>- Địch dồn dame nhanh: Lên <b>Quả Cầu Băng Sương</b>.</li>
                    </ul>
                </div>
            </div>
        </div>

        <div id="screen-zata" class="hidden">
            <button onclick="goTo('screen-home')" class="mb-4 text-blue-400 font-bold">← QUAY LẠI</button>
            <h2 class="text-2xl font-bold text-yellow-500 mb-4 italic">BÍ KÍP BAY ZATA</h2>
            <div class="video-container shadow-2xl">
                <iframe src="https://www.youtube.com/embed/KsNLuWezUfw" frameborder="0" allowfullscreen></iframe>
            </div>
            <div class="card-custom p-4 mt-6">
                <p class="text-sm font-bold text-yellow-400 uppercase italic">Combo 5 Stack:</p>
                <p class="text-[12px] text-slate-400 mt-2">Dùng Chiêu 2 -> Chiêu 1 -> Ulti và lướt đúng vào luồng gió. Luôn xen kẽ đánh thường để tối ưu hóa nội tại.</p>
            </div>
        </div>

        <div id="screen-quiz" class="hidden">
            <button onclick="goTo('screen-home')" class="mb-4 text-blue-400 font-bold">← QUAY LẠI</button>
            <div class="card-custom p-8 text-center">
                <div id="quiz-area">
                    <p class="text-xs text-yellow-500 font-bold uppercase mb-2" id="q-number">CÂU HỎI 1</p>
                    <h3 class="text-xl font-bold mb-8 min-h-[60px]" id="q-text">Đang tải...</h3>
                    <div id="q-options"></div>
                </div>
                <div id="quiz-result" class="hidden mt-6 p-4 rounded-xl font-bold"></div>
                <button id="next-btn" class="hidden mt-6 bg-gold-gradient px-8 py-2 rounded-full font-bold text-white shadow-lg transition hover:scale-105" onclick="nextQuestion()">CÂU TIẾP THEO</button>
            </div>
        </div>
    </div>

    <script>
        const quizData = [
            { q: "Món đồ nào giúp khắc chế các tướng có khả năng hồi máu mạnh?", o: ["Vương miện Hecate", "Sách Truy Hồn", "Kiếm Fafnir"], c: 1 },
            { q: "Vị trí nào thường đi cùng Xạ thủ để bảo vệ và lấy tầm nhìn?", o: ["Pháp sư", "Đấu sĩ", "Trợ thủ"], c: 2 },
            { q: "Phép bổ trợ nào giúp di chuyển xuyên tường ngay lập tức?", o: ["Tốc biến", "Tốc hành", "Bộc phá"], c: 0 },
            { q: "Khi Zata bay lên trời (Ulti), trạng thái của hắn là gì?", o: ["Bị làm chậm", "Bất tử (Không thể bị chọn)", "Bị choáng"], c: 1 }
        ];

        let currentIdx = 0;

        function goTo(id) {
            const screens = ['screen-home', 'screen-intro', 'screen-heroes', 'screen-map', 'screen-counter', 'screen-zata', 'screen-quiz'];
            screens.forEach(s => document.getElementById(s).classList.add('hidden'));
            document.getElementById(id).classList.remove('hidden');
            if(id === 'screen-quiz') resetQuiz();
        }

        function resetQuiz() {
            currentIdx = 0;
            showQuestion();
        }

        function showQuestion() {
            if(currentIdx >= quizData.length) {
                document.getElementById('quiz-area').innerHTML = "<i class='fas fa-trophy text-6xl text-yellow-500 mb-4'></i><h2 class='text-2xl font-bold'>XUẤT SẮC!<br>BẠN ĐÃ TỐT NGHIỆP!</h2>";
                document.getElementById('next-btn').classList.add('hidden');
                return;
            }
            const data = quizData[currentIdx];
            document.getElementById('q-number').innerText = `CÂU HỎI ${currentIdx + 1} / ${quizData.length}`;
            document.getElementById('q-text').innerText = data.q;
            const options = document.getElementById('q-options');
            options.innerHTML = '';
            data.o.forEach((opt, i) => {
                const btn = document.createElement('button');
                btn.className = "btn-option";
                btn.innerText = opt;
                btn.onclick = () => selectAns(i);
                options.appendChild(btn);
            });
            document.getElementById('quiz-result').classList.add('hidden');
            document.getElementById('next-btn').classList.add('hidden');
        }

        function selectAns(i) {
            const res = document.getElementById('quiz-result');
            res.classList.remove('hidden');
            if(i === quizData[currentIdx].c) {
                res.innerText = "CHÍNH XÁC! +1 ĐIỂM CHIẾN THUẬT.";
                res.className = "mt-6 p-4 rounded-xl bg-green-900/50 text-green-400 font-bold";
            } else {
                res.innerText = "SAI RỒI! HÃY NGHIÊN CỨU LẠI GIÁO ÁN.";
                res.className = "mt-6 p-4 rounded-xl bg-red-900/50 text-red-400 font-bold";
            }
            document.getElementById('next-btn').classList.remove('hidden');
        }

        function nextQuestion() {
            currentIdx++;
            showQuestion();
        }
    </script>
</body>
</html>
