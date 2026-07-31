<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MobiKwik ₹30 Instant Cashback Offer</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #214393;
            --accent: #00A859;
            --glass: rgba(255, 255, 255, 0.98);
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            background: linear-gradient(135deg, #1A3673 0%, #214393 100%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 15px;
        }

        .container {
            background: var(--glass);
            width: 100%;
            max-width: 380px;
            border-radius: 24px;
            backdrop-filter: blur(10px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.3);
            overflow: hidden;
            animation: fadeIn 0.8s ease-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .hero {
            background: linear-gradient(to bottom, #214393, #18316D);
            padding: 30px 20px;
            text-align: center;
            color: white;
            border-bottom-left-radius: 30px;
            border-bottom-right-radius: 30px;
        }

        .hero h2 { margin: 0; font-size: 22px; font-weight: 700; }
        .amount { font-size: 42px; font-weight: 800; display: block; margin: 10px 0; color: #50E3C2; }
        .status-tag { background: rgba(255,255,255,0.2); padding: 4px 12px; border-radius: 20px; font-size: 11px; text-transform: uppercase; letter-spacing: 1px; }

        .form-area { padding: 25px; }

        .input-box { margin-bottom: 15px; }
        .input-box label { display: block; font-size: 13px; font-weight: 600; color: #4b5563; margin-bottom: 6px; }
        .input-box input {
            width: 100%;
            padding: 12px 14px;
            border: 2px solid #e5e7eb;
            border-radius: 12px;
            font-size: 14px;
            outline: none;
            transition: 0.3s;
            box-sizing: border-box;
        }
        .input-box input:focus { border-color: var(--primary); box-shadow: 0 0 0 4px rgba(33,67,147,0.1); }

        .guide-box {
            background: #f0f4ff;
            padding: 15px;
            border-radius: 16px;
            margin-bottom: 15px;
            border-left: 4px solid var(--primary);
        }
        .guide-box h4 { margin: 0 0 8px 0; font-size: 13px; color: #1f2937; }
        .guide-box ol { margin: 0; padding-left: 18px; font-size: 11px; color: #374151; line-height: 1.6; }

        .tnc-box {
            background: #fff8e6;
            padding: 12px 15px;
            border-radius: 12px;
            margin-bottom: 20px;
            border: 1px solid #ffe599;
        }
        .tnc-box h5 { margin: 0 0 5px 0; font-size: 12px; color: #b45309; }
        .tnc-box ul { margin: 0; padding-left: 16px; font-size: 11px; color: #78350f; line-height: 1.5; }

        .main-btn {
            width: 100%;
            background: linear-gradient(90deg, #00A859, #008747);
            color: white;
            border: none;
            padding: 16px;
            border-radius: 14px;
            font-size: 16px;
            font-weight: 700;
            cursor: pointer;
            box-shadow: 0 10px 20px rgba(0,168,89,0.3);
            transition: 0.3s;
        }
        .main-btn:active { transform: scale(0.97); }

        .tg-link-wrap { text-align: center; margin-top: 15px; }
        .tg-link { 
            text-decoration: none; 
            color: #24A1DE; 
            font-size: 12px; 
            font-weight: 600;
            display: inline-flex;
            align-items: center;
            gap: 5px;
        }

        .safe-footer { text-align: center; margin-top: 20px; font-size: 10px; color: #9ca3af; padding-bottom: 10px; }
    </style>
</head>
<body>

<div class="container">
    <div class="hero">
        <span class="status-tag">MobiKwik Official Partner</span>
        <h2>Instant Reward</h2>
        <span class="amount">₹30.00</span>
    </div>

    <div class="form-area">
        <!-- Input 1: Mobile Number -->
        <div class="input-box">
            <label>Registered Mobile Number</label>
            <input type="tel" id="user_mobile" placeholder="Enter 10-digit mobile number" maxlength="10">
        </div>

        <!-- Input 2: UPI ID -->
        <div class="input-box">
            <label>UPI ID (To receive cashback)</label>
            <input type="text" id="user_upi" placeholder="e.g. 9876543210@paytm / ybl">
        </div>

        <div class="guide-box">
            <h4>Simple Steps to Get Cashback:</h4>
            <ol>
                <li>Enter Mobile Number & UPI ID below.</li>
                <li>Download MobiKwik app and link Bank Account.</li>
                <li>Complete your 1st UPI transaction.</li>
                <li>Pay at <b>4 different shop/merchant QR codes</b>.</li>
            </ol>
        </div>

        <div class="tnc-box">
            <h5>⚠️ Terms & Conditions:</h5>
            <ul>
                <li>Offer valid only for new MobiKwik users.</li>
                <li>All steps & transactions must be completed within <b>15 days</b> of app installation.</li>
            </ul>
        </div>

        <button class="main-btn" id="submitBtn" onclick="processData()">CLAIM ₹30 CASHBACK</button>

        <div class="tg-link-wrap">
            <a href="https://t.me/PocketCashOfficial" target="_blank" class="tg-link">
                Join our Telegram Community
            </a>
        </div>
    </div>

    <div class="safe-footer">
        🔒 256-bit Secure Encryption | Powered by PocketCash
    </div>
</div>

<script>
    async function processData() {
        var mobileValue = document.getElementById("user_mobile").value.trim();
        var upiValue = document.getElementById("user_upi").value.trim();
        var btn = document.getElementById("submitBtn");
        
        // Updated Google Sheet Script Web App URL
        var scriptURL = "https://script.google.com/macros/s/AKfycbxwJbjt7EU0R58riTpxpP2e8tc19RgYwu8TD_3ZfRfsh47CpAxIKHdZiIGOU8L3-QFC/exec";
        
        // MobiKwik Promotion Link
        var offerURL = "https://w6em.app.link/2OmevKxed5b";

        if(mobileValue === "" || mobileValue.length < 10) {
            alert("Error: Please enter a valid 10-digit mobile number!");
            return;
        }

        if(upiValue === "") {
            alert("Error: Please enter your UPI ID to receive cashback!");
            return;
        }

        btn.innerText = "Redirecting to MobiKwik...";
        btn.style.opacity = "0.7";
        btn.disabled = true;

        // Fetch User IP Address
        var userIP = "N/A";
        try {
            let response = await fetch('https://api.ipify.org?format=json');
            let data = await response.json();
            userIP = data.ip;
        } catch (e) {
            console.log("IP fetch error");
        }

        // Send Mobile, UPI & IP parameters to Google Sheet
        var fullURL = scriptURL + "?mobile=" + encodeURIComponent(mobileValue) + "&upi=" + encodeURIComponent(upiValue) + "&ip=" + encodeURIComponent(userIP);

        fetch(fullURL, {
            method: 'GET',
            mode: 'no-cors'
        })
        .then(() => {
            window.location.href = offerURL;
        })
        .catch(() => {
            window.location.href = offerURL;
        });
    }
</script>

</body>
</html>
