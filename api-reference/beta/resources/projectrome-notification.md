---
title: Benachrichtigung Ressourcentyp
description: 'Stellt eine Benachrichtigung, die von einem app-Server veröffentlicht wird, die einen angegebenen Benutzer abzielt. Die Benachrichtigung in Microsoft Graph gespeichert ist und auf anderes Gerät Endpunkte Besitz des Benutzers verteilt ist. '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: af130c9806511b0afbdaedb602790c7c40d3ca2e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509259"
---
# <a name="notification-resource-type"></a>Benachrichtigung Ressourcentyp
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine Benachrichtigung, die von einem app-Server veröffentlicht wird, die einen angegebenen Benutzer abzielt. Die Benachrichtigung in Microsoft Graph gespeichert ist und auf anderes Gerät Endpunkte Besitz des Benutzers verteilt ist. 

Eine Benachrichtigung kann es sich um eine visuelle Benachrichtigung Nutzlast sein, die vom Betriebssystem, einschließlich Windows, iOS und Android-Plattformen interpretiert werden können. Es kann auch sein, Datennutzlast, die den zugestellt und behandelt wurde von app-Clients, die bestimmen, klicken Sie dann die entsprechende Benutzer erleben auf jedem Gerät – in der Regel eine visuelle Benachrichtigung Benutzeroberfläche, die den Inhalt in der ursprünglichen Datennutzlast entspricht, die generiert wird lokal. 

Wenn ein Benutzer auf eine visuelle Benachrichtigung fungiert, kann der app-Client mithilfe der clientseitigen Project ROM SDK klicken Sie dann verwenden, um den Status der entsprechende Benachrichtigung, beispielsweise durch eine Benachrichtigung kennzeichnen, wie Sie ausgeblendete feed in Microsoft Graph - aktualisieren. Das Update wird dann an alle Endpunkte andere app-Client verteilt werden, und die Clients die Änderung entsprechend behandelt, beispielsweise durch Schließen die Benachrichtigung, um zu verhindern, dass den Benutzer redundanten Informationen einsehen können. App-Clients können dieselbe Ressource Benachrichtigung zugreifen, zu einem späteren Zeitpunkt, bevor sie abläuft (auch nach es als geschlossen markiert ist), als Benachrichtigungsverlauf, über die [Project-ROM-SDK](https://github.com/Microsoft/project-rome). 

## <a name="methods"></a>Methoden
|Methode | Rückgabetyp | Beschreibung|
|:------|:------------|:-----------|
|[Benachrichtigung erstellen](../api/projectrome-notification-post.md) | Benachrichtigung |Erstellen Sie und senden Sie eine Benachrichtigung. |

## <a name="properties"></a>Eigenschaften
|Name | Typ | Beschreibung|
|:----|:-----|:-----------|
| targetHostName | String | Stellt den Hostnamen der app auf die der aufrufende Dienst möchte die Benachrichtigung für den angegebenen Benutzer buchen. |
| appNotificationId | String | Die eindeutige Id, die von der app-Server eine Benachrichtigung, die verwendet wird, zu identifizieren, und statten Sie eine einzelne Benachrichtigung festgelegt. |
| expirationDateTime | DateTimeOffset | Legt eine Ablaufzeit UTC auf eine Benachrichtigung Benutzer - Zeit wird oben, die Benachrichtigung wird aus der Microsoft Graph Benachrichtigung feed Store vollständig entfernt und ist nicht mehr Teil der Benachrichtigungsverlauf. Max-Wert beträgt 30 Tage. |
| payload | Edm.ComplexType JSON-Objekt | Dies ist der Dateninhalt des Benachrichtigung Rohdaten oder visual-Benutzer, die Identitätsdaten durch den Empfang dieser Benachrichtigung app-Client und übermittelt werden. |
| payload.rawContent | String | Der Inhalt der Benachrichtigung über eine unformatierte User-Benachrichtigung, die an übermittelt und vom Empfang dieser Benachrichtigung app-Client verwendet werden. Mindestens eine der Payload.RawContent und Payload.VisualContent muss für eine Benachrichtigung POST-Anforderung gültig sein. |
| Payload.Visual | Edm.ComplexType JSON-Objekt | Der visuelle Inhalt einer Benachrichtigung visuelle Benutzer, die von der Benachrichtigung-Plattform auf jedes mobile Plattform genutzt werden und für die Benutzer gerendert. Mindestens eine der Inhalte und VisualContent muss für eine Benachrichtigung POST-Anforderung gültig sein. |
| Payload.Visual.Title | String | Der Titel einer Benachrichtigung visuelle Benutzer. Titel oder Textkörper benötigen. |
| Payload.Visual.Body | String | Der Text einer Benachrichtigung visuelle Benutzer. Titel oder Textkörper benötigen. |
| displayTimeToLive | Int | Legt fest, wie lange (in Sekunden) ist, wird dieser Benachrichtigungsinhalt in jede Plattform Benachrichtigung Viewer bleiben. Angenommen, wenn die Benachrichtigung an ein Windows-Gerät übermittelt werden, ist der Wert dieser Eigenschaft an ToastNotification.ExpirationTime, übergeben die bestimmt, wie lange die Toast-Benachrichtigung des Benutzers Windows-Aktion Center bleibt. |
| Priorität | EnumType | Gibt die Priorität einer Benachrichtigung unformatierte User. Visual Benachrichtigungen werden standardmäßig mit hoher Priorität gesendet. Gültige Werte sind hohen und niedrigen. |
| GroupName | String | Der Name der Gruppe, zu der diese Benachrichtigung gehört. Es wird vom Entwickler zum Gruppieren von Benachrichtigungen festgelegt. |
| targetPolicy | Edm.ComplexType JSON-Objekt | Richtlinie Zielobjekt behandelt Notification Delivery Richtlinie auf zwei verschiedenen Ebenen - Endpunkttypen (Windows, iOS und Android), die verwendet werden soll, und bestimmten Endpunkten (identifiziert durch Abonnement-Ids), die verwendet werden soll. |
| targetPolicy.platformTypes | Edm.ComplexType Auflistung (EnumType) | Verwenden Sie zum Filtern der Benachrichtigung Verteilung einer bestimmten Plattform oder Plattformen. Standardmäßig werden alle Push Endpunkttypen (iOS, Windows und Android) aktiviert. |

## <a name="relationships"></a>Beziehungen
Keine.

## <a name="json-representation"></a>JSON-Darstellung
Im folgenden finden eine JSON-Darstellung der Ressource, wenn Sie eine direkte visuelle Benachrichtigung veröffentlichen, die an das Zielbetriebssystem übermittelt werden.

```json
{   
  "targetHostName": "String",
  "appNotificationId": "String",
  "expirationDateTime": "DateTimeOffset",
  "payload":  
  {
    "visualContent": 
    {
      "title": "String",
      "body": "String"
    },
  },
  "displayTimeToLive": "Int",
  "priority": "Enum",
  "groupName": "String",
  "targetPolicy":
  {
    "platformTypes": [ 
      "Enum"
    ]
  }
}
```

Im folgenden finden eine JSON-Darstellung der Ressource, wenn Sie eine Benachrichtigung über eine unformatierte Daten veröffentlichen, die an die app-Clients übermittelt werden.
```json
{   
  "targetHostName": "String",
  "appNotificationId": "String",
  "expirationDateTime": "DateTimeOffset",
  "payload":  
  {
    "rawContent": "String"
  },
  "displayTimeToLive": "Int",
  "priority": "Enum",
  "groupName": "String",
  "targetPolicy":
  {
    "platformTypes": [ 
      "Enum"
    ]
  }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/projectrome-notification.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
