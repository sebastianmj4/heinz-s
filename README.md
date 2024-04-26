Meine Idee ist einen Nachhaltigkeits-Tracker zu entwickeln. Es soll eine Anwendung sein die Benutzern helfen wird ihren ökologischen Fußabdruck zu verfolgen und gleichzeitig Tipps gibt ihren CO2-Ausstoß zu reduzieren. Sie könnte diese Funktionen haben: Eine persönliche CO2-Bilanzierung die genau aufzeigt wie viel, wo und was genau man wo verbraucht, Eine umweltfreundliche Einkaufsliste die verschiedene Produkte mit genauem C02 Ausstoß aufzeigt und gegebenenfalls alternativen für diese Produkte. 
Ich würde mich bei der CO-2 Bilanz auf den bereich der Ausstöße der Ernährung bzw. Lebensmittel beschränken. Die CO-2 bilanz dokumentiert also welche Lebensmittel welchen Ausstoß haben und wie dieser reduziert werden kann. Diese Daten sollten bearbeitet oder im nachhinein auch wieder gelöscht werden können. Vorgesehen ist das wenn etwas konsumiert wird wie beispielsweise eine Banane, diesin der App eingetragen werden kann und dort ihr CO-2 ausstoß agezeigt und dokumeniert wird. Unter jedem dokumentierten Lebensmittel soll ein Produkt angezeigt werden, das eine CO-2 freundlichere alternative zum dokumentierten produkt ist das dadurch emissionenn eingespart werden können. 
Die App soll so aufgebaut sein das wenn man auf die Startseite kommt, die persönliche CO2-Bilanzierung direkt auf der Hauptseite zu sehen ist. Links oben soll ein Menü zeichen eingeblendet sein welches sich durch ein klick oder tippen öffnen lässt. In diesem Menü sind verschiedenen Anwendungen wie die Einkaufsliste möglich. Die App muss auf perönliche Daten zugreifen müssen, um beispielsweise eine perönliche CO2-Bilanzierung oder eine umweltfreundliche Einkaufsliste zu erstellen. Die App soll auf allen Mobilen Geräten (Smartphone, Laptop, Computer, etc.) zum kostenlosen Download zur verfügung gestellt werden.

<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CO-2 Bilanz</title>
    <style>
        
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0; 
        }

       
        header {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 20px 0;
        }

        header h1 {
            margin: 0;
        }

        #menu-toggle {
            position: absolute;
            top: 10px;
            left: 10px;
            font-size: 24px;
            cursor: pointer;
            color: #fff;
        }

     
        main {
            text-align: center;
            padding: 20px;
        }

        .food {
            display: inline-block;
            background-color: #4CAF50; 
            color: #fff; 
            padding: 10px;
            margin: 20px auto; 
            border-radius: 15px; 
        }

        .food-name {
            display: block;
            font-weight: bold;
        }

       
        #stats {
            background-color: #f0f0f0;
            padding: 20px;
            margin-bottom: 20px;
            border-radius: 5px;
        }

       
        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 10px;
            position: fixed;
            width: 100%;
            bottom: 0;
        }

       
        .food-alternative {
            color: blue; 
            font-style: italic; 
        }

       
        #menu-toggle::before {
            content: "Menü öffnen";
            position: absolute;
            clip: rect(0 0 0 0);
            width: 1px;
            height: 1px;
            overflow: hidden;
        }
    </style>
</head>
<body>
    <header>
        <h1>XY's Nachhaltigkeits-Tracker</h1>
        <nav id="menu-toggle" aria-label="Menü">&#9776;</nav>
    </header>
    <main>
        <div id="earth">
            <h2>Persönliche Lebensmittel</h2>
            <div class="food" id="food1">
                <span class="food-name">Chiasamen</span>
                <span class="food-co2">CO2: 30%</span>
                <span class="food-alternative">Alternative: Alternative 1</span>
            </div>
            <div class="food" id="food2">
                <span class="food-name">Rindfleisch</span>
                <span class="food-co2">CO2: 40%</span>
                <span class="food-alternative">Alternative: Alternative 2</span>
            </div>
            <div class="food" id="food3">
                <span class="food-name">Erdbeeren</span>
                <span class="food-co2">CO2: 30%</span>
                <span class="food-alternative">Alternative: Alternative 3</span>
            </div>
            <div class="food" id="food4">
                <span class="food-name">Nutella</span>
                <span class="food-co2">CO2: 100%</span>
                <span class="food-alternative">Alternative: Alternative 4</span>
            </div>
            <div class="food" id="food5">
                <span class="food-name">Avocado</span>
                <span class="food-co2">CO2: 50%</span>
                <span class="food-alternative">Alternative: Alternative 5</span>
            </div>
            <div class="food" id="food6">
                <span class="food-name">Lachs</span>
                <span class="food-co2">CO2: 60%</span>
                <span class="food-alternative">Alternative: Alternative 6</span>
            </div>
            <div class="food" id="food7">
                <span class="food-name">Käse</span>
                <span class="food-co2">CO2: 70%</span>
                <span class="food-alternative">Alternative: Alternative 7</span>
            </div>
            <div class="food" id="food8">
                <span class="food-name">Quinoa</span>
                <span class="food-co2">CO2: 20%</span>
                <span class="food-alternative">Alternative: Alternative 8</span>
            </div>
        </div>
        <div id="stats">
            <h2>Alternativen</h2>
            <p>Hier werden die persönlichen Alternativen angezeigt und ausführlich erklärt.</p>
        </div>
    </main>
    <footer>
        <p>Persönliche Einkaufsliste</p>
    </footer>
</body>
</html>
