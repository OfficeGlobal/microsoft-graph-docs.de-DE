---
title: Erstellen von programControl
description: Zugriff auf in Azure AD Bewertungen Feature, Erstellen eines neuen ProgramControl-Objekts.  Dadurch werden eine Access-Überprüfung an ein Programm verknüpft.
localization_priority: Normal
ms.openlocfilehash: 89e31994ea91dba68e2f4563c64eeab53dd4db93
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511114"
---
# <a name="create-programcontrol"></a>Erstellen von programControl

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Erstellen Sie ein neues [ProgramControl](../resources/programcontrol.md) -Objekt in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature.  Dadurch werden eine Access-Überprüfung an ein Programm verknüpft.

Bevor Sie diese Anforderung machen, muss der Aufrufer zuvor verfügen

 - [erstellt ein Programm](program-create.md) oder [eine Anwendung abgerufen](program-list.md), damit den Wert der `programId` zum Einschließen in die Anforderung
 - [erstellt eine Überprüfung Access](accessreview-create.md) oder [eine Access-Überprüfung abgerufen](accessreview-get.md), damit den Wert der `controlId` zum Einschließen in die Anforderung und
 - [die Liste der Typen von Steuerelementen Programm abgerufen](programcontroltype-list.md), damit den Wert der `controlTypeId` in der Anforderung enthalten.


## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)     | `ProgramControl.ReadWrite.All`.  Der Benutzer angemeldet muss auch in einer Directory-Rolle sein, die diese zum Erstellen einer ProgramControl zulässt. |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
|Anwendung                            | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a>Anforderungsheader
| Name         | Typ        | Beschreibung |
|:-------------|:------------|:------------|
| Authorization | string | Bearertoken Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [ProgramControl](../resources/programcontrol.md) -Objekts.

In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie ein Programmsteuerelement erstellen.

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
| `programId`              |`String`                | Die ProgramId des Programms wird dieses Steuerelement eines Teils werden sollte.                             |
| `controlId`              |`String`                | Die ControlId des Steuerelements, insbesondere die eine Access-ID überprüfen.                                                |
| `controlTypeId`          |`String`                | Die ProgramControlType identifiziert den Typ des programmfreigabesteuerung – beispielsweise ein Steuerelement verknüpfen mit Gast Access überprüft. |

## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201, Created` Antwortcode und eines [ProgramControl](../resources/programcontrol.md) -Objekts in der Antworttext.


## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [ProgramControl](../resources/programcontrol.md) -Objekts.

<!-- {
  "blockType": "request",
  "name": "create_programControl_from_programControls"
}-->
```http
POST https://graph.microsoft.com/beta/programControls
Content-type: application/json

{
    "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
}
```

##### <a name="response"></a>Antwort
>**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "63b2302c-7e62-43b7-aefb-063ba5bdb853",
  "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
  "displayName": "test",
  "status": "Active",
  "createdDateTime": "2018-05-18T20:26:05.2976279Z"
}
```

## <a name="see-also"></a>Siehe auch

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Liste programControlTypes](../api/programcontroltype-list.md) | [ProgramControlType](../resources/programcontroltype.md) -Auflistung| Programm Steuerelement Listentypen. |


<!--
{
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
