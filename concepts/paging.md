---
title: 'Paging der Microsoft Graph-Daten in Ihrer App '
description: 'odata.nextLink-Eigenschaft in der Antwort, die eine URL zur nächsten Seite mit Ergebnissen enthält. '
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 6a19d1873057f5a6f6ea1749a6941389b9be8eb5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830660"
---
# <a name="paging-microsoft-graph-data-in-your-app"></a>Paging der Microsoft Graph-Daten in Ihrer App 

Einige Abfragen in Microsoft Graph geben mehrere Seiten von Daten zurück, entweder aufgrund von serverseitigem Paging oder aufgrund der Verwendung des `$top`-Abfrageparameters, um die Seitengröße in einer Anforderung gezielt zu begrenzen. Wenn ein Resultset mehrere Seiten umfasst, gibt Microsoft Graph eine `@odata.nextLink`-Eigenschaft in der Antwort, die eine URL zu der nächsten Seite mit Ergebnissen enthält. 

Die folgende URL fordert beispielsweise alle Benutzer in einer Organisation mit einer Seitengröße von 5 an, die mit dem `$top`-Abfrageparameter angegeben wird:

```html
https://graph.microsoft.com/v1.0/users?$top=5
```

Wenn das Ergebnis mehr als fünf Benutzer enthält, gibt Microsoft Graph eine `@odata:nextLink`-Eigenschaft ähnlich der folgenden zusammen mit der ersten Seite von Benutzern zurück.

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27"
```

Sie können die nächste Seite mit Ergebnissen abrufen, indem Sie den URL-Wert der `@odata:nextLink`-Eigenschaft an Microsoft Graph senden. 

```html
https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27
```

Microsoft Graph gibt weiterhin einen Verweis auf die nächste Seite von Daten in der `@odata:nextLink`-Eigenschaft mit jeder Antwort zurück, bis alle Seiten des Ergebnisses gelesen wurden.

>**Wichtig:** Sie sollten die gesamte URL in die `@odata:nextLink`-Eigenschaft in Ihrer Anforderung für die nächste Seite mit Ergebnissen einschließen. In Abhängigkeit von der API, für die die Abfrage ausgeführt wird, enthält der `@odata:nextLink`-URL-Wert entweder den Abfrageparameter `$skiptoken` oder `$skip`. Die URL enthält auch alle anderen Abfrageparameter, die in der ursprünglichen Anforderung vorhanden sind. Versuchen Sie nicht, den Wert von `$skiptoken` oder `$skip` zu extrahieren und in einer anderen Anforderung zu verwenden. 

Das Paging-Verhalten variiert in den verschiedenen Microsoft Graph-APIs. Berücksichtigen Sie beim Arbeiten mit ausgelagerten Daten die folgenden Punkte:

- Unterschiedliche APIs weisen möglicherweise unterschiedliche Standard- und Maximalgrößen für Seiten auf.
- Unterschiedliche APIs verhalten sich möglicherweise unterschiedlich, wenn Sie eine Seitengröße (über den `$top`-Abfrageparameter) angeben, der die maximale Seitengröße für diese API überschreitet. Je nach API wird die angeforderte Seitengröße möglicherweise ignoriert oder standardmäßig auf die maximale Seitengröße für diese API festgelegt, oder Microsoft Graph gibt einen Fehler zurück. 
- Nicht alle Ressourcen oder Beziehungen unterstützen Paging. Abfragen von [directoryRoles](/graph/api/resources/directoryrole?view=graph-rest-1.0) unterstützen beispielsweise kein Paging. Dies umfasst das Lesen von Rollenobjekten und Rollenmitgliedern.
