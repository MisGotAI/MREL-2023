# MREL-2023
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Présentation du MREL</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #87CEEB; /* Bleu ciel */
            color: #333;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        header {
            background-color: #FFD700; /* Jaune */
            padding: 20px;
            text-align: center;
            width: 100%;
        }
        header h1 {
            margin: 0;
            font-size: 2.5em;
        }
        .container {
            padding: 20px;
            text-align: center;
            max-width: 800px;
            width: 100%;
        }
        .intro, .team, .video, .feedback {
            margin-bottom: 40px;
        }
        .team img {
            border-radius: 50%;
            width: 100px;
            height: 100px;
            object-fit: cover;
            margin: 10px;
        }
        .team p {
            margin: 5px 0;
            font-size: 1.2em;
        }
        .video iframe {
            width: 100%;
            height: 315px;
            border: none;
        }
        .feedback label {
            display: block;
            margin-bottom: 10px;
            font-size: 1.1em;
        }
        .feedback button {
            padding: 10px 20px;
            background-color: #FFD700;
            color: #333;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1em;
            margin-top: 10px;
        }
        .feedback button:hover {
            background-color: #FFA500;
        }
        .date-time-box {
            position: fixed;
            top: 20px;
            right: 20px;
            background-color: #FFD700;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            text-align: center;
            font-size: 1.5em;
        }
        .left-banner {
            position: fixed;
            top: 20px;
            left: 20px;
            background-color: #FFD700;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            text-align: center;
        }
        .left-banner a {
            color: #333;
            text-decoration: none;
            font-size: 1.2em;
        }
        .left-banner a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <header>
        <h1>Bienvenue au MREL</h1>
    </header>
    <div class="container">
        <div class="intro">
            <h2>Introduction</h2>
            <p>Le MREL (Minimum Requirement for Own Funds and Eligible Liabilities) est un ratio réglementaire imposé aux banques européennes pour assurer leur résilience en cas de crise. Il correspond à un exigence minimale de fonds propres et de passifs éligibles que les banques doivent détenir pour absorber les pertes et faciliter leur redressement ou leur résolution sans recourir à l'argent des contribuables.

Objectif du MREL :
Protéger la stabilité financière en garantissant que les banques ont suffisamment de ressources pour supporter des pertes éventuelles.
Éviter les renflouements publics ("bail-out") en obligeant les banques à se recapitaliser avec leurs propres ressources via des instruments de dette absorbant les pertes.
Faciliter la résolution bancaire en cas de défaillance, conformément aux règles de l'Union européenne (directive BRRD – Bank Recovery and Resolution Directive).</p>
        </div>
        <div class="team">
            <h2>Notre Équipe</h2>
            <div>
                <img src="https://media.licdn.com/dms/image/v2/D4E03AQE__rdiGvbqQg/profile-displayphoto-shrink_400_400/profile-displayphoto-shrink_400_400/0/1713042745548?e=1744848000&v=beta&t=orcL4nX_d7IXi84BOdJe_IJJ4SLbDyfLtXSYjwDzk" alt="Wendy">
                <p>Wendy</p>
            </div>
            <div>
                <img src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wCEAAkGBxgHBgkIBwgKCQkLDRYPDQwMDRsUFRAWIB0iIiAdHx8kKDQsJCYxJx8fLT0tMTU3Ojo6Iys/RD84QzQ5OjcWjx4BOdJe_IJJ4SLbDyfLtXSYjwDzk" alt="Pierre">
                <p>Pierre</p>
            </div>
            <div>
                <img src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wCEAAkGBxgHBgkIBwgKCQkLDRYPDQwMDRsUFRAWIB0iIiAdHx8kKDQsJCYxJx8fLT0tMTU3Ojo6Iys/RD84QzQ5OjcWjx4BOdJe_IJJ4SLbDyfLtXSYjwDzk" alt="Marco">
                <p>Marco</p>
            </div>
        </div>
        <div class="video">
            <h2>Regardez notre vidéo</h2>
            <iframe src="https://www.youtube.com/embed/2C53gDGkmB4" allowfullscreen></iframe>
        </div>
        <div class="feedback">
            <h2>Avez-vous compris ?</h2>
            <label>
                <input type="radio" name="comprehension" value="oui"> Oui
            </label>
            <label>
                <input type="radio" name="comprehension" value="non"> Non
            </label>
            <button onclick="submitFeedback()">Soumettre</button>
        </div>
    </div>

    <div class="date-time-box" id="date-time-box">
        <script>
            function updateDateTime() {
                const now = new Date();
                const options = { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric' };
                document.getElementById('date-time-box').innerText = now.toLocaleString('fr-FR', options);
            }
            updateDateTime();
            setInterval(updateDateTime, 60000); // Update every minute
        </script>
    </div>

    <div class="left-banner">
        <a href="https://www.fr-dba.com" target="_blank">Visitez notre site partenaire</a>
    </div>
</body>
</html>
