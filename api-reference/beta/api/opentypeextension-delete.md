---
title: Offene Erweiterung löschen
description: 'Mit dieser API können Sie offene Erweiterungen (Objekte des Typs openTypeExtension aus der jeweils angegebenen Ressourceninstanz löschen. '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 6882cd1502221642e10c7e0fe7cbca5d43e543a5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512528"
---
# <a name="delete-open-extension"></a>Offene Erweiterung löschen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Mit dieser API können Sie offene Erweiterungen (Objekte des Typs [openTypeExtension](../resources/opentypeextension.md) aus der jeweils angegebenen Ressourceninstanz löschen. 

## <a name="permissions"></a>Berechtigungen

Je nach der Ressource, die Sie die Erweiterung von löschen möchten, und die Berechtigung Typ (delegierte oder-Anwendung) angefordert, die Berechtigung, die in der folgenden Tabelle angegebenen mit den geringsten ist erforderlich, um diese API aufzurufen. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).

| Unterstützte Ressource | Delegiert (Geschäfts-, Schul- oder Unikonto) | Delegiert (persönliches Microsoft-Konto) | Anwendung |
|:-----|:-----|:-----|:-----|
| [Gerät](../resources/device.md) | Directory.AccessAsUser.All | Nicht unterstützt | Device.ReadWrite.All |
| [event](../resources/event.md) | Calendars.ReadWrite | Calendars.ReadWrite | Calendars.ReadWrite |
| [group](../resources/group.md) | Group.ReadWrite.All | Nicht unterstützt | Group.ReadWrite.All |
| [group event](../resources/event.md) | Group.ReadWrite.All | Nicht unterstützt | Nicht unterstützt |
| [group post](../resources/post.md) | Group.ReadWrite.All | Nicht unterstützt | Group.ReadWrite.All |
| [message](../resources/message.md) | Mail.ReadWrite | Mail.ReadWrite | Mail.ReadWrite | 
| [organization](../resources/organization.md) | Directory.AccessAsUser.All | Nicht unterstützt | Nicht unterstützt |
| [personal contact](../resources/contact.md) | Contacts.ReadWrite | Contacts.ReadWrite | Contacts.ReadWrite |
| [user](../resources/user.md) | User.ReadWrite.All | User.ReadWrite | User.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

In der Anforderung geben Sie die Ressourceninstanz an, spezifizieren in der Navigationseigenschaft **extensions** dieser Instanz die Erweiterung und wenden anschließend den Befehl `DELETE` auf diese Erweiterungsinstanz an.

<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{Id}/extensions/{extensionId}
DELETE /devices/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/extensions/{extensionId}
DELETE /groups/{id}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
DELETE /organization/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/extensions/{extensionId}
```

>**Hinweis:** Die obige Syntax zeigt mehrere häufig verwendete Möglichkeiten zum Identifizieren einer Ressourceninstanz, um eine Erweiterung daraus zu löschen. Alle anderen Syntaxen, mit denen Sie diese Ressourceninstanzen identifizieren können, unterstützen das Löschen offener Erweiterungen daraus in einer ähnlichen Weise.

## <a name="path-parameters"></a>Pfadparameter
|**Parameter**|**Typ**|**Beschreibung**|
|:-----|:-----|:-----|
|id|string|Ein eindeutiger Bezeichner für eine Instanz in der entsprechenden Sammlung. Erforderlich.|
|extensionId|string|Dies kann ein Erweiterungsname sein. Der Erweiterungsname ist ein eindeutiger Textbezeichner der Erweiterung oder ein vollqualifizierter Name, der den Erweiterungstyp und den eindeutigen Textbezeichner verkettet. Der vollqualifizierte Name wird beim Erstellen der Erweiterung in der `id`-Eigenschaft zurückgegeben. Erforderlich.|

## <a name="request-headers"></a>Anforderungsheader
| Name       | Wert |
|:---------------|:----------|
| Authorization | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Das erste Beispiel referenziert eine Erweiterung über ihren Namen und löscht die Erweiterung in der angegebenen Nachricht.
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

Das zweite Beispiel löscht eine Erweiterung in dem angegebenen Gruppenereignis.

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVlN17IsAAA=')/extensions('Com.Contoso.Referral')
```

 

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/opentypeextension-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
