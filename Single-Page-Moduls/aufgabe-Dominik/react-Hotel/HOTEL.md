Unser Hotel ist etwas in die Jahre gekommen. So wird die Zimmerbelegung bisher noch auf Papier festgehalten, was in der heutigen Zeit nicht mehr sein muss. Wir wollen das nun ändern und entwickeln deshalb eine digitale Zimmerverwaltung!
1. Zuerst wollen wir uns anschauen, welche Daten für ein Zimmer nötig sind. Wir beginnen damit, die aktuelle Belegung darzustellen.
Ein Datensatz für ein Zimmer enthält die Raumnummer (roomNo), Details zum Gast (guest) und Anreise- und Abreise-Datum (checkIn & checkout):
{
    "roomNo": 208,
    "guest": {
        "firstName": "Melicent",
        "lastName": "Dragge"
    },
    "checkIn": "2022-04-10",
    "checkOut": "2022-04-11"
}
Diese Daten wollen wir in einer eigenständigen Komponente ausgeben. Als Name bietet sich "Room" an.
Wenn du die Komponente erstellst, nutze zuerst den Beispieldatensatz als Variable innerhalb der Komponente, wie in den ersten drei JSX-Aufgaben von gestern.
2. Da wir mehrere Zimmer haben, sollten wir diese natürlich alle anzeigen. Erstelle hierfür eine neue Komponente für die Übersicht und rendere dort drei Room-Komponenten. Dass die Daten zunächst gleich sind, ist für diesen Schritt egal.
3. Nun steuere die Daten für die drei Zimmer über Props. Übergebe hier ein ganzes Objekt für das Zimmer. So kannst du dieses später besser erweitern.
4. Da wir mehr als drei Zimmer haben, macht es Sinn, auf eine dynamische Generierung umzusteigen. Nutze hierfür map() und die vollständige Liste mit allen Datensätzen.
5. Die Zimmernummern sind noch nicht geordnet. Kannst du sie nach Zimmernummer aufsteigend sortieren und dann ausgeben? Beachte dabei, dass die ursprüngliche Liste nicht umgeschrieben werden soll. Die Sortierung muss innerhalb deines Codes passieren.
6. Die Datumsangaben checkIn und checkOut lassen sich bestimmt noch etwas schöner formatieren. Kannst du sie in das Format DD.MM.YY bringen?
rooms.json
 
[
    {
        "roomNo": 208,
        "guest": {
            "firstName": "Melicent",
            "lastName": "Dragge"
        },
        "checkIn": "2022-04-10",
        "checkOut": "2022-04-11"
    },
    {
        "roomNo": 201,
        "guest": {
            "firstName": "Aggy",
            "lastName": "Nussgen"
        },
        "checkIn": "2021-12-04",
        "checkOut": "2021-11-11"
    },
    {
        "roomNo": 4,
        "guest": {
            "firstName": "Pepita",
            "lastName": "Spight"
        },
        "checkIn": "2022-04-02",
        "checkOut": "2021-10-19"
    },
    {
        "roomNo": 280,
        "guest": {
            "firstName": "Brady",
            "lastName": "Massingham"
        },
        "checkIn": "2021-11-08",
        "checkOut": "2022-09-07"
    },
    {
        "roomNo": 239,
        "guest": {
            "firstName": "Gracia",
            "lastName": "Harness"
        },
        "checkIn": "2022-10-01",
        "checkOut": "2022-04-04"
    },
    {
        "roomNo": 89,
        "guest": {
            "firstName": "Pierrette",
            "lastName": "Bland"
        },
        "checkIn": "2022-01-25",
        "checkOut": "2022-08-14"
    },
    {
        "roomNo": 117,
        "guest": {
            "firstName": "Findley",
            "lastName": "Ohlsen"
        },
        "checkIn": "2022-09-21",
        "checkOut": "2022-03-24"
    },
    {
        "roomNo": 188,
        "guest": {
            "firstName": "Eadie",
            "lastName": "Kynman"
        },
        "checkIn": "2022-01-05",
        "checkOut": "2022-10-30"
    },
    {
        "roomNo": 46,
        "guest": {
            "firstName": "Rogers",
            "lastName": "Soff"
        },
        "checkIn": "2022-04-25",
        "checkOut": "2021-12-13"
    },
    {
        "roomNo": 271,
        "guest": {
            "firstName": "Theresa",
            "lastName": "Howchin"
        },
        "checkIn": "2021-10-22",
        "checkOut": "2022-06-04"
    },
    {
        "roomNo": 272,
        "guest": {
            "firstName": "Tanner",
            "lastName": "Keohane"
        },
        "checkIn": "2022-09-10",
        "checkOut": "2022-09-15"
    },
    {
        "roomNo": 168,
        "guest": {
            "firstName": "Roscoe",
            "lastName": "Cruce"
        },
        "checkIn": "2022-07-10",
        "checkOut": "2021-12-11"
    },
    {
        "roomNo": 285,
        "guest": {
            "firstName": "Ulick",
            "lastName": "Bickardike"
        },
        "checkIn": "2022-05-08",
        "checkOut": "2021-11-06"
    },
    {
        "roomNo": 214,
        "guest": {
            "firstName": "Baldwin",
            "lastName": "Haggish"
        },
        "checkIn": "2022-02-23",
        "checkOut": "2022-05-16"
    },
    {
        "roomNo": 14,
        "guest": {
            "firstName": "Wendy",
            "lastName": "Tedman"
        },
        "checkIn": "2022-04-14",
        "checkOut": "2022-04-09"
    },
    {
        "roomNo": 31,
        "guest": {
            "firstName": "Koralle",
            "lastName": "Kunkel"
        },
        "checkIn": "2022-05-11",
        "checkOut": "2021-10-11"
    },
    {
        "roomNo": 220,
        "guest": {
            "firstName": "Hamilton",
            "lastName": "Doget"
        },
        "checkIn": "2022-10-02",
        "checkOut": "2022-10-03"
    },
    {
        "roomNo": 196,
        "guest": {
            "firstName": "Scott",
            "lastName": "Scoggans"
        },
        "checkIn": "2022-07-14",
        "checkOut": "2022-07-15"
    },
    {
        "roomNo": 119,
        "guest": {
            "firstName": "Ulberto",
            "lastName": "Tindle"
        },
        "checkIn": "2021-11-02",
        "checkOut": "2022-02-09"
    },
    {
        "roomNo": 5,
        "guest": {
            "firstName": "Hilde",
            "lastName": "McAneny"
        },
        "checkIn": "2022-03-05",
        "checkOut": "2022-04-15"
    },
    {
        "roomNo": 232,
        "guest": {
            "firstName": "Jock",
            "lastName": "Chattell"
        },
        "checkIn": "2022-06-14",
        "checkOut": "2022-02-01"
    },
    {
        "roomNo": 273,
        "guest": {
            "firstName": "Lauri",
            "lastName": "di Rocca"
        },
        "checkIn": "2022-01-14",
        "checkOut": "2021-10-10"
    },
    {
        "roomNo": 161,
        "guest": {
            "firstName": "Samantha",
            "lastName": "McPaike"
        },
        "checkIn": "2022-01-04",
        "checkOut": "2022-02-03"
    },
    {
        "roomNo": 289,
        "guest": {
            "firstName": "Jolyn",
            "lastName": "Rizzotto"
        },
        "checkIn": "2022-09-25",
        "checkOut": "2022-02-19"
    },
    {
        "roomNo": 135,
        "guest": {
            "firstName": "Francoise",
            "lastName": "Simony"
        },
        "checkIn": "2022-03-29",
        "checkOut": "2022-06-12"
    },
    {
        "roomNo": 222,
        "guest": {
            "firstName": "Ed",
            "lastName": "Frankes"
        },
        "checkIn": "2022-06-18",
        "checkOut": "2022-04-11"
    },
    {
        "roomNo": 208,
        "guest": {
            "firstName": "Thor",
            "lastName": "Hubbocks"
        },
        "checkIn": "2022-08-10",
        "checkOut": "2022-03-09"
    },
    {
        "roomNo": 175,
        "guest": {
            "firstName": "Dahlia",
            "lastName": "Hastewell"
        },
        "checkIn": "2022-09-08",
        "checkOut": "2022-10-22"
    },
    {
        "roomNo": 52,
        "guest": {
            "firstName": "Iolande",
            "lastName": "Levane"
        },
        "checkIn": "2022-08-25",
        "checkOut": "2022-02-13"
    },
    {
        "roomNo": 87,
        "guest": {
            "firstName": "Jamaal",
            "lastName": "D'Alessandro"
        },
        "checkIn": "2021-11-12",
        "checkOut": "2021-11-21"
    },
    {
        "roomNo": 142,
        "guest": {
            "firstName": "Scot",
            "lastName": "Beinke"
        },
        "checkIn": "2022-09-15",
        "checkOut": "2022-03-18"
    },
    {
        "roomNo": 228,
        "guest": {
            "firstName": "Violetta",
            "lastName": "Camilletti"
        },
        "checkIn": "2022-08-01",
        "checkOut": "2022-03-08"
    },
    {
        "roomNo": 71,
        "guest": {
            "firstName": "Otho",
            "lastName": "Treherne"
        },
        "checkIn": "2022-03-12",
        "checkOut": "2021-11-13"
    },
    {
        "roomNo": 156,
        "guest": {
            "firstName": "Farr",
            "lastName": "Gabbatiss"
        },
        "checkIn": "2022-08-08",
        "checkOut": "2022-10-11"
    },
    {
        "roomNo": 56,
        "guest": {
            "firstName": "Cleo",
            "lastName": "Bromby"
        },
        "checkIn": "2022-01-18",
        "checkOut": "2022-06-20"
    },
    {
        "roomNo": 281,
        "guest": {
            "firstName": "Eunice",
            "lastName": "Kiendl"
        },
        "checkIn": "2021-10-02",
        "checkOut": "2022-01-26"
    },
    {
        "roomNo": 76,
        "guest": {
            "firstName": "Nina",
            "lastName": "Gritten"
        },
        "checkIn": "2022-01-23",
        "checkOut": "2022-01-11"
    },
    {
        "roomNo": 75,
        "guest": {
            "firstName": "Dannie",
            "lastName": "Bastian"
        },
        "checkIn": "2022-10-07",
        "checkOut": "2021-11-13"
    },
    {
        "roomNo": 189,
        "guest": {
            "firstName": "Lorianne",
            "lastName": "Craigmile"
        },
        "checkIn": "2022-01-24",
        "checkOut": "2022-06-19"
    },
    {
        "roomNo": 205,
        "guest": {
            "firstName": "Glenn",
            "lastName": "Steven"
        },
        "checkIn": "2022-03-31",
        "checkOut": "2022-01-15"
    },
    {
        "roomNo": 245,
        "guest": {
            "firstName": "Darda",
            "lastName": "Grinval"
        },
        "checkIn": "2022-09-12",
        "checkOut": "2022-06-24"
    },
    {
        "roomNo": 224,
        "guest": {
            "firstName": "Giacopo",
            "lastName": "Tattershall"
        },
        "checkIn": "2022-04-07",
        "checkOut": "2022-04-17"
    },
    {
        "roomNo": 282,
        "guest": {
            "firstName": "Valerye",
            "lastName": "Bre...

            1. Füge einen Button "Check In / Check Out" in der Komponente Room.js ein und setze einen OnClick-Handler darauf. Gib das Event in der Konsole aus.


Für unser Hotel soll ein Anfrageformular erstellt werden. In das Formular soll ein Gast den Vor- und Nachnamen, sowie ein Anreise- und Abreisedatum angeben.
1. Erstelle ein passendes Formular in einer neuen Komponente. Kümmere dich zuerst nur um das Formular an sich (in JSX). Achte auf eindeutige Namen für die Inputs.
2. Baue die Inputs nun zu Controlled Components um: Richte einen oder mehrere States ein, gib sie in den Inputs aus und mache sie veränderbar über Eingaben.
3. Ein Formular, das man nicht absenden kann, bringt uns nicht viel. Daher richte eine Möglichkeit zum Absenden ein. Beim Absenden sollen alle Werte des Formulars in einem Objekt in der Konsole ausgegeben werden.
4. Nach dem Absenden wollen wir noch etwas aufräumen: Setze das Formular zurück.