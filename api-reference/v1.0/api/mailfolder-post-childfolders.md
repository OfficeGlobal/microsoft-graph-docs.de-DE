---
title: MailFolder erstellen
description: Mit dieser API können Sie neue untergeordnete Objekte des Typs „mailfolder“ erstellen.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: bf078e34f216dde5a3daf3bcf0cecd27517e7da7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941443"
---
# <a name="create-mailfolder"></a>MailFolder erstellen

Mit dieser API können Sie neue untergeordnete Objekte des Typs „mailfolder“ erstellen.

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
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

Geben Sie in der Abfrage-URL als eine Ordner-ID oder den Ordnernamen einer bekannten des übergeordneten Ordners. Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).

## <a name="request-headers"></a>Anforderungsheader

| Header | Wert |
|:-------|:------|
| Authorization | `Bearer {token}`. Erforderlich.  |
| Content-Type | `application/json`. Erforderlich.  |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an. **DisplayName** ist die nur schreibbare Eigenschaft für ein [MailFolder](../resources/mailfolder.md) -Objekt.

| Parameter | Typ | Beschreibung |
|:----------|:-----|:------------|
|displayName|Zeichenfolge|Der Anzeigename für den neuen Ordner.|

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode und eine [MailFolder](../resources/mailfolder.md) Ressource in den Antworttext.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.

> **Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
