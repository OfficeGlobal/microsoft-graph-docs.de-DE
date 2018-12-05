---
title: Bezeichner in Aufgaben
description: 'Bezeichner für Objekte in Aufgaben sind Zeichenfolgenwerte Dienst generiert. . Die Werte sind 28 Zeichen lang sein und Groß-/Kleinschreibung beachtet. Wenn als übergeben, wird der Dienst eine einfache Format Validierung des Bezeichners, vorgehen, wenn Format Überprüfung fehlschlägt, die Anrufer ungültige Anforderung (400) Fehler, der angibt, des Problems beantwortet werden. Diese Fehlermeldung gibt einen Fehler in der aufrufenden Anwendung, wie an:'
ms.openlocfilehash: d57ca282de87c2bce42b37d0be6d08dbe128c522
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065797"
---
# <a name="identifiers-in-tasks"></a>Bezeichner in Aufgaben

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Bezeichner für Objekte in Aufgaben sind Zeichenfolgenwerte Dienst generiert. . Die Werte sind 28 Zeichen lang sein und Groß-/Kleinschreibung beachtet. Wenn als übergeben, wird der Dienst eine einfache Format Validierung des Bezeichners, vorgehen, wenn Format Überprüfung fehlschlägt, die Anrufer ungültige Anforderung (400) Fehler, der angibt, des Problems beantwortet werden. Diese Fehlermeldung gibt einen Fehler in der aufrufenden Anwendung, wie an:

- Die aufrufende Anwendung hat den Bezeichner als Zeichenfolge verarbeitet, bei der nicht zwischen Groß- und Kleinschreibung unterschieden wird. Bei Bezeichnern in Aufgaben wird zwischen Groß- und Kleinschreibung unterschieden.
- Die aufrufende Anwendung hat den Bezeichner abgeschnitten. Bezeichner in Aufgaben sind 28 Zeichen lang.
- Die aufrufende Anwendung hat versucht, einen Bezeichnerwert für ein Objekt in Aufgaben zu generieren. Vom Client generierte Bezeichner werden nicht akzeptiert. Alle Bezeichner werden vom Dienst bei Erstellung der Objekte generiert.

Diese Überprüfung ist **kein Sicherheitsfeature**. Sie dient lediglich dazu, Anwendungen über allgemeine Probleme im Zusammenhang mit Bezeichnern zu informieren, die bei der Entwicklung der Anwendung auftreten und andernfalls schwer zu erkennen sind.