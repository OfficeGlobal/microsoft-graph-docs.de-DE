---
title: Erwähnen Ressourcentyp
description: Stellt eine Benachrichtigung an eine Person basierend auf e-Mail-Adresse der Person.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 4ab60fafe00f14f69d79e482d0616576c73d1092
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858429"
---
# <a name="mention-resource-type"></a>Erwähnen Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine Benachrichtigung an eine Person basierend auf e-Mail-Adresse der Person. Die Benachrichtigung wird auch als @ erwähnungen.

Die [Nachricht](../resources/message.md) Ressource unterstützt **erwähnen**. Sie umfasst eine **MentionsPreview** -Eigenschaft, die angibt, ob der angemeldeten Benutzer in dieser Nachrichteninstanz genannt wird. Darüber hinaus Navigationseigenschaft **erwähnt** , das die erste Details der Vermerk oder Löschen der Vermerk in dieser Instanz unterstützt.

Beim Erstellen einer Nachricht kann eine app in der gleichen Vermerk erstellen `POST` Anforderung durch, einschließlich der Angabe in der **erwähnungen** -Eigenschaft. Verwenden einer `GET` fordern Sie mit der `$filter` Abfragezeichenfolgen-Parameter eine app kann Zurückgeben aller Nachrichten im Postfach des angemeldeten Benutzers, in denen den Benutzer erwähnt. Eine `GET` fordern Sie mit der `$expand` Abfrage Parameter können die app alle Vorkommnisse in eine bestimmte Nachricht zu erweitern.

Dieser Mechanismus, lassen eine app festlegen und Abrufen erwähnungen in Nachrichten ermöglicht lightweight-Benachrichtigungen, in dem der Benutzer die Erwähnung, in dem vorhandenen Kontext (beispielsweise Verfassen eines Nachrichtentexts) verbleiben kann während der app wird die zugrunde liegende **erwähnt** -Eigenschaft . Erwähnten Personen können auf einfache Weise ermitteln, ob die und, in denen sie über erwähnt sind `GET` fordert mit der `$filter` oder `$expand` Parameter Abfragen.  

In der Outlook-Mailclient, wenn ein Benutzer beispielsweise `@` beim Verfassen einer Nachricht, lässt Outlook den Benutzer aktivieren, oder geben Sie einen Namen für die Durchführung der @ Erwähnung. Outlook wird die Eigenschaft **erwähnt** , bevor er erstellt und die Nachricht oder Ereignis sendet. Outlook verwendet auch `GET` Vorgänge mit `$filter` und `$expand` warnen der Benutzer zum Aufgaben oder Diskussionen, wodurch eine schnellere Antwort ermöglicht, um die angemeldeten Benutzer nach Nachrichten suchen, in denen den Benutzer erwähnt,.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mention"
}-->

```json
{
  "application": "string",
  "clientReference": "string",
  "createdBy": {"@odata.type": "microsoft.graph.emailAddress"},
  "createdDateTime": "DateTimeOffset",
  "deepLink": "string",
  "id": "string (identifier)",
  "mentioned": {"@odata.type": "microsoft.graph.emailAddress"},
  "mentionText": "string",
  "serverCreatedDateTime": "DateTimeOffset"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Anwendung | Zeichenfolge | Der Name der Anwendung, in dem die Erwähnung erstellt wird. Optional. Wird nicht verwendet und nicht mehr als Null für **Nachricht**übernommen. |
|clientReference | Zeichenfolge | Ein eindeutiger Bezeichner, der ein übergeordnetes Element der Ressourceninstanz darstellt. Optional. Wird nicht verwendet und nicht mehr als Null für **Nachricht**übernommen. |
|createdBy  | [emailAddress](../resources/emailaddress.md) | Die e-Mail-Informationen des Benutzers, der die Erwähnung vorgenommen. |
|createdDateTime  |DateTimeOffset |Das Datum und die Uhrzeit, die auf dem Client die Erwähnung erstellt wird. |
|deepLink | Zeichenfolge | Tiefe Weblink zu den Kontext des Hinweises auf die Instanz der Ressource. Optional. Wird nicht verwendet und nicht mehr als Null für **Nachricht**übernommen. |
|id | Zeichenfolge| Der eindeutige Bezeichner des Vermerk in einer Ressourceninstanz einer.|
|erwähnten | [emailAddress](../resources/emailaddress.md) | Die e-Mail-Informationen der weiter oben erwähnt Person. Erforderlich. |
|mentionText | Zeichenfolge | Optional. Wird nicht verwendet und nicht mehr als Null für **Nachricht**übernommen. Wenn die erwähnungen in einer Nachricht erhalten möchten, finden Sie stattdessen die **BodyPreview** -Eigenschaft der Nachricht. |
|serverCreatedDateTime | DateTimeOffset | Das Datum und die Uhrzeit, die die Erwähnung auf dem Server erstellt wird. Optional. Wird nicht verwendet und nicht mehr als Null für **Nachricht**übernommen. |

## <a name="relationships"></a>Beziehungen
Keine


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[POST-Anforderung](../api/user-sendmail.md#request-2) und senden | Keine | Erstellen und Senden von erwähnungen im Rahmen einer neuen Nachricht.|
|[POST-Anforderung](../api/user-post-messages.md#request-2) an einen neuen Entwurf | [Nachricht](../resources/message.md) , die ein oder mehrere **erwähnen** Objekte enthält. | Erstellen ein Entwurfs oder eine neue Nachricht und fügen Sie ein oder mehrere **erwähnen** Objekte.|
|[Abrufen](../api/user-list-messages.md#request-2) von Nachrichten Erwähnung me | [message](../resources/message.md)-Sammlung | Rufen Sie alle Nachrichten im Postfach des angemeldeten Benutzers, die ein **erwähnen** dieses Benutzers enthalten.|
|Eine Meldung [erhalten](../api/message-get.md#request-2) und seine erwähnungen | [message](../resources/message.md)-Sammlung | Möchten Sie eine Meldung erhalten, und erweitern Sie die Details der einzelnen **erwähnen** in der Nachricht.|
|[Löschen](../api/message-delete.md#request-2) der Vermerk | Keine |Löscht die angegebene Erwähnung in der angegebenen Nachricht im Postfach des angemeldeten Benutzers. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
