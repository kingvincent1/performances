<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Live Music Event Flyer</title>
    <style>
        :root {
            --primary-color: #ff4757;
            --secondary-color: #ffa502;
            --bg-dark: #1e1e24;
            --card-bg: #2f3542;
            --text-light: #ffffff;
            --text-muted: #a4b0be;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--bg-dark);
            color: var(--text-light);
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 20px;
        }

        .flyer-container {
            background: linear-gradient(135deg, var(--card-bg) 0%, #1e1e24 100%);
            width: 100%;
            max-width: 500px;
            border: 3px solid var(--primary-color);
            border-radius: 15px;
            padding: 40px 30px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
            position: relative;
            overflow: hidden;
        }

        /* Decorative music accent */
        .flyer-container::before {
            content: "🎵";
            position: absolute;
            top: -20px;
            right: -10px;
            font-size: 8rem;
            opacity: 0.05;
            pointer-events: none;
        }

        .header-tag {
            background-color: var(--primary-color);
            color: white;
            display: inline-block;
            padding: 6px 16px;
            border-radius: 20px;
            font-size: 0.9rem;
            text-transform: uppercase;
            letter-spacing: 2px;
            font-weight: bold;
            margin-bottom: 20px;
        }

        .headline {
            font-size: 2.5rem;
            margin-bottom: 10px;
            color: white;
            line-height: 1.2;
        }

        .vocalist-names {
            font-size: 1.3rem;
            color: var(--secondary-color);
            margin-bottom: 25px;
            font-weight: 600;
            letter-spacing: 1px;
        }

        .description {
            color: var(--text-muted);
            font-size: 1.05rem;
            line-height: 1.6;
            margin-bottom: 30px;
            padding: 0 10px;
        }

        .details-box {
            background-color: rgba(0, 0, 0, 0.2);
            border-radius: 10px;
            padding: 20px;
            margin-bottom: 30px;
            border-left: 4px solid var(--secondary-color);
        }

        .detail-row {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 12px;
            font-size: 1.1rem;
        }

        .detail-row:last-child {
            margin-bottom: 0;
        }

        .label {
            color: var(--text-muted);
            font-weight: 500;
            text-transform: uppercase;
            font-size: 0.85rem;
            letter-spacing: 1px;
        }

        .value {
            font-weight: 600;
            text-align: right;
        }

        .price-tag {
            font-size: 1.4rem;
            color: #2ed573;
            font-weight: bold;
            margin-top: 5px;
        }

        .price-note {
            font-size: 0.85rem;
            color: var(--text-muted);
            display: block;
            font-weight: normal;
            font-style: italic;
        }

        .footer-info {
            border-top: 1px solid rgba(255,255,255,0.1);
            padding-top: 25px;
        }

        .phone-link {
            display: inline-block;
            color: var(--primary-color);
            font-size: 1.3rem;
            font-weight: bold;
            text-decoration: none;
            margin-top: 5px;
            transition: color 0.2s;
        }

        .phone-link:hover {
            color: var(--secondary-color);
        }
    </style>
</head>
<body>

    <div class="flyer-container">
        <span class="header-tag">Live Performance</span>
        
        <!-- Artists -->
        <h1 class="headline">An Intimate Evening Of Jazz</h1>
        <div class="vocalist-names">Featuring vocalist Victoria Rosemond & pianist Vince Robinson</div>
        
        <!-- Brief Description -->
        <p class="description">
            Join us for an exclusive, one-night-only musical experience. Enjoy a soulful blend of jazz, stripped-down acoustic arrangements, and powerful vocal storytelling.
        </p>
        
        <!-- Event Logistics -->
        <div class="details-box">
            <div class="detail-row">
                <span class="label">Date</span>
                <span class="value">Saturday, November 14, 2026</span>
            </div>
            <div class="detail-row">
                <span class="label">Time</span>
                <span class="value">6:00PM - 9:00PM</span>
            </div>
            <div class="detail-row">
                <span class="label">Location</span>
                <span class="value">
                    <strong> Larchmere Arts</strong><br>
                    12726 Larchmere Blvd<br>
                    Cleveland, Ohio
                </span>
            </div>
            <div class="detail-row" style="margin-top: 15px; padding-top: 15px; border-top: 1px dashed rgba(255,255,255,0.1);">
                <span class="label">Admission</span>
                <span class="value price-tag">
                    $15 <span class="price-note">at the door</span>
                    <span class="price-note">*includes refreshments*</span>
                </span>
            </div>
        </div>
        
        <!-- Contact / Action Call -->
        <div class="footer-info">
            <span class="label">For More Information</span><br>
            <a href="tel:1234567890" class="phone-link">Call (216) 780-2470</a>
        </div>
    </div>

</body>
</html>
