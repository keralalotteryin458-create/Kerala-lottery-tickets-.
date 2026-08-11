<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kerala State Lottery - Mega Jackpot</title>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-dark: #0b0e14;
            --card-bg: #141820;
            --border-color: #232936;
            --accent-gold: #f59e0b;
            --accent-yellow: #fbbf24;
            --whatsapp-green: #25d366;
            --text-white: #ffffff;
            --text-gray: #94a3b8;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Plus Jakarta Sans', sans-serif;
        }

        body {
            background-color: var(--bg-dark);
            color: var(--text-white);
            padding-bottom: 90px;
        }

        /* HEADER */
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 20px;
            background-color: rgba(11, 14, 20, 0.95);
            border-bottom: 1px solid var(--border-color);
            position: sticky;
            top: 0;
            z-index: 100;
            backdrop-filter: blur(8px);
        }

        .logo-box {
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .logo-icon {
            background: linear-gradient(135deg, var(--accent-gold), var(--accent-yellow));
            color: #000;
            font-weight: 800;
            font-size: 20px;
            width: 42px;
            height: 42px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 0 15px rgba(245, 158, 11, 0.4);
        }

        .logo-text h2 {
            font-size: 16px;
            font-weight: 800;
            letter-spacing: 0.5px;
            line-height: 1.1;
        }

        .logo-text span {
            font-size: 11px;
            color: var(--accent-gold);
            letter-spacing: 1.5px;
            font-weight: 600;
        }

        .btn-header-wa {
            background-color: rgba(37, 211, 102, 0.15);
            color: var(--whatsapp-green);
            border: 1px solid var(--whatsapp-green);
            padding: 8px 14px;
            border-radius: 30px;
            font-size: 12px;
            font-weight: 700;
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 6px;
        }

        .container {
            max-width: 500px;
            margin: 0 auto;
            padding: 15px;
        }

        /* HERO JACKPOT CARD */
        .badge-live {
            background: rgba(245, 158, 11, 0.15);
            border: 1px solid var(--accent-gold);
            color: var(--accent-gold);
            font-size: 11px;
            font-weight: 700;
            padding: 4px 12px;
            border-radius: 20px;
            display: inline-block;
            margin: 15px auto 10px auto;
            text-align: center;
        }

        .hero-title {
            text-align: center;
            font-size: 28px;
            font-weight: 900;
            line-height: 1.1;
            margin-bottom: 5px;
            background: linear-gradient(180deg, #ffffff 0%, #cbd5e1 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .hero-title span {
            background: linear-gradient(180deg, var(--accent-yellow) 0%, var(--accent-gold) 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            display: block;
        }

        .hero-sub {
            text-align: center;
            font-size: 13px;
            color: var(--text-gray);
            margin-bottom: 20px;
        }

        .jackpot-circle {
            width: 240px;
            height: 240px;
            margin: 0 auto 25px auto;
            border-radius: 50%;
            border: 4px solid var(--accent-gold);
            box-shadow: 0 0 30px rgba(245, 158, 11, 0.25);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            background: radial-gradient(circle, rgba(245,158,11,0.1) 0%, rgba(20,24,32,1) 80%);
            position: relative;
        }

        .crown-icon {
            font-size: 28px;
            margin-bottom: 4px;
        }

        .jackpot-circle p {
            font-size: 11px;
            color: var(--accent-gold);
            font-weight: 700;
            letter-spacing: 1px;
        }

        .jackpot-circle h1 {
            font-size: 38px;
            font-weight: 900;
            color: #fff;
            line-height: 1;
            margin: 4px 0;
        }

        .stars {
            color: var(--accent-gold);
            font-size: 14px;
        }

        /* TIMER & PROGRESS */
        .timer-card {
            background: var(--card-bg);
            border: 1px solid var(--border-color);
            border-radius: 12px;
            padding: 15px;
            text-align: center;
            margin-bottom: 15px;
        }

        .timer-title {
            font-size: 12px;
            color: var(--accent-gold);
            font-weight: 700;
            margin-bottom: 10px;
            letter-spacing: 1px;
        }

        .timer-digits {
            display: flex;
            justify-content: center;
            gap: 15px;
            font-weight: 800;
        }

        .time-box span {
            display: block;
            font-size: 22px;
            color: #fff;
        }

        .time-box label {
            font-size: 9px;
            color: var(--text-gray);
        }

        .progress-box {
            background: var(--card-bg);
            border: 1px solid var(--border-color);
            border-radius: 12px;
            padding: 12px;
            margin-bottom: 20px;
        }

        .progress-text {
            font-size: 12px;
            color: #ef4444;
            font-weight: 700;
            margin-bottom: 8px;
            display: flex;
            align-items: center;
            gap: 6px;
        }

        .progress-bar {
            height: 8px;
            background: #232936;
            border-radius: 10px;
            overflow: hidden;
        }

        .progress-fill {
            width: 78%;
            height: 100%;
            background: linear-gradient(90deg, #f59e0b, #ef4444);
        }

        /* TICKET SELECTION GRID */
        .section-title {
            text-align: center;
            font-size: 20px;
            font-weight: 800;
            margin-top: 10px;
        }

        .section-sub {
            text-align: center;
            font-size: 12px;
            color: var(--text-gray);
            margin-bottom: 15px;
        }

        .custom-input-box {
            background: var(--card-bg);
            border: 1px solid var(--border-color);
            border-radius: 12px;
            padding: 12px;
            margin-bottom: 15px;
        }

        .custom-input-box label {
            font-size: 12px;
            font-weight: 700;
            color: var(--accent-gold);
            display: block;
            margin-bottom: 6px;
        }

        .custom-input-group {
            display: flex;
            gap: 8px;
        }

        .custom-input-group input {
            flex: 1;
            background: #0b0e14;
            border: 1px solid var(--border-color);
            border-radius: 8px;
            padding: 10px;
            color: #fff;
            font-weight: 700;
            font-size: 16px;
            letter-spacing: 2px;
            outline: none;
        }

        .custom-input-group button {
            background: var(--accent-gold);
            color: #000;
            border: none;
            padding: 0 15px;
            border-radius: 8px;
            font-weight: 700;
            cursor: pointer;
        }

        .ticket-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 12px;
            margin-bottom: 25px;
        }

        .ticket-card {
            background: var(--card-bg);
            border: 1px solid var(--border-color);
            border-radius: 10px;
            padding: 14px 10px;
            text-align: center;
            cursor: pointer;
            position: relative;
            transition: all 0.2s ease;
        }

        .ticket-card.selected {
            border-color: var(--accent-gold);
            background: rgba(245, 158, 11, 0.08);
        }

        .ticket-card.selected::after {
            content: "✓";
            position: absolute;
            top: -6px;
            right: -6px;
            background: var(--accent-gold);
            color: #000;
            width: 18px;
            height: 18px;
            border-radius: 50%;
            font-size: 11px;
            font-weight: 900;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .ticket-tag {
            font-size: 10px;
            color: var(--text-gray);
            letter-spacing: 1px;
            display: block;
            margin-bottom: 2px;
        }

        .ticket-number {
            font-size: 18px;
            font-weight: 800;
            color: #fff;
            letter-spacing: 1px;
        }

        /* BOTTOM STICKY BAR */
        .bottom-bar {
            position: fixed;
            bottom: 0; left: 0; right: 0;
            background: #141820;
            border-top: 1px solid var(--border-color);
            padding: 12px 20px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            z-index: 90;
        }

        .bottom-info p {
            font-size: 11px;
            color: var(--text-gray);
        }

        .bottom-info h3 {
            font-size: 18px;
            color: var(--accent-gold);
            font-weight: 800;
        }

        .btn-proceed {
            background: linear-gradient(135deg, #f59e0b, #d97706);
            color: #000;
            border: none;
            padding: 12px 22px;
            border-radius: 10px;
            font-weight: 800;
            font-size: 14px;
            cursor: pointer;
            box-shadow: 0 4px 15px rgba(245, 158, 11, 0.3);
        }

        /* MODAL */
        .modal {
            display: none;
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: rgba(0, 0, 0, 0.85);
            backdrop-filter: blur(5px);
            justify-content: center;
            align-items: center;
            z-index: 999;
            padding: 15px;
        }

        .modal-content {
            background: #141820;
            border: 1px solid var(--border-color);
            border-radius: 16px;
            width: 100%;
            max-width: 420px;
            padding: 22px;
            position: relative;
        }

        .close-btn {
            position: absolute;
            top: 15px; right: 15px;
            font-size: 20px;
            cursor: pointer;
            color: var(--text-gray);
        }

        .modal-title {
            font-size: 18px;
            font-weight: 800;
            color: var(--accent-gold);
            text-align: center;
            margin-bottom: 4px;
        }

        .upi-box {
            background: #0b0e14;
            border: 1px dashed var(--accent-gold);
            border-radius: 10px;
            padding: 10px;
            text-align: center;
            margin: 15px 0;
        }

        .upi-id {
            font-size: 14px;
            font-weight: 800;
            color: #fff;
            margin-top: 4px;
        }

        .qr-box {
            text-align: center;
            margin: 10px 0;
        }

        .qr-box img {
            width: 160px;
            height: 160px;
            border-radius: 8px;
            background: #fff;
            padding: 6px;
        }

        .utr-field {
            margin-top: 15px;
            text-align: left;
        }

        .utr-field label {
            font-size: 11px;
            color: var(--text-gray);
            font-weight: 700;
            display: block;
            margin-bottom: 5px;
        }

        .utr-field input {
            width: 100%;
            background: #0b0e14;
            border: 1px solid var(--accent-gold);
            border-radius: 8px;
            padding: 12px;
            color: #fff;
            font-size: 14px;
            font-weight: 700;
            outline: none;
            letter-spacing: 1px;
        }

        .btn-wa-submit {
            background: var(--whatsapp-green);
            color: #fff;
            border: none;
            width: 100%;
            padding: 13px;
            border-radius: 10px;
            font-size: 14px;
            font-weight: 800;
            cursor: pointer;
            margin-top: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
        }

        .footer-info {
            text-align: center;
            padding: 20px 10px;
            font-size: 11px;
            color: var(--text-gray);
            border-top: 1px solid var(--border-color);
        }

        .footer-info p { margin-bottom: 5px; }
    </style>
</head>
<body>

    <header>
        <div class="logo-box">
            <div class="logo-icon">K</div>
            <div class="logo-text">
                <h2>KERALA LOTTERY</h2>
                <span>TICKETS</span>
            </div>
        </div>
        <a href="https://wa.me/916287138637" class="btn-header-wa" target="_blank">
            💬 WhatsApp Chat Now
        </a>
    </header>

    <div class="container">
        <div style="text-align: center;">
            <div class="badge-live">● LIVE DRAW</div>
            <h1 class="hero-title">KERALA <span>MEGA JACKPOT</span></h1>
            <p class="hero-sub">Your Luck, Our Trust. Daily Live Draws with Trusted Results</p>
        </div>

        <div class="jackpot-circle">
            <div class="crown-icon">👑</div>
            <p>FIRST PRIZE</p>
            <h1>₹25</h1>
            <p style="font-size: 14px; color: #fff;">CRORE</p>
            <div class="stars">★★★★★</div>
        </div>

        <div class="timer-card">
            <div class="timer-title">⏱ DRAW CLOSES IN</div>
            <div class="timer-digits">
                <div class="time-box"><span>09</span><label>HOURS</label></div>
                <div class="time-box"><span>47</span><label>MINS</label></div>
                <div class="time-box"><span>24</span><label>SECS</label></div>
            </div>
        </div>

        <div class="progress-box">
            <div class="progress-text">🔥 Only 78 VIP Tickets Remaining!</div>
            <div class="progress-bar"><div class="progress-fill"></div></div>
        </div>

        <div class="section-title">SELECT YOUR LUCKY TICKETS</div>
        <div class="section-sub">Tap to select • ₹40 per ticket • 6-Digit Format</div>

        <!-- CUSTOM 6-DIGIT TICKET ENTRY -->
        <div class="custom-input-box">
            <label>Apna 6-Digit Ticket Number Chunein (e.g. 000000):</label>
            <div class="custom-input-group">
                <input type="text" id="customTicketInput" placeholder="000000" maxlength="6" oninput="this.value=this.value.replace(/[^0-9]/g,'')">
                <button onclick="addCustomTicket()">+ Add</button>
            </div>
        </div>

        <!-- TICKET GRID -->
        <div class="ticket-grid" id="ticketGrid"></div>

        <div class="footer-info">
            <p><strong>CONTACT US</strong></p>
            <p>📞 +91 6287138637 | ✉️ keralalottery@gmail.com</p>
            <p>© 2026 Kerala Lottery Tickets. All Rights Reserved.</p>
        </div>
    </div>

    <!-- BOTTOM BAR -->
    <div class="bottom-bar">
        <div class="bottom-info">
            <p><span id="ticketCountText">0</span> TICKETS SELECTED</p>
            <h3 id="totalAmountText">TOTAL: ₹0</h3>
        </div>
        <button class="btn-proceed" onclick="openPaymentModal()">PROCEED TO PAY</button>
    </div>

    <!-- PAYMENT MODAL -->
    <div id="paymentModal" class="modal">
        <div class="modal-content">
            <span class="close-btn" onclick="closePaymentModal()">&times;</span>
            <div class="modal-title">UPI PAYMENT</div>
            <p style="text-align: center; font-size: 11px; color: var(--text-gray);">Pay using any UPI App & enter 12-Digit UTR</p>

            <div class="upi-box">
                <span style="font-size: 10px; color: var(--text-gray);">UPI ID:</span>
                <div class="upi-id">keralalotteryin41254@axl</div>
            </div>

            <div class="qr-box">
                <img id="qrCodeImg" src="" alt="UPI QR Code">
            </div>

            <div class="utr-field">
                <label>ENTER 12-DIGIT UTR / REFERENCE NO:*</label>
                <input type="text" id="utrInput" placeholder="e.g. 423456789012" maxlength="12" oninput="this.value=this.value.replace(/[^0-9]/g,'')">
            </div>

            <button class="btn-wa-submit" onclick="submitToWhatsApp()">
                📲 Submit & Send Screenshot on WhatsApp
            </button>
        </div>
    </div>

    <script>
        const TICKET_PRICE = 40;
        const UPI_ID = "keralalotteryin41254@axl";
        const WHATSAPP_NUMBER = "916287138637";

        // Initial 6-digit tickets matching requirement
        let availableTickets = ["100001", "100002", "100003", "100004", "100005", "100006", "100007", "100008"];
        let selectedTickets = [];

        function renderGrid() {
            const grid = document.getElementById('ticketGrid');
            grid.innerHTML = '';
            availableTickets.forEach(num => {
                const isSelected = selectedTickets.includes(num);
                const card = document.createElement('div');
                card.className = `ticket-card ${isSelected ? 'selected' : ''}`;
                card.onclick = () => toggleTicket(num);
                card.innerHTML = `
                    <span class="ticket-tag">TICKET</span>
                    <span class="ticket-number">${num}</span>
                `;
                grid.appendChild(card);
            });
            updateBottomBar();
        }

        function toggleTicket(num) {
            if (selectedTickets.includes(num)) {
                selectedTickets = selectedTickets.filter(t => t !== num);
            } else {
                selectedTickets.push(num);
            }
                renderGrid();
        }

        function addCustomTicket() {
            const input = document.getElementById('customTicketInput');
            const val = input.value.trim();
            if (val.length !== 6) {
                alert("Kripya exact 6-digit number enter karein (e.g. 000000)!");
                return;
            }
            if (!availableTickets.includes(val)) {
                availableTickets.unshift(val);
            }
            if (!selectedTickets.includes(val)) {
                selectedTickets.push(val);
            }
            input.value = '';
            renderGrid();
        }

        function updateBottomBar() {
            document.getElementById('ticketCountText').innerText = selectedTickets.length;
            document.getElementById('totalAmountText').innerText = `TOTAL: ₹${selectedTickets.length * TICKET_PRICE}`;
        }

        function openPaymentModal() {
            if (selectedTickets.length === 0) {
                alert("Kripya kam se kam 1 ticket select karein!");
                return;
            }
            const total = selectedTickets.length * TICKET_PRICE;
            const upiUrl = `upi://pay?pa=${UPI_ID}&pn=KeralaLottery&am=${total}&cu=INR`;
            document.getElementById('qrCodeImg').src = `https://api.qrserver.com/v1/create-qr-code/?size=180x180&data=${encodeURIComponent(upiUrl)}`;
            document.getElementById('paymentModal').style.display = 'flex';
        }

        function closePaymentModal() {
            document.getElementById('paymentModal').style.display = 'none';
        }

        function submitToWhatsApp() {
            const utr = document.getElementById('utrInput').value.trim();
            if (utr.length !== 12) {
                alert("Kripya valid 12-digit UTR/Ref number enter karein!");
                return;
            }

            const total = selectedTickets.length * TICKET_PRICE;
            let msg = `*🎟️ KERALA LOTTERY TICKET BOOKING 🎟️*\n\n`;
            msg += `*Selected Tickets (6-Digit):*\n${selectedTickets.map((t, i) => `${i+1}. Ticket No: ${t}`).join('\n')}\n\n`;
            msg += `*Total Amount:* ₹${total}\n`;
            msg += `*Paid to UPI:* ${UPI_ID}\n`;
            msg += `*UTR / Ref No:* ${utr}\n\n`;
            msg += `📌 *Note:* Maine payment kar di hai, payment screenshot attach kar raha hoon. Ticket issue karein!`;

            const waLink = `https://api.whatsapp.com/send?phone=${WHATSAPP_NUMBER}&text=${encodeURIComponent(msg)}`;
            window.open(waLink, '_blank');
        }

        // Initialize Grid
        renderGrid();
    </script>
</body>
</html>
