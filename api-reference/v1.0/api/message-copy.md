---
title: 'message: copy'
description: Mit dieser API können Sie Nachrichten in Ordner kopieren.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 38ff866ac6464f53adc021fabb05ad3ad7d435c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854929"
---
# <a name="message-copy"></a>message: copy

Mit dieser API können Sie Nachrichten in Ordner kopieren.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten) |
|:----------------|:--------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Mail.ReadWrite    |
|Delegiert (persönliches Microsoft-Konto) | Mail.ReadWrite    |
|Anwendung | Mail.ReadWrite |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a>Anforderungsheader

| Kopfzeile | Wert |
|:-------|:------|
| Authorization | `Bearer {token}`. Erforderlich. |
| Content-Type | `application/json`. Erforderlich. |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

| Parameter | Typ | Beschreibung |
|:----------|:-----|:------------|
|destinationId|String|Die Ziel-Ordner-ID oder den Ordnernamen einer bekannten. Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).|

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode und eine [Nachricht](../resources/message.md) Ressource in den Antworttext.

## <a name="example"></a>Beispiel

Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.

##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

> **Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
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
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
