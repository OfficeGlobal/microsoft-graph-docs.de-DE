---
title: Bezeichner in Planner
description: 'Bezeichner in Planner-Objekte sind Zeichenfolgenwerte Dienst generiert. Die Werte sind 28 Zeichen lang sein und Groß-/Kleinschreibung beachtet. Wenn als übergeben, wird der Dienst eine einfache Format Validierung des Bezeichners, vorgehen, wenn Format Überprüfung fehlschlägt, die Anrufer ungültige Anforderung (400) Fehler, der angibt, des Problems beantwortet werden. Diese Fehlermeldung gibt einen Fehler in der aufrufenden Anwendung, wie an:'
localization_priority: Normal
ms.openlocfilehash: 6efb1192de87082cae99fbcc058607a2239a618c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816590"
---
# <a name="identifiers-in-planner"></a>Bezeichner in Planner

Bezeichner in Planner-Objekte sind Zeichenfolgenwerte Dienst generiert. Die Werte sind 28 Zeichen lang sein und Groß-/Kleinschreibung beachtet. Wenn als übergeben, wird der Dienst eine einfache Format Validierung des Bezeichners, vorgehen, wenn Format Überprüfung fehlschlägt, die Anrufer ungültige Anforderung (400) Fehler, der angibt, des Problems beantwortet werden. Diese Fehlermeldung gibt einen Fehler in der aufrufenden Anwendung, wie an:

- Die aufrufende Anwendung hat den Bezeichner als Zeichenfolge verarbeitet, bei der nicht zwischen Groß- und Kleinschreibung unterschieden wird. Bei Bezeichnern in Aufgaben wird zwischen Groß- und Kleinschreibung unterschieden.
- Die aufrufende Anwendung hat den Bezeichner abgeschnitten. Bezeichner in Aufgaben sind 28 Zeichen lang.
- Die aufrufende Anwendung hat versucht, einen Bezeichnerwert für ein Objekt in Aufgaben zu generieren. Vom Client generierte Bezeichner werden nicht akzeptiert. Alle Bezeichner werden vom Dienst bei Erstellung der Objekte generiert.

Diese Überprüfung ist **kein Sicherheitsfeature**. Sie dient lediglich dazu, Anwendungen über allgemeine Probleme im Zusammenhang mit Bezeichnern zu informieren, die bei der Entwicklung der Anwendung auftreten und andernfalls schwer zu erkennen sind.
