<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Parrot Facts</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .parrot-card {
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        h1 {
            color: #ff6347;
            text-align: center;
        }

        ul {
            list-style-type: none;
            padding: 0;
        }

        li {
            background-color: #e0f7fa;
            margin: 10px 0;
            padding: 10px;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <div class="parrot-card">
        <h1>Interesting Facts About Parrots</h1>
        <ul id="facts-list">
            <!-- Facts will be added by JavaScript -->
        </ul>
    </div>
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const facts = [
                "Varied Species: There are around 393 species of parrots found across the world, predominantly in tropical and subtropical regions.",
                "Longevity: Some parrot species can live for a long time, with lifespans ranging from 20 to over 80 years in captivity.",
                "Vocal Mimicry: Parrots are renowned for their ability to mimic human speech and other sounds, thanks to their advanced vocal apparatus.",
                "Diet: Most parrots eat a diet consisting of seeds, nuts, fruits, and occasionally insects. Some species have specialized diets, like the lorikeets, which feed on nectar and pollen.",
                "Monogamous Bonds: Many parrot species form monogamous pair bonds, often remaining with the same partner for life.",
                "Strong Beaks: Parrots have strong, curved beaks which are great for cracking open tough nuts and seeds.",
                "Zygodactyl Feet: Their feet have a unique structure with two toes pointing forward and two pointing backward, which helps them grasp and manipulate objects.",
                "Endangered Species: Unfortunately, many parrot species are threatened or endangered due to habitat loss, the pet trade, and other human activities."
            ];

            const factsList = document.getElementById('facts-list');

            facts.forEach(fact => {
                const listItem = document.createElement('li');
                listItem.textContent = fact;
                factsList.appendChild(listItem);
            });
        });
    </script>
</body>
</html>
