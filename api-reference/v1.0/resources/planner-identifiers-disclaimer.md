---
title: Bezeichner in Planner
description: 'Bezeichner in Planner-Objekte sind Zeichenfolgenwerte Dienst generiert. Die Werte sind 28 Zeichen lang sein und Groß-/Kleinschreibung beachtet. Wenn als übergeben, wird der Dienst eine einfache Format Validierung des Bezeichners, vorgehen, wenn Format Überprüfung fehlschlägt, die Anrufer ungültige Anforderung (400) Fehler, der angibt, des Problems beantwortet werden. Diese Fehlermeldung gibt einen Fehler in der aufrufenden Anwendung, wie an:'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 75c284d576ed6f03691828309fab7ed899c1c066
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951858"
---
# <a name="identifiers-in-planner"></a>Bezeichner in Planner

Bezeichner in Planner-Objekte sind Zeichenfolgenwerte Dienst generiert. Die Werte sind 28 Zeichen lang sein und Groß-/Kleinschreibung beachtet. Wenn als übergeben, wird der Dienst eine einfache Format Validierung des Bezeichners, vorgehen, wenn Format Überprüfung fehlschlägt, die Anrufer ungültige Anforderung (400) Fehler, der angibt, des Problems beantwortet werden. Diese Fehlermeldung gibt einen Fehler in der aufrufenden Anwendung, wie an:

- Die aufrufende Anwendung hat den Bezeichner als Zeichenfolge verarbeitet, bei der nicht zwischen Groß- und Kleinschreibung unterschieden wird. Bei Bezeichnern in Aufgaben wird zwischen Groß- und Kleinschreibung unterschieden.
- Die aufrufende Anwendung hat den Bezeichner abgeschnitten. Bezeichner in Aufgaben sind 28 Zeichen lang.
- Die aufrufende Anwendung hat versucht, einen Bezeichnerwert für ein Objekt in Aufgaben zu generieren. Vom Client generierte Bezeichner werden nicht akzeptiert. Alle Bezeichner werden vom Dienst bei Erstellung der Objekte generiert.

Diese Überprüfung ist **kein Sicherheitsfeature**. Sie dient lediglich dazu, Anwendungen über allgemeine Probleme im Zusammenhang mit Bezeichnern zu informieren, die bei der Entwicklung der Anwendung auftreten und andernfalls schwer zu erkennen sind.
