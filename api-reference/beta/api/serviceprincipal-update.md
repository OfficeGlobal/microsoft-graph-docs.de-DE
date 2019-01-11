---
title: Serviceprincipal aktualisieren
description: Aktualisieren Sie die Eigenschaften des Serviceprincipal-Objekts.
localization_priority: Normal
ms.openlocfilehash: a8d4eebe64ac9c0c658ae9c43e2e92045be67424
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813027"
---
# <a name="update-serviceprincipal"></a>Serviceprincipal aktualisieren

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Aktualisieren Sie die Eigenschaften des Serviceprincipal-Objekts.
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Application.ReadWrite.OwnedBy Application.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|accountEnabled|Boolean|                **true,** Wenn das Dienstkonto für den Prinzipal aktiviert ist. anderenfalls **false**.            |
|appDisplayName|String|Der Anzeigename, der von der zugeordneten Anwendung verfügbar gemacht werden.|
|appId|Zeichenfolge|Der eindeutige Bezeichner für die zugewiesene Anwendung (dessen **AppId** -Eigenschaft).|
|appRoleAssignmentRequired|Boolean|Gibt an, ob ein **AppRoleAssignment** für einen Benutzer oder Gruppe erforderlich ist, bevor Azure AD einen Benutzer oder eine Zugriffstoken an die Anwendung ausstellt.                            **Notes**: erfordert Version 1.5 oder neuere, nicht NULL-Werte zulässt.            |
|appRoles|appRole|Die Rollen der Anwendung von der zugeordneten Anwendung verfügbar gemacht werden. Weitere Informationen finden Sie in der Definition der **AppRoles** -Eigenschaft in der Anwendung Entität **Notes**: erfordert Version 1.5 oder neuere, nicht NULL-Werte zulässt.            |
|displayName|String|Der Anzeigename für den Dienstprinzipal.|
|errorUrl|String|            |
|Homepage|String|Die URL zur Homepage der zugehörigen Anwendung.|
|keyCredentials|keyCredential|Die Auflistung von wichtigen Anmeldeinformationen, die dem Prinzipal Dienst zugeordnet sind.                            **Hinweis:** Lässt keine Nullwerte zu.            |
|logoutUrl|String| Gibt die URL, die von Microsoft Autorisierungsdienst Abmelden ein Benutzer mit der [Vorderseite-Kanal](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [Back-Kanal](https://openid.net/specs/openid-connect-backchannel-1_0.html) oder SAML Abmeldung Protokolle verwendet werden soll. |
|oauth2Permissions|oAuth2Permission|Die OAuth 2.0-Berechtigungen von der zugeordneten Anwendung verfügbar gemacht werden. Weitere Informationen finden Sie in der Definition der **oauth2Permissions** -Eigenschaft in der Anwendung Entität.                            **Notes**: erfordert Version 1.5 oder neuere, nicht NULL-Werte zulässt.            |
|passwordCredentials|passwordCredential|Die Auflistung von Anmeldeinformationen den Dienstprinzipal zugeordnet.                            **Hinweis:** Lässt keine Nullwerte zu.            |
|preferredTokenSigningKeyThumbprint|String|Nur für interne Zwecke vorbehalten. Schreiben oder verlassen sich andernfalls auf diese Eigenschaft nicht. Kann in zukünftigen Versionen entfernt werden.                            **Notes**: erfordert Version 1.5 oder höher.            |
|publisherName|String|Der Anzeigename des Mandanten in dem verbundenen Anwendung angegeben wird.|
|replyUrls|String|Die URLs, dass Benutzertoken, um für die Anmeldung mit der zugeordneten Anwendung oder die Umleitung URIs, dass OAuth 2.0 Autorisierungscodes gesendet werden und Zugriffstoken werden für die zugewiesene Anwendung an.                            **Hinweis:** Lässt keine Nullwerte zu.            |
|samlMetadataUrl|String|            |
|servicePrincipalNames|String|Die URIs, mit denen die zugewiesene Anwendung identifiziert. Weitere Informationen finden Sie unter [Application Objects und Service Principal-Objekte](https://msdn.microsoft.com/library/azure/dn132633.aspx).                            **Notes**: keine Nullwerte zulassen der **any** -Operator ist erforderlich für Filterausdrücke auf mehrwertige Eigenschaften; Weitere Informationen finden Sie unter [unterstützte Abfragen, Filter, und Paging-Optionen](https://msdn.microsoft.com/library/azure/dn727074.aspx).            |
|-Tags hinzugefügtes Markup|String|                                        **Hinweis:** Lässt keine Nullwerte zu.            |

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [ServicePrincipal](../resources/serviceprincipal.md) -Objekts in der Antworttext.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceprincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
