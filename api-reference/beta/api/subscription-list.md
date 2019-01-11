---
title: Liste von Abonnements
description: " finden Sie die Szenarien unter Weitere Informationen."
localization_priority: Normal
ms.openlocfilehash: 1b751b8632d82626e2ba87bf00a054b2be4f25f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876986"
---
# <a name="list-subscriptions"></a>Liste von Abonnements

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Abrufen einer Liste der Webhook-Abonnements. Der Inhalt der Antwort hängt von den Kontext, in dem die app anruft. finden Sie die Szenarien unter Weitere Informationen.

## <a name="permissions"></a>Berechtigungen

Diese API unterstützt die folgenden berechtigungsbereiche. Weitere, einschließlich auswählen von Berechtigungen finden Sie unter [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp  | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)  |
|:---------------- |:-------------------------------------------- |
| [Delegiert](/graph/auth-v2-user) (Arbeit oder Schule Konto) | Erforderliche Berechtigung zum [Erstellen von Abonnement](subscription-post-subscriptions.md) oder Subscription.Read.All (siehe unten). |
| [Delegiert](/graph/auth-v2-user) (Persönliches Microsoft-Konto) | Erforderliche Berechtigung zum [Erstellen von Abonnement](subscription-post-subscriptions.md) oder Subscription.Read.All (siehe unten). |
| [Anwendung](/graph/auth-v2-service) | Erforderliche Berechtigung zum [Abonnement zu erstellen](subscription-post-subscriptions.md). |

Antwort Ergebnisse basieren auf dem Kontext der aufrufenden app. Es folgt eine Zusammenfassung der gängigen Szenarien:

### <a name="basic-scenarios"></a>Grundlegende Szenarios

In den meisten Fällen eine Anwendung Abonnements abrufen möchte, die ursprünglich für den aktuell angemeldeten Benutzer oder für alle Benutzer in das Verzeichnis (Arbeit/Schule Konten) erstellt. Diese Szenarien ist keine speziellen Berechtigungen als die die app ursprünglich verwendet, um dessen Abonnements erstellen erforderlich.

| Kontext der aufrufenden app | Antwort enthält |
|:-----|:---------------- |
| App ist im Namen des angemeldeten Benutzers (Delegierte Berechtigung) aufrufen. <br/>- und -<br/>App besitzt die ursprüngliche Berechtigung erforderlich, um [das Abonnement zu erstellen](subscription-post-subscriptions.md).<br/><br/>Hinweis: Dies gilt für persönliche Microsoft-Konten und Arbeit/Schule Konten. | Abonnements durch **diese app** für den angemeldeten Benutzer nur erstellt. |
| App ist im Namen selbst (Anwendung die Berechtigung) aufrufen.<br/>- und -<br/>App besitzt die ursprüngliche Berechtigung erforderlich, um [das Abonnement zu erstellen](subscription-post-subscriptions.md).<br/><br/>Hinweis: Dies gilt Arbeit/nur Konten Schule.| Abonnements, die **diese** App für sich selbst oder für jeden Benutzer in das Verzeichnis erstellt werden.|

### <a name="advanced-scenarios"></a>Erweiterte Szenarien

In einigen Fällen eine app von anderen apps erstellt Abonnements abrufen möchte. Beispielsweise möchte ein Benutzer alle Abonnements, die von einer beliebigen app in ihrem Auftrag erstellt. Oder ein Administrator alle Abonnements aus allen apps in ihrem Verzeichnis finden Sie unter möchten.
Für solche Szenarien ist eine delegierte Berechtigung Subscription.Read.All erforderlich.

| Kontext der aufrufenden app | Antwort enthält |
|:-----|:---------------- |
| App ist im Namen des angemeldeten Benutzers (Delegierte Berechtigung) aufrufen. *Der Benutzer ist ein nicht-Administrator*. <br/>- und -<br/>App verfügt über die Berechtigung Subscription.Read.All<br/><br/>Hinweis: Dies gilt für persönliche Microsoft-Konten und Arbeit/Schule Konten. | Abonnements, die von **einer beliebigen app** nur für den angemeldeten Benutzer erstellt. |
| App ist im Namen des angemeldeten Benutzers (Delegierte Berechtigung) aufrufen. *Der Benutzer ist ein Administrator*.<br/>- und -<br/>App verfügt über die Berechtigung Subscription.Read.All<br/><br/>Hinweis: Dies gilt Arbeit/nur Konten Schule. | Abonnements, die von **einer beliebigen app** für **alle Benutzer** im Verzeichnis erstellt.|

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt nicht die [OData-Abfrage-Parameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , mit denen die Antwort anpassen.

## <a name="request-headers"></a>Anforderungsheader

| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext

Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Liste von Objekten im Antworttext [Abonnement](../resources/subscription.md) .

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Die hier gezeigte Antwort der Kürze halber werden möglicherweise abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 586

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions",
  "value": [
    {
      "id": "0fc0d6db-0073-42e5-a186-853da75fb308",
      "resource": "Users",
      "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
      "changeType": "updated,deleted",
      "clientState": null,
      "notificationUrl": "https://webhookappexample.azurewebsites.net/api/notifications",
      "expirationDateTime": "2018-03-12T05:00:00Z",
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

Wenn eine Anforderung mehrere Seiten mit Daten zurückgegeben, die Antwort enthält eine `@odata.nextLink` Eigenschaft zur einfacheren Verwaltung der Ergebnisse.  Finden Sie weitere Informationen finden Sie unter [Microsoft Graph Paging von Daten in Ihrer app](/graph/paging).
