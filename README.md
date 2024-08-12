<!DOCTYPE html>
<html lang="pl-PL">
<head>
    <meta charset="utf-8">
    <title>ZADANIE FORMULARZ</title>
    <style>
        body {
            background-color: #87CEFA;
            font-family: Arial, sans-serif;
        }
        h1 {
            font-size: 2em;
            color: red;
        }
        table {
            width: 100%;
            border-collapse: collapse;
        }
        td {
            padding: 10px;
        }
        input[type="text"], input[type="time"], input[type="date"], input[type="color"], input[type="range"], textarea {
            width: 100%;
        }
        button, input[type="reset"], input[type="submit"] {
            height: 80px;
            width: 150px;
        }
        button {
            width: 300px;
        }
        select {
            width: 100%;
        }
    </style>
</head>
<body>
    <center>
        <h1>Formularz </h1>
    </center>
    <form enctype="text/plain" action="mailto:mkryniew@wp.pl" subject="formularz_dane" method="post">
        <table>
            <tr height="100">
                <td width="500">
                    <b>Imię</b><br>
                    <input name="imie" type="text" size="22"><br><br>
                    <b>Drugie imię</b><br>
                    <input name="drugie" type="text" size="22"><br><br>
                    <b>Nazwisko</b><br>
                    <input name="nazwisko" type="text" size="22"><br><br>
                    <b>Pseudonim artystyczny</b><br>
                    <input name="login" type="text" size="22"><br><br>
                </td>
                <td width="300">
                    <center>
                        <font size="5" color="red"><b>Podaj środek lokomacji dojazdu do pracy</b></font>
                        <br><br>
                        <select name="srodek">
                            <option value="autobus">Autobus</option>
                            <option value="motocykl">Motocykl</option>
                            <option value="prom">Prom</option>
                            <option value="samolot">Samolot</option>
                            <option value="lodz">Łódź podwodna</option>
                            <option value="kajak">Kajak</option>
                        </select>
                    </center>
                </td>
                <td width="500">
                    <b>Jaka jest Twoja ulubione ciastko?</b><br><br>
                    <input type="checkbox" name="ciastko" value="k"> BEZA<br>
                    <input type="checkbox" name="ciastko" value="m"> SERNIK<br>
                    <input type="checkbox" name="ciastko" value="inna"> INNE<br><br>
                    <nobr>Jeśli zaznaczyłeś INNE to podaj swoje ciastko<br>wpisz ciastko poniżej. Maks: 100 znaków</nobr><br><br>
                    <input name="inna" type="text" size="25" maxlength="100">
                </td>
            </tr>
            <tr height="200">
                <td>
                    <b>Czy umiesz programować?</b><br><br>
                    <input type="radio" name="pyt3" value="tak"> Tak<br>
                    <input type="radio" name="pyt3" value="nie"> Nie<br>
                    <input type="radio" name="pyt3" value="nie wiem"> Nie wiem<br><br>
                    <b>W polu poniżej wpisz opinię na temat pogody:</b><br>
                    <textarea cols="50" rows="4" name="opinia"></textarea>
                </td>
                <td>
                    <b>Podaj czas:</b><br>
                    <input type="time" name="czas"><br><br>
                    <b>Podaj datę:</b><br>
                    <input type="date" name="data"><br><br>
                    <b>Wybierz kolor:</b><br>
                    <input type="color" name="kolor"><br><br>
                </td>
                <td>
                    <b>Jaka jest wilgotność:</b><br>
                    <input type="range" name="wilgotnosc" min="0" max="100" step="1"><br><br>
                    <b>Proszę czekać...</b><br>
                    <progress value="50" max="100"></progress>
                </td>
            </tr>
            <tr height="100">
                <td>
                    <button type="button" onclick="alert('A kuku')">Przycisk niespodzianka</button>
                </td>
                <td>
                    <input type="reset" value="Reset">
                </td>
                <td>
                    <input type="submit" value="Wyślij formularz">
                </td>
            </tr>
        </table>
    </form>
    <p><a href="indexhtml.html">Powrót do strony głównej</a></p>
</body>
</html>
