---
title: Klonen Sie ein team
description: Erstellen Sie eine Kopie eines Teams. Dieser Vorgang wird außerdem eine Kopie der entsprechenden Gruppe erstellt.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: afd0c4d1f264989a349a300201ea4a1c528fd681
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912498"
---
# <a name="clone-a-team"></a>Klonen Sie ein team



Erstellen Sie eine Kopie eines [Team](../resources/team.md). Dieser Vorgang wird außerdem eine Kopie der entsprechenden [Gruppe](../resources/group.md)erstellt.
Sie können die Teile des Teams Klonen angeben:

- **apps** – Microsoft-Teams, Kopien apps, die im Team installiert sind. 
- **Kanäle** – kopiert die Struktur DDE-Kanal (jedoch nicht die Nachrichten im Kanal).
- **Elemente des Objekts** – kopiert die Mitglieder und Besitzer der Gruppe.
- **Einstellungen** – kopiert alle Einstellungen im Team, zusammen mit den wichtigsten gruppeneinstellungen.
- **Registerkarten** – kopiert die Registerkarten in den Kanälen.

Wenn Registerkarten geklont werden, in einen nicht konfigurierten Status zugeführt werden – auf der Registerleiste in Microsoft-Teams angezeigt werden, und beim ersten Öffnen, werden über den Konfigurationsbildschirm wechseln. (Wenn die Person, die beim Öffnen der Registerkarte keinen Berechtigung zum Konfigurieren von apps, sehen sie eine Meldung angezeigt, dass die Registerkarte nicht konfiguriert wurde.)

Klonen ist ein zeitintensiver Vorgang.
Nachdem der POST-Klon zurückgegeben wird, müssen Sie den [Vorgang](../resources/teamsasyncoperation.md) abrufen, um festzustellen, ob es sich um "ausführen" oder "erfolgreich" oder "Fehler" ist. Sie sollten zu berechnen fortfahren, bis der Status nicht "aktiv" ist. Die empfohlene Verzögerung zwischen ruft beträgt 5 Sekunden.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)     | Group.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung                            | Group.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a>Anforderungsheader
| Header       | Wert |
|:---------------|:--------|
| Authorization  | Bearer {token}. Erforderlich.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Anforderungstext

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Klassifikation|Zeichenfolge (optional)|Beschreibt eine Klassifizierung für die Gruppe (z. B. niedrig, Mittel oder hoch geschäftliche Relevanz). Wenn Klassifizierung nicht angegeben ist, wird die Klassifizierung aus der ursprünglichen Team-Gruppe kopiert werden.|
|description|Zeichenfolge (optional)|Eine optionale Beschreibung für die Gruppe. Wenn diese Eigenschaft nicht angegeben ist, wird es leer sein.|
|displayName|Zeichenfolge|Der Anzeigename der Gruppe. Diese Eigenschaft ist beim Erstellen einer Gruppe erforderlich und kann bei Updates nicht deaktiviert werden. Unterstützt $Filter und $orderby.|
|mailNickname|Zeichenfolge|Der e-Mail-Alias für die Gruppe, die in der Organisation eindeutig. Diese Eigenschaft muss angegeben werden, wenn eine Gruppe erstellt wird. Unterstützt $filter. Wenn diese Eigenschaft nicht angegeben ist, wird er von der DisplayName berechnet. Bekanntes Problem: Diese Eigenschaft wird zurzeit ignoriert.|
|partsToClone| [clonableTeamParts](../resources/clonableteamparts.md) |Eine durch Trennzeichen getrennte Liste der Teile zum Klonen. Rechtliche Webparts sind "apps, Registerkarten, Einstellungen, Kanäle, Mitglieder".|
|visibility|[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)| Gibt die Sichtbarkeit der Gruppe. Mögliche Werte sind: **Private**, **Public**. Wenn die Sichtbarkeit nicht angegeben wird, werden die Sichtbarkeit aus der ursprünglichen Team-Gruppe kopiert. Wenn das Team geklont wird ist ein **EducationClass** Team der Sichtbarkeit-Parameter wird ignoriert und Sichtbarkeit für die neue Gruppe wird auf HiddenMembership festgelegt werden.|

## <a name="response"></a>Antwort

Wenn erfolgreich, mit dieser Methode zurückgegeben wird eine `202 Accepted` Antwortcode mit einem Standortprofil: Verweisen auf die Ressource [Vorgang](../resources/teamsasyncoperation.md) Kopfzeile.
Wenn der Vorgang abgeschlossen ist, wird die Vorgang Ressource die Id des erstellten Teams informieren.

## <a name="example"></a>Beispiel
#### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
POST /teams/{id}/clone
Content-Type: application/json

{  
     "displayName": "Library Assist",
     "description": "Self help community for library",
     "mailNickname": "libassist",
     "partsToClone": "apps,tabs,settings,channels,members",
     "visibility": "public"
}
```

#### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
