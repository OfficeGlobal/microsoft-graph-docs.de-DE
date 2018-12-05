---
title: Erstellen der Anwendung
description: Zugriff auf in Azure AD Bewertungen Feature, erstellen Sie ein neues Programmobjekt.
ms.openlocfilehash: 1ac3fa1f0b555fc92449adf0e57217d0a7d50375
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064152"
---
# <a name="create-program"></a>Erstellen der Anwendung

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Erstellen Sie ein neues [Programm](../resources/program.md) -Objekt in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature.
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)     | `ProgramControl.ReadWrite.All`.  Der Benutzer angemeldet muss auch in einer Directory-Rolle sein, die diese zum Erstellen eines Programms zulässt. |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
|Anwendung                            | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a>Anforderungsheader
| Name         | Typ        | Beschreibung |
|:-------------|:------------|:------------|
| Authorization | string | Bearer \{token\}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines Objekts [Programm](../resources/program.md) .

In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie ein Programm erstellen.

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  Der Name des Programms.                   |
| `description`               |`String`                              |  Die Beschreibung des Programms.           |


## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201, Created` Antwortobjekt und [Programmdateien](../resources/program.md) im Antworttext.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Programm](../resources/program.md) -Objekts.

<!-- {
  "blockType": "request",
  "name": "create_program_from_programs"
}-->
```http
POST https://graph.microsoft.com/beta/programs
Content-type: application/json

{
    "displayName": "testprogram3",
    "description": "test description"
}
```

##### <a name="response"></a>Antwort
>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3",
    "description": "test description"
}
```

## <a name="see-also"></a>Siehe auch

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Programme auflisten](program-list.md) | [Programm](../resources/program.md) -Auflistung|  Rufen Sie eine Auflistung aller Programme.|
|[Liste ProgramControls eines Programms](program-listcontrols.md) |     [ProgramControl](../resources/programcontrol.md) -Auflistung|    Rufen Sie eine Auflistung der Steuerelemente eines Programms.|
|[Update-Programm](program-update.md) |  [Programm](../resources/program.md)| Aktualisieren eines Programms.|
|[Erstellen von programControl](programcontrol-create.md) |        [programControl](../resources/programcontrol.md)    |   Fügen Sie ein Programm ein ProgramControl hinzu.|

<!-- {
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->