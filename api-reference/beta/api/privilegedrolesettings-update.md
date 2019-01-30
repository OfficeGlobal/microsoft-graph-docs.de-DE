---
title: PrivilegedRoleSettings aktualisieren
description: Aktualisieren Sie die rolleneinstellungen für die bestimmten Rolle-Einstellung. Ein PrivilegedRoleSettings-Objekt wird zurückgegeben.
localization_priority: Normal
ms.openlocfilehash: 09464c878c76ed557f30d0eac21e0572fae05062
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641120"
---
# <a name="update-privilegedrolesettings"></a>PrivilegedRoleSettings aktualisieren

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aktualisieren Sie die rolleneinstellungen für die bestimmten Rolle-Einstellung. Ein [PrivilegedRoleSettings](../resources/privilegedrolesettings.md) -Objekt wird zurückgegeben.
## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

>**Hinweis:** Die anfordernde Person muss eines der folgenden Rollen haben: berechtigten Rolle Administrators, globaler Administrator, Sicherheitsadministrator oder Sicherheit Leser. 

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Application | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a>Anforderungsheader
| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [PrivilegedRoleSettings](../resources/privilegedrolesettings.md) -Objekts.

Die folgende Tabelle enthält die Eigenschaften, die Sie angeben können, wenn Sie eine Einstellung für die Rolle aktualisieren.

|Eigenschaft|Typ|Beschreibung|
|:---------------|:--------|:----------|
|elevationDuration|duration|Die Dauer, wenn die Rolle aktiviert ist. Erforderlich. |
|id|string|Der eindeutige Bezeichner für die rolleneinstellungen. Schreibgeschützt. Erforderlich. |
|isMfaOnElevationConfigurable|Boolescher Wert|**true,** Wenn MfaOnElevation konfigurierbar ist. **false,** Wenn MfaOnElevation nicht konfigurierbar ist. Erforderlich. |
|lastGlobalAdmin|Boolean|Nur für internen Gebrauch.|
|maxElavationDuration|duration|Maximale Speicherdauer für die aktivierte Rolle. Erforderlich. |
|mfaOnElevation|Boolean|**true,** Wenn mehrstufiger Authentifizierung das erforderlich ist, um die Rolle zu aktivieren. **false,** Wenn mehrstufiger Authentifizierung das nicht erforderlich ist, um die Rolle zu aktivieren. Erforderlich. |
|minElevationDuration|duration|Minimale Dauer für die aktivierte Rolle. Erforderlich. |
|notificationToUserOnElevation|Boolean|**true,** Wenn für den Endbenutzer Benachrichtigung senden, wenn die Rolle aktiviert ist. **false,** Wenn keine Benachrichtigung senden, wenn die Rolle aktiviert ist. Erforderlich. |
|ticketingInfoOnElevation|Boolean|**true,** Wenn die Informationen zur erforderlichen wann ist die Rolle zu aktivieren. **false,** Wenn die Informationen zur nicht erforderlich bei ist die Rolle zu aktivieren. Erforderlich. |
|approvalOnElevation|Boolean|**true,** Wenn die Genehmigung erforderlich wann ist die Rolle zu aktivieren. **false,** Wenn die Genehmigung ist nicht erforderlich bei die Rolle zu aktivieren. Erforderlich. |
|approverIds|Array|Liste der Genehmigung-IDs, wenn die Genehmigung für die Aktivierung erforderlich ist.|

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.

Beachten Sie, dass der Mandant muss auf den PIM registriert werden. Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "put_privilegedrolesettings"
}-->
```http
PUT https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
Content-type: application/json

{
    "id": "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    "elevationDuration": "PT8H",
    "notificationToUserOnElevation": false,
    "ticketingInfoOnElevation": true,
    "mfaOnElevation": false,
    "maxElavationDuration": "PT0S",
    "minElevationDuration": "PT0S",
    "lastGlobalAdmin": false,
    "isMfaOnElevationConfigurable": true,
    "approvalOnElevation": false,
    "approverIds": ["e2b2a2fb-13d7-495c-adc9-941fe966793f", "22770e3f-b9b4-418e-9dea-d0e3d2f275dd"]
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrolesettings-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
