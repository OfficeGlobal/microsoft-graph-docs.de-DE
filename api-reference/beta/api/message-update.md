---
title: Nachricht aktualisieren
description: Mit dieser API können Sie die Eigenschaften eines Nachrichtenobjekts aktualisieren.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5a42e9d6a10e79a4ae801cca464c912dc6fade7b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515685"
---
# <a name="update-message"></a>Nachricht aktualisieren

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Mit dieser API können Sie die Eigenschaften eines Nachrichtenobjekts aktualisieren.
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Mail.ReadWrite    |
|Delegiert (persönliches Microsoft-Konto) | Mail.ReadWrite    |
|Anwendung | Mail.ReadWrite |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |
| Content-Type | string  | Die Art der Daten im Textkörper einer Entität. Erforderlich. |
## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben. Die folgenden Eigenschaften können aktualisiert werden.

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|bccRecipients|Empfänger|Die Bcc:-Empfänger der Nachricht. |
|body|ItemBody|Der Text der Nachricht. Kann nur aktualisiert werden, wenn IsDraft = True.|
|categories|String collection|Die Kategorien, die mit der Nachricht verknüpft sind.|
|ccRecipients|Empfänger-Sammlung|Die Cc:-Empfänger der Nachricht. |
|from|Empfänger|Der Postfachbesitzer und Absender der Nachricht. Muss dem tatsächlich verwendeten Postfach entsprechen. |
|importance|Zeichenfolge|Wichtigkeit der Nachricht Mögliche Werte: `Low`, `Normal`, `High`.|
|inferenceClassification | String | Die Klassifizierung der Nachricht für den Benutzer, basierend auf der abgeleiteten Relevanz oder Wichtigkeit oder auf einer expliziten Außerkraftsetzung. Mögliche Werte sind: `focused` oder `other`. |
|internetMessageId |String |Die Nachrichten-ID im von [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) angegebenen Format. Kann nur aktualisiert werden, wenn IsDraft = True.|
|isDeliveryReceiptRequested|Boolean|Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.|
|isRead|Boolean|Gibt an, ob die Nachricht gelesen wurde.|
|isReadReceiptRequested|Boolean|Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)-Sammlung| Die Sammlung der für die Nachricht definierten mehrwertigen erweiterten Eigenschaften. Nullwerte zulassend.|
|replyTo|Empfänger-Sammlung|Die E-Mail-Adressen, die beim Antworten verwendet werden sollen. Kann nur aktualisiert werden, wenn isDraft = True.|
|sender|Empfänger|Das Konto, das tatsächlich verwendet wird, um die Nachricht zu generieren. Kann beim Senden einer Nachricht aus einem [freigegebenen Postfach](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes) oder beim Senden einer Nachricht als[Stellvertretung](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926) aktualisiert werden. Der Wert muss auf jeden Fall dem tatsächlich verwendeten Postfach entsprechen.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)-Sammlung| Die Sammlung der für die Nachricht definierten einwertigen erweiterten Eigenschaften. Nullwerte zulassend.|
|subject|String|Der Betreff der Nachricht. Kann nur aktualisiert werden, wenn IsDraft = True.|
|toRecipients|Empfänger-Sammlung|Die An:-Empfänger der Nachricht. |

Da die **message**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, erlaubt der `PATCH`-Vorgang das Hinzufügen, Aktualisieren oder Löschen eigener App-spezifischer Daten in den benutzerdefinierten Eigenschaften von Erweiterungen in vorhandenen **message**-Instanzen.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [message](../resources/message.md)-Objekt im Antworttext zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "inferenceClassification": "other"
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "inferenceClassification": "other"
}
```

## <a name="see-also"></a>Weitere Artikel

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)](/graph/extensibility-open-users)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
