---
title: Typ der Benutzeridentität
description: 'Für die Azure AD zugreifen Reviews (engl.), diesen Typ eine Benutzeridentität Azure AD für Bearbeiter die Überprüfung einer Access darstellt.  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 80e8cc68d4fc2f642be6c748b762fe47c7489d59
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932280"
---
# <a name="useridentity-type"></a>Typ der Benutzeridentität

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Für die Azure AD, [Access überprüft](accessreviews-root.md)ist stellt dieses Typs eine Benutzeridentität Azure AD eines Bearbeiters eines Access-Überprüfung.  
Im Zusammenhang mit einer Azure AD-Überwachungsprotokoll stellt dies die Benutzerinformationen, die initiiert oder durch eine Aktivität Audit betroffen war.

Dieser Typ erbt von [Identität](identity.md) und verfügt über eine zusätzliche Eigenschaft, den Benutzerprinzipalnamen des Benutzers.

## <a name="methods"></a>Methoden

Keine.  Schließen Sie Objekte dieses Typs im Textkörper einer Anforderung beim [Erstellen einer AccessReview](../api/accessreview-create.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| `displayName` | `String` | Die Identität der Anzeigename. Beachten Sie, dass dies möglicherweise nicht immer verfügbar oder auf dem neuesten Stand.    |
| `id`          | `String` | Eindeutiger Bezeichner für die Identität.  |
| `ipAddress`| `String`| Gibt an, die Client-IP-Adresse von Benutzer, die Ausführung der Aktivität (nur Audit Log) verwendet wird.|
| `userPrincipalName`|`String` | Das UserPrincipalName-Attribut des Benutzers. |

## <a name="remarks"></a>Bemerkungen

Unter gewissen Umständen steht der eindeutige Bezeichner für den Akteur möglicherweise nicht zur Verfügung. In diesem Fall die wird die Eigenschaft **DisplayName** für die Identität zurückgegeben werden, aber die **Id**-Eigenschaft ist aus der Ressource nicht vorhanden.

## <a name="relationships"></a>Beziehungen

Keine.

## <a name="see-also"></a>Siehe auch

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von AccessReview Bearbeiter](../api/accessreview-listreviewers.md) |       [Benutzeridentität](useridentity.md) -Auflistung| Rufen Sie die Bearbeiter ein AccessReview. |
|[AccessReview Bearbeiter hinzufügen](../api/accessreview-addreviewer.md) |      Keine.   |   Fügen Sie einem Bearbeiter ein AccessReview hinzu. |
|[AccessReview Reviewer entfernen](../api/accessreview-removereviewer.md) | Keine.  |   Entfernen Sie einen Prüfer aus einer AccessReview. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung des Typs.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
"displayName", "thumbnails"
  ],
  "@odata.type": "microsoft.graph.userIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string",
 "userPrincipalName": "String"
}

```

<!-- {
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
