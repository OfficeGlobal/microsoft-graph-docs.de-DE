---
title: Verwenden von ORDER-Hinweisen in Planner
description: '`)'
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 22596f7e9fea5954fc9b6fceb8dae117cf762cb5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525983"
---
# <a name="using-order-hints-in-planner"></a>Verwenden von ORDER-Hinweisen in Planner

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Objekte in Planner identifizieren ihre Sortierreihenfolge anhand von ORDER-Hinweisen. Die Werte von ORDER-Hinweisen sind Zeichenfolgen. Die Clients können die Zeichenfolgen basierend auf dem Ordnungswert von darin enthaltenen Zeichen sortieren, um die Reihenfolge von Elementen zu identifizieren. Die Zeichen werden ab dem Anfang der Zeichenfolge verglichen, bis ein Unterschied in den Ordnungswerten der Zeichen gefunden wird oder bis eine Zeichenfolge endet. In diesem Fall wird die kürzere Zeichenfolge vor der längeren sortiert. Die Werte können beliebige Zeichen zwischen den Ordnungszahlen 32 (Leerzeichen) und 126 enthalten (`~`).

Als Beispiel würde ein Element mit dem ORDER-Hinweis `a` (Ordnungswert 97) vor einem anderen Element mit dem ORDER-Hinweis `z` (Ordnungswert 122) platziert werden. Ein Element mit dem ORDER-Hinweis `abc` (Ordnungswerte 97, 98, 99) würde vor einem anderen Element mit dem ORDER-Hinweis `abd` (Ordnungswerte 97, 98, 100) platziert werden. Ein Element mit dem ORDER-Hinweis `a` würde vor einem anderen Element mit dem ORDER-Hinweis `ab` platziert, da alle vorhandenen Zeichen identisch sind und `a` kürzer ist.

Die Werte für alle ORDER-Hinweise werden vom Dienst berechnet. Der Client kann die Reihenfolge von Elementen ändern, indem der ORDER-Hinweis für das Element angegeben wird, das zwischen zwei Elementen verschoben wurde, indem der ORDER-Hinweis auf den folgenden Wert festgelegt wird: `<previous order hint> <next order hint>!`, wobei `<previous order hint>` durch den ORDER-Hinweis des Elements ersetzt werden muss, das sich vor der neuen gewünschten Position befindet, und `<next order hint>` durch den ORDER-Hinweis des Elements ersetzt werden muss, das sich nach der neuen gewünschten Position befindet. Es gibt ein Leerzeichen zwischen den Werten dieser ORDER-Hinweise, und `!` wird an den gesamten Wert angehängt. Wenn eines der Elemente nicht vorhanden ist, sollte stattdessen eine leere Zeichenfolge verwendet werden. Dieser Wert kann auch aus vorherigen Berechnungen zusammengestellt werden, und kann im Client verwendet werden, um Elemente genau wie vom Dienst zurückgegebene ORDER-Hinweise zu sortieren. Nachdem der Client diese Werte an eine Aktualisierung gesendet hat, berechnet der Dienst einen kurzen Wert, der an der gewünschten Position sortiert wird.

> **Hinweis:** In den folgenden Beispielen werden die tatsächliche Reihenfolge Hint Werte in einfache Anführungszeichen umgeben (`'`) aus Gründen der Übersichtlichkeit jedoch diese sind nicht Teil der Daten und müssen nicht mit dem Dienst gesendet werden.
 
Sehen Sie sich als Beispiel die folgende Liste sortierter ORDER-Hinweise an:

1. Element 1 (ORDER-Hinweis: `'5637'`)
2. Element 2 (ORDER-Hinweis: `'adhg'`)

Durch Platzieren eines Elements 3 vor Element 1, anschließendes Platzieren von Element 4 zwischen Element 1 und Element 2 und anschließendes Platzieren von Element 5 nach Element 2 würden die folgenden ORDER-Hinweise auf dem Client erstellt. 

1. Element 3 (ORDER-Hinweis: `' 5637!'`)
2. Element 1 (ORDER-Hinweis: `'5637'`)
3. Element 4 (ORDER-Hinweis: `'5637 adhg!'`)
4. Element 2 (ORDER-Hinweis: `'adhg'`)
5. Element 5 (ORDER-Hinweis: `'adhg !'`)

Durch Verschieben von Element 1 an das Ende der Liste würde Folgendes generiert:

1. Element 3 (ORDER-Hinweis: `' 5637!'`)
2. Element 4 (ORDER-Hinweis: `'5637 adhg!'`)
3. Element 2 (ORDER-Hinweis: `'adhg'`)
4. Element 5 (ORDER-Hinweis: `'adhg !'`)
5. Element 1 (ORDER-Hinweis: `'adhg ! !'`)

Durch Verschieben von Element 5 zwischen Element 3 und Element 4 würde schließlich Folgendes generiert:

1. Element 3 (ORDER-Hinweis: `' 5637!'`)
2. Element 5 (ORDER-Hinweis: `' 5637! 5637 adhg!!'`)
3. Element 4 (ORDER-Hinweis: `'5637 adhg!'`)
4. Element 2 (ORDER-Hinweis: `'adhg'`)
5. Element 1 (ORDER-Hinweis: `'adhg ! !'`)

Wenn diese Änderungen auf Reihenfolge Hint Werte an den Dienst in Patch Anfragen gesendet werden, wird der Dienst geeignete Werte berechnen, die die Reihenfolge für die direkte Verwendung durch den Client beibehalten. Der Client kann die direkte If Werte erhalten die `Prefer: return=representation` Einstellung Kopfzeile wird angegeben, der `PATCH` Anforderungen. Die Werte für die oben genannten Fall sehen in etwa wie folgt aus (die tatsächlichen Werte können anders lauten). 

1. Element 3 (ORDER-Hinweis: `'432b'`)
2. Element 5 (ORDER-Hinweis: `'6F"#'`)
3. Element 4 (ORDER-Hinweis: `'7A$6'`)
4. Element 2 (ORDER-Hinweis: `'adhg'`)
5. Element 1 (ORDER-Hinweis: `'de5%'`)

ORDER-Hinweise können für das Erstellen des ersten Elements in der Liste als ` !` angegeben werden, da in diesem Fall weder ein vorheriges noch ein nächstes Element vorhanden ist, dies ist jedoch nicht erforderlich, da der Dienst Werte für alle ORDER-Hinweise für Elemente automatisch generiert, wenn diese während der Erstellung des Elements nicht angegeben werden. Im folgenden Beispiel werden die ORDER-Hinweise veranschaulicht, die verwendet werden sollten, wenn Element in einer zuvor leeren Liste platziert werden. Fügen Sie das erste Element hinzu:

1. Element 1 (ORDER-Hinweis: `' !'`)

Fügen Sie das zweite Elemente am Anfang hinzu:

1. Element 2 (ORDER-Hinweis: `'  !!'`)
2. Element 1 (ORDER-Hinweis: `' !'`)

Fügen Sie das dritte Element am Ende hinzu:

1. Element 2 (ORDER-Hinweis: `'  !!'`)
2. Element 1 (ORDER-Hinweis: `' !'`)
3. Element 3 (ORDER-Hinweis: `' ! !'`)







<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/planner-order-hint-format.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
