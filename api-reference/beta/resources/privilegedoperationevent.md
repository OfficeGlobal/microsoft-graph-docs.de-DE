---
title: Ressourcentyp privilegedOperationEvent
description: Stellt ein Überwachungsereignis, die für die Rolle Vorgänge von privilegierten Identity Management generiert wird, wie ein Administrator privilegierte Rollen verwaltet, ein Benutzer seine Rolle aktiviert und ein Benutzer seine Rolle deaktiviert.
localization_priority: Normal
ms.openlocfilehash: 2ad8f7e5db956dfbb2fa0d74f441b01f2b5d68aa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525591"
---
# <a name="privilegedoperationevent-resource-type"></a>Ressourcentyp privilegedOperationEvent

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt ein Überwachungsereignis, die für die Rolle Vorgänge von privilegierten Identity Management generiert wird, wie ein Administrator privilegierte Rollen verwaltet, ein Benutzer seine Rolle aktiviert und ein Benutzer seine Rolle deaktiviert.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Liste privilegedOperationEvent](../api/privilegedoperationevent-list.md) | [PrivilegedOperationEvent](privilegedoperationevent.md) -Auflistung. |Rufen Sie die Auflistung von PrivilegedOperationEvent-Objekten.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|zusätzliche Informationen|string|Ausführliche lesbare human Informationen für das Ereignis.|
|creationDateTime|dateTimeOffset|Gibt den Zeitpunkt der Erstellung des Ereignisses.|
|expirationDateTime|dateTimeOffset|Dies wird nur verwendet, wenn die RequestType "Activate", und es gibt die Ablaufzeit für die Aktivierung der Rolle an.|
|id|string|Der eindeutige Bezeichner für PrivilegedOperationEvent. Schreibgeschützt.|
|referenceKey|string|Ticket-Nummer während der Aktivierung der Rolle Vorfall-Anforderung. Der Wert wird nur dargestellt, wenn die Ticket-Nummer während der Aktivierung der Rolle bereitgestellt wird.|
|referenceSystem|string|Vorfall/Anforderung mitgearbeitet während der Aktivierung Tole bereitgestellt. Der Wert wird dargestellt, nur, wenn das System Ticket während der Aktivierung der Rolle bereitgestellt wird.|
|RequestType|string|Der Typ der Anforderung Operation. Der RequestType-Wert sein kann: ```Assign``` (rollenzuweisung) ```Activate``` (Role-Aktivierung), ```Unassign``` (rollenzuweisung entfernen), ```Deactivate``` (Rolle Deaktivierung) ```ScanAlersNow``` (scan Sicherheitshinweise), ```DismissAlert``` (Schließen Sicherheitshinweis), ```FixAlertItem``` (beheben ein Wertpapiers Warnen Problem), ```AccessReview_Review``` (Überprüfen Sie eine Access überprüfen), ```AccessReview_Create``` (Erstellen einer Access überprüfen), ```AccessReview_Update``` (update Überprüfen einer Access), und ```AccessReview_Delete``` (Löschen einer Access überprüfen).|
|requestorId|string|Die Benutzer-Id der anfordernden Person, die den Vorgang initiiert.|
|requestorName|string|Der Name der anfordernden Person, die den Vorgang initiiert.|
|roleId|string|Die Id des der Rolle, die den Vorgang zugeordnet ist.|
|roleName|string|Der Name der Rolle.|
|tenantId|string|Die Id des Mandanten (Unternehmen).|
|userId|string|Die Id des Benutzers, der den Vorgang zugeordnet ist.|
|userMail|string|E-Mail des Benutzers.|
|userName|string|Der Anzeigename des Benutzers.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedOperationEvent"
}-->

```json
{
  "additionalInformation": "string",
  "creationDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "requestType": "string",
  "requestorId": "string",
  "requestorName": "string",
  "roleId": "string",
  "roleName": "string",
  "tenantId": "string",
  "userId": "string",
  "userMail": "string",
  "userName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedOperationEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedoperationevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
