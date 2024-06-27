# Projekt-f-r-den-Kurs-Programmierung-von-Webanwendungsoberfl-chen-
<!DOCTYPE html>
<html lang="de">
    <head>
        <title> Kleiderspende "Gute Sachen" </title>
        <link rel="Stylesheet"
        href="https://cdn.jsdelivr.net/npm/bootstrap@5.2/dist/css/bootstrap.min.css">
        <meta name="viewpoint" content="width=device-width, initial-scale=1.0">
        <title> Homepage von Kleiderspende "Gute Sachen"</title>
        <style type="text/css">
            header {background-color: rgb(255, 184, 175);}
            header nav ul {text-align: right}
            header nav ul li {display: inline;}
            main {display: flex;}
            main nav {width: 40%; float: left; background-color: rgb(156, 156, 255);}
            main div#content {width: 60%; float: left; background-color: #aff;}
            footer {clear: both; background-color: rgb(243, 191, 191);}
            footer nav ul {text-align: center;}
            footer nav ul li {display: inline;}
            @media screen and (max-width: 767px) {
                main {display: block;}
                main nav, main div#content {width: 100%;}
            }
            p {color: coral;}
            h1{
                background-color: rgb(255, 255, 255);
                padding: 1em;
                border: 5px solid black;
            }
            h1, h2 {color: rgb(253, 34, 34);}
            table {font-size: 200%;}
            body {background-color: antiquewhite;}

        </style>
    </head>
    <body> 
        
        <h1> Kleiderspende "Gute Sachen"<img src="data:image/png;base64,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" alt="Logo von Kleiderspendestiftuing" width="100" height="100" align="right"></h1>
        <h2> Gib deine Kleidung zweite Chance!</h2>
        
        <header>
            <nav>
                <ul class="text-end">
                    <li class="d-inline">
                        <form>
                            <input type="text" name="suche" placeholder="Suche">
                        </form>
                    </li>
                    <li class="d-inline"><a 
                        href="https://www.kleiderstiftung.de/kontakt">Deutsche Kleiderstiftung</a></li>
                </ul>
            </nav>
        </header>
        <p>
            Die Wohltätigkeitsstiftung "Gute Sachen" ist die größte gemeinnützige Organisation in Deutschland, die Kleidung annimmt und an Menschen aus sozial benachteiligten Gruppen und gefährlichen oder einkommensschwachen Regionen weitergibt.
            Jedes Jahr landen in Deutschland Millionen Tonnen Kleidung auf Mülldeponien. Es dauert bis zu 200 Jahre, bis sich Kleidung zersetzt. Dabei wird Methan freigesetzt, das den Boden und das Grundwasser verunreinigt und das Volumen von Mülldeponien vergrößert.
        </p>


        <h3>
            Formular, mit dem die Kleiderspende regestriert werden kann 
        </h3>
        <h5>Name (*)</h5>
        <form>
            <input type="text" name="name" placeholder="Vorname">
        </form>
        <form>
            <input type="text" name="surename" placeholder="Nachname">
        </form>
        <h5>Adresse (*)</h5>
        <form>
            <input type="text" name="plz" placeholder="Postleitzahl">
        </form>
        <form>
            <input type="text" name="city" placeholder="Stadt">
        </form>
        <form>
            <input type="text" name="street" placeholder="Straße">
        </form>
        <form>
            <input type="text" name="house number" placeholder="Hausnummer">
        </form>
        <h5>E-Mail</h5>
        <form>
            <input type="text" name="e-mail" placeholder="beispiel@beispiel.de">
        </form>
        <h5>Telefonnummer (*)</h5>
        <form>
            <input type="text" name="e-mail" placeholder="Eine gültige Telefonnummer eingeben!">
        </form>

        <h5>Art des Übergebens (*)</h5>
        <input name="art des uebergebens" type="radio"> An der Geschäftsstelle übergeben
        <input name="art des uebergebens" type="radio"> Die Kleidung sollte von einem Sammelfahrzeug abgeholt werden

        <h5>Falls Sie die Kleidung an der Geschäftsstelle übergeben möchten, dann suchen Sie eine Geschäftsstelle in Ihre Nähe </h5>
        <form>
            <input type="text" name="plz geschaeftsstelle" placeholder="Postleitzahl der Geschäftsstelle">
        </form>
        <h5>Wie ist der Zustand des Kleides? (*)</h5>
        <input name="zustand" type="radio"> Brandneu
        <input name="zustand" type="radio"> Sehr guter Zustand
        <input name="zustand" type="radio"> Guter Zustand
        <input name="zustand" type="radio"> Durchschnittlicher Zustand
        <input name="zustand" type="radio"> Schlechter Zustand
        


        <h5>Aus welchem Stoff ist die Kleidung?</h5>
        <fieldset> 
            <input type="checkbox" name="stoff" value="baumwollgewebe" id="check1">
            <label for="check1">Baumwollgewebe</label>
            <input type="checkbox" name="stoff" value="leinenstoff" id="check2">
            <label for="check2">Leinenstoff</label>
            <input type="checkbox" name="stoff" value="leder" id="check3">
            <label for="check3">Leder</label>
            <input type="checkbox" name="stoff" value="chiffon" id="check4">
            <label for="check4">Chiffon</label>
            <input type="checkbox" name="stoff" value="polyester" id="check5">
            <label for="check5">Polyester</label>
            <input type="checkbox" name="stoff" value="denim" id="check6">
            <label for="check6">Denim</label>
            <input type="checkbox" name="stoff" value="viskose" id="check 7"
            <label for="check7">Viskose</label>
            <input type="checkbox" name="stoff" value="krepp" id="check 8"
            <label for="check8">Krepp</label>
            <input type="checkbox" name="stoff" value="netz- oder spitzenstoff" id="check 9"
            <label for="check9">Netz- oder Spitzenstoff</label>
            <input type="checkbox" name="stoff" value="seidenstoff" id="check 10"
            <label for="check10">Seidenstoff</label>
            <input type="checkbox" name="stoff" value="wolle" id="check 11"
            <label for="check11">Wolle</label>
            <input type="checkbox" name="stoff" value="georgette" id="check 12"
            <label for="check12">Georgette</label>
            <input type="checkbox" name="stoff" value="nylon" id="check 13"
            <label for="check13">Nylon</label>
            <input type="checkbox" name="stoff" value="samt" id="check 14"
            <label for="check14">Samt</label>
            <input type="checkbox" name="stoff" value="rayon" id="check 15"
            <label for="check15">Rayon</label>
            <input type="checkbox" name="stoff" value="satin" id="check 16"
            <label for="check16">Satin</label>
            <input type="checkbox" name="stoff" value="lycra" id="check 17"
            <label for="check17">Lycra</label>
            <input type="checkbox" name="stoff" value="anderer stoff" id="check 18"
            <label for="check18">Anderer Stoff</label>
        </fieldset>

        <h5>Art der Kleidung (*)</h5>
        <fieldset> 
            <input type="checkbox" name="art der kleidung" value="hemd/bluse" id="check1">
            <label for="check1">Hemd/Bluse</label>
            <input type="checkbox" name="art der kleidung" value="hose" id="check2">
            <label for="check2">Hose</label>
            <input type="checkbox" name="art der kleidung" value="kleid, rock" id="check3">
            <label for="check3">Kleid, Rock</label>
            <input type="checkbox" name="art der kleidung" value="pullover/sweatshirt" id="check4">
            <label for="check4">Pullover/Sweatshirt</label>
            <input type="checkbox" name="art der kleidung" value="t-shirt" id="check5">
            <label for="check5">T-Shirt</label>
            <input type="checkbox" name="art der kleidung" value="jacke" id="check6">
            <label for="check6">Jacke</label>
            <input type="checkbox" name="art der kleidung" value="sportanzug" id="check7">
            <label for="check7">Sportanzug</label>
            <input type="checkbox" name="art der kleidung" value="pyjama/Bademantel" id="check8">
            <label for="check8">Pyjama/Bademantel</label>
            <input type="checkbox" name="art der kleidung" value="schuhe" id="check9">
            <label for="check9">Schuhe</label>
            <input type="checkbox" name="art der kleidung" value="socken" id="check10">
            <label for="check10">Socken</label>
            <input type="checkbox" name="art der kleidung" value="muetze" id="check11">
            <label for="check11">Mütze</label>
            <input type="checkbox" name="art der kleidung" value="babykleidung" id="check12">
            <label for="check12">Babykleidung</label>
            <input type="checkbox" name="art der kleidung" value="andere kleidungsstuecke" id="check13">
            <label for="check13">Andere Kleidungsstücke</label>


        <nav>
            <ul>
                <li><a href="home.html"Homepage</li>
                <li> <a href="services.html"Kleidung spenden</li>
                <li><a href="about.html"Über uns</li>
            </ul>
        </nav>
        <footer> 
            <nav>
                <ul>
                    <li></li>
                </ul>
            </nav>
        </footer>
    </body>
</html>
