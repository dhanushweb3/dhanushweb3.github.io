<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dhanush Kumar | Web3 Professional</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500&family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" rel="stylesheet">
    <style>
        body { 
            font-family: 'Open Sans', sans-serif; 
            margin: 0; 
            padding: 0; 
            background-color: #121212; 
            color: #fff;
            overflow-x: hidden;
            overflow-y: auto;
        }
        .hero {
            height: 100vh;
            background: url('https://img.freepik.com/free-vector/gradient-hexagonal-background_23-2148944165.jpg?semt=ais_hybrid') no-repeat center center/cover;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            position: relative;
            background-size: cover;
            background-position: center center;
        }
        .hero h1 {
            font-size: 4rem;
            color: #fff;
            z-index: 1;
            text-shadow: 2px 2px 6px rgba(0, 0, 0, 0.6);
        }
        .hero p {
            font-size: 1.5rem;
            color: #fff;
            z-index: 1;
            text-shadow: 2px 2px 6px rgba(0, 0, 0, 0.6);
        }
        .hero .cta-button {
            margin-top: 20px;
            padding: 15px 30px;
            font-size: 1.2rem;
            background-color: #00bcd4;
            color: #fff;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
        .hero .cta-button:hover {
            background-color: #008c8c;
        }
        .section {
            padding: 80px 20px;
            text-align: center;
        }
        .projects, .claimed-airdrops, .interests, .contact {
            color: #fff;
            background: no-repeat center center/cover;
            padding: 60px 0;
        }
        .projects {
            background: url('https://img.freepik.com/free-vector/futuristic-hexagonal-net-background_23-2148345194.jpg') no-repeat center center/cover;
        }
        .claimed-airdrops {
            background: url('https://img.freepik.com/premium-photo/big-data-visualization-futuristic-hexagon-background-big-data-connection-background-3d-rendering_105800-2450.jpg?w=360') no-repeat center center/cover;
        }
        .interests {
            background: url('your-interests-bg-image-url.jpg') no-repeat center center/cover;
        }
        .contact {
            background: url('https://media.istockphoto.com/id/1367477512/photo/metaverse-web3-and-blockchain-technology-concepts-opened-hand-levitating-virtual-objects.jpg?s=612x612&w=0&k=20&c=KRP5D6xfPHI_ymgVNGvEV2gBF5XfKSbprJq54oMoitQ=') no-repeat center center/cover;
        }
        .projects, .claimed-airdrops, .interests, .contact {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 40px;
        }
        .card, .airdrop-card, .interest-card {
            background: linear-gradient(135deg, #f9f9f9, #ffffff);
            padding: 15px;
            border-radius: 8px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            width: 220px;
            text-align: center;
        }
        .card:hover, .airdrop-card:hover, .interest-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
        }
        .card img, .airdrop-card img, .interest-card img {
            max-width: 100%;
            height: auto;
            border-radius: 8px;
            transition: transform 0.3s ease;
        }
        .card:hover img, .airdrop-card:hover img, .interest-card:hover img {
            transform: scale(1.05);
        }
        .card h3, .airdrop-card h3, .interest-card h3 {
            color: #000;
            font-size: 1.2rem;
        }
        .card p, .interest-card p {
            color: #000;
            font-size: 1rem;
        }
        .contact-icons {
            display: flex;
            justify-content: center;
            gap: 40px;
            font-size: 2.5rem;
            margin-top: 40px;
        }
        .contact-icons a {
            color: #00bcd4;
            transition: color 0.3s ease;
        }
        .contact-icons a:hover {
            color: #008c8c;
        }
        footer {
            background: #00695c;
            padding: 20px;
            font-size: 0.9rem;
            text-align: center;
            color: #ffffff;
        }
        footer p {
            margin: 0;
        }
        /* Adjusted for smaller "Claimed Airdrops" cards */
        .claimed-airdrops .airdrop-card {
            width: 150px; /* Reduced size further */
        }
        .claimed-airdrops .airdrop-card img {
            max-width: 80%;
            margin: 0 auto;
        }
        /* Bold & Uppercase for Section Titles */
        h2 {
            font-weight: bold;
            text-transform: uppercase;
            color: #fff;
            margin-bottom: 30px;
        }
        /* Styling for "Contact Me" Section */
        .contact {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        .contact p {
            margin: 10px 0;
            font-size: 1.2rem;
            font-weight: bold;
            color: #fff;
        }
        .contact-icons a {
            color: #fff;
            font-size: 2rem;
            margin: 10px;
            transition: color 0.3s ease;
        }
        .contact-icons a:hover {
            color: #00bcd4;
        }
        .contact a {
            color: #00bcd4;
            text-decoration: none;
            font-weight: bold;
        }
        .contact a:hover {
            text-decoration: underline;
        }
        /* Adjusting the "Interested in" Section */
        .interests .interest-card {
            width: 220px;
            background: #fff;
            border-radius: 8px;
            text-align: center;
            padding: 20px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }
        .interests .interest-card img {
            max-width: 60%;
            height: auto;
            margin-bottom: 15px;
        }
        .interests .interest-card h3 {
            color: #000;
        }
        .interests .interest-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
        }
    </style>
</head>
<body>
    <div class="hero">
        <div>
            <h1>Dhanush Kumar</h1>
            <p>Community Manager | Marketing & Business Development | Web3 Enthusiast</p>
            <p style="color: #fff; font-size: 1rem;">I have 4 years of experience in the crypto industry and 2 years of hands-on involvement with Web3 projects. I’ve worked as a Community Manager, Collabs & Partnerships Manager, and Marketing & Business Development Assistant for top Web3 projects such as Zoppel Universe, Lucky Buy, 10k World Cup, and X Metaverse. Previously, I led a team at King Game.</p>
            <button class="cta-button" onclick="window.location.href='https://t.me/dondhanush5109r'"> SAY HI TO ME ON TELEGRAM </button>
        </div>
    </div>

    <div class="section projects" id="projects">
        <h2>WEB3 PROJECTS CONTRIBUTED</h2>
        <div class="card">
            <img src="https://miro.medium.com/v2/resize:fill:320:214/1*YXNppi5vU9Y2KOLoLNmY3A.png" alt="Zoppel Universe">
            <h3>Zoppel Universe</h3>
            <p>Driving Collaborations and Partnerships with other projects for market reach.</p>
        </div>
        <div class="card">
            <img src="https://coin-images.coingecko.com/nft_contracts/images/2273/large/10k.png?1707288275" alt="10k World Cup">
            <h3>10k World Cup</h3>
            <p>Established partnerships and collaborations with NFT projects and communities as freelancer.</p>
        </div>
        <div class="card">
            <img src="https://d1j2c9jkfhu70p.cloudfront.net/X_Metaverse_banner_4957123511.jpg" alt="X Metaverse">
            <h3>X Metaverse</h3>
            <p>Assisted in marketing activities, business development activities, and fostering partnerships under the head marketing officer.</p>
        </div>
        <div class="card">
            <img src="https://consumersiteimages.trustpilot.net/business-units/65b3554dd8f72eb1e03cb610-198x149-1x.avif" alt= <"King Game">
            <h3>King Game</h3>
            <p> Worked as a team leader where led my team to game testing , review , KOL collaorations and event plannings.</p>
        </div>
    </div>

    <div class="section claimed-airdrops" id="claimed-airdrops">
        <h2>CLAIMED AIRDROPS</h2>
        <div class="airdrop-card">
            <img src="https://aptosfoundation.org/brandbook/logomark/PNG/Aptos_mark_BLK.png" alt="Aptos">
            <h3>Aptos</h3>
        </div>
        <div class="airdrop-card">
            <img src="https://cryptologos.cc/logos/arbitrum-arb-logo.png" alt="Arbitrum">
            <h3>Arbitrum</h3>
        </div>
        <div class="airdrop-card">
            <img src="https://cryptologos.cc/logos/jupiter-ag-jup-logo.png" alt="Jupiter">
            <h3>Jupiter</h3>
        </div>
        <div class="airdrop-card">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQdgCiAXRBMDOVU6I7hPyyfx18aRRat5d5NoF-eiQiA23yzTJc6n5ZM8R1OXpdEd0llJE0&usqp=CAU" alt="Deep">
            <h3>Deep</h3>
        </div>
        <div class="airdrop-card">
            <img src="https://img.cryptorank.io/coins/notcoin1704281436837.png" alt="Notcoin">
            <h3>Notcoin</h3>
        </div>
        <div class="airdrop-card">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ5AfkbnwXZWteiLBlsHTw2IUZyrV0XsZtPDSSDdnpgH3UPW_5-fZJ93uTIvg68m0TUkWM&usqp=CAU" alt="Sui (ICO)">
            <h3>Sui (ICO)</h3>
        </div>
    </div>

    <div class="section interests" id="interests">
        <h2>INTERESTED IN</h2>
        <div class="interest-card">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSNXuVN_LWYteUwmRL6QNObROxGXzwzivu4Lg&s" alt="Airdrops">
            <h3>Airdrop Hunter</h3>
        </div>
        <div class="interest-card">
            <img src="https://img.freepik.com/free-vector/digital-asset-nft-blockchain-technology-background_1017-41103.jpg?ga=GA1.1.358523940.1734412138&semt=ais_hybrid" alt="Web Worker">
            <h3>NFT Enthusiast</h3>
        </div>
        <div class="interest-card">
            <img src="https://img.freepik.com/premium-vector/concept-illustration-nft-art-as-famous-painting-tablet-with-crypto-coins_658963-54.jpg?ga=GA1.1.358523940.1734412138&semt=ais_hybrid" alt="Blockchain">
            <h3>Content Creation</h3>
        </div>
        <div class="interest-card">
            <img src="https://img.freepik.com/free-psd/3d-nft-icon-chain_629802-28.jpg?ga=GA1.1.358523940.1734412138&semt=ais_hybrid" alt="Crypto">
            <h3> Decentralization</h3>
        </div>
    </div>

    <div class="section contact" id="contact">
        <h2>CONTACT ME</h2>
        <p>Feel free to reach out to discuss Web3 projects or collaborations!</p>
        <div class="contact-icons">
            <a href="https://x.com/undervaluednft" target="_blank" class="fab fa-twitter"></a>
            <a href="https://www.linkedin.com/in/dhanush-kumar-m-825023226/" target="_blank" class="fab fa-linkedin"></a>
            <a href="mailto:dhanushweb33@gmail.com" target="_blank" class="fas fa-envelope"></a>
        </div>
        <p><a href="mailto:dhanushweb33@gmail.com">Email me directly</a></p>
    </div>

    <footer>
        <p>&copy; 2025 Dhanush Kumar. All rights reserved.</p>
    </footer>
</body>
</html>
