---
title: Ein Mitglied hinzufügen
description: Verwenden Sie diese API zum Hinzufügen eines Mitglieds (Benutzer oder Gruppe), um eine administrative Einheit.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f64ca4c00265903fa1b4ebc467f2d70274628078
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946826"
---
# <a name="add-a-member"></a>Ein Mitglied hinzufügen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Verwenden Sie diese API zum Hinzufügen eines Mitglieds (Benutzer oder Gruppe), um eine administrative Einheit.

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).


|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a>Anforderungsheader
| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [Benutzers](../resources/user.md), [Gruppe](../resources/group.md) oder [DirectoryObject](../resources/directoryobject.md) hinzugefügt werden soll.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.

```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
Geben Sie im Textkörper Anforderung eine JSON-Darstellung der die `id` des Objekts [Benutzer](../resources/user.md) oder eine [Gruppe](../resources/group.md) hinzufügen möchten.

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.
 
```http
HTTP/1.1 204 No Content
```
