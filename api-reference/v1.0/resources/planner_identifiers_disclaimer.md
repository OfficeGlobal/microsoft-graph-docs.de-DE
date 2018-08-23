# <a name="identifiers-in-planner"></a>Bezeichner in Planner

Bezeichner für Objekte in Planner sind vom Dienst generierte Zeichenfolgenwerte. Die Werte sind 28 Zeichen lang, Groß- und Kleinschreibung wird berücksichtigt. Wenn diese übergeben werden, führt der Dienst eine einfache Formatüberprüfung des Bezeichners durch. Wenn diese fehlschlägt, erhalten die aufrufenden Funktionen eine Fehlermeldung vom Typ "Ungültige Anforderung (400) mit einer Angabe dieses Problems. Diese Fehlermeldung weist auf einen Fehler in der aufrufenden Anwendung hin, z. B.:

- Die aufrufende Anwendung hat den Bezeichner als Zeichenfolge verarbeitet, bei der nicht zwischen Groß- und Kleinschreibung unterschieden wird. Bei Bezeichnern in Aufgaben wird zwischen Groß- und Kleinschreibung unterschieden.
- Die aufrufende Anwendung hat den Bezeichner abgeschnitten. Bezeichner in Aufgaben sind 28 Zeichen lang.
- Die aufrufende Anwendung hat versucht, einen Bezeichnerwert für ein Objekt in Aufgaben zu generieren. Vom Client generierte Bezeichner werden nicht akzeptiert. Alle Bezeichner werden vom Dienst bei Erstellung der Objekte generiert.

Diese Überprüfung ist **kein Sicherheitsfeature**. Sie dient lediglich dazu, Anwendungen über allgemeine Probleme im Zusammenhang mit Bezeichnern zu informieren, die bei der Entwicklung der Anwendung auftreten und andernfalls schwer zu erkennen sind.