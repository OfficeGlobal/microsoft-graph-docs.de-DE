---
title: Serviceprincipal aktualisieren
description: Aktualisieren Sie die Eigenschaften des Serviceprincipal-Objekts.
localization_priority: Normal
ms.openlocfilehash: a562bca03881923cfc21d32eadee2a7f7053fa9b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641176"
---
# <a name="update-serviceprincipal"></a>Serviceprincipal aktualisieren

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aktualisieren Sie die Eigenschaften des Serviceprincipal-Objekts.
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Application.ReadWrite.OwnedBy, Application.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Autorisierung  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|accountEnabled|Boolescher Wert|                **True**, wenn das Dienstprinzipalkonto aktiviert ist; andernfalls **false**.            |
|appDisplayName|Zeichenfolge|Der von der verknüpften Anwendung verfügbar gemachte Anzeigename.|
|appId|Zeichenfolge|Die eindeutige ID für die verknüpfte Anwendung (die **appId**-Eigenschaft).|
|appRoleAssignmentRequired|Boolescher Wert|Gibt an, ob eine **eppRoleAssignment** für einen Benutzer oder eine Gruppe erforderlichist, bevor Azure Active Directory ein Benutzer- oder Zugriffstoken für die Anwendung ausstellt.                            **Notes**: erfordert Version 1.5 oder neuere, nicht NULL-Werte zulässt.            |
|appRoles|appRole|Die von der verknüpften Anwendung verfügbar gemachten Anwendungsrollen. Weitere Informationen finden Sie in der Definition der **AppRoles** -Eigenschaft in der Anwendung Entität **Notes**: erfordert Version 1.5 oder neuere, nicht NULL-Werte zulässt.            |
|displayName|Zeichenfolge|Der Anzeigename für den Dienstprinzipal.|
|errorUrl|Zeichenfolge|            |
|homepage|Zeichenfolge|Die URL zur Homepage der zugehörigen Anwendung.|
|keyCredentials|keyCredential|Die Auflistung der wichtigsten Anmeldeinformationen, die mit dem Dienstprinzipal verknüpft sind.                            **Hinweis:** Lässt keine Nullwerte zu.            |
|logoutUrl|Zeichenfolge| Gibt die URL an, die vom Autorisierungsdienst von Microsoft verwendet wird, um einen Benutzer mithilfe von [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html)-, [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html)- oder SAML-Abmeldeprotokollen abzumelden. |
|oauth2Permissions|oAuth2Permission|Die von der verknüpften Anwendung verfügbar gemachten OAuth 2.0-Berechtigungen. Weitere Informationen finden Sie in der **oauth2Permissions**-Eigenschaftsdefinition in der application-Entität.                            **Notes**: erfordert Version 1.5 oder neuere, nicht NULL-Werte zulässt.            |
|passwordCredentials|passwordCredential|Die Auflistung der Kennwortanmeldeinformationen, die mit dem Dienstprinzipal verknüpft sind.                            **Hinweis:** Lässt keine Nullwerte zu.            |
|preferredTokenSigningKeyThumbprint|Zeichenfolge|Nur für die interne Verwendung reserviert. Schreiben Sie diese Eigenschaft nicht, und verwenden Sie diese Eigenschaft nicht anderweitig. Sie kann in zukünftigen Versionen möglicherweise entfernt werden.                            **Notes**: erfordert Version 1.5 oder höher.            |
|publisherName|Zeichenfolge|Der Anzeigename des Mandanten, in dem verknüpfte Anwendung angegeben wird.|
|replyUrls|String|Die URLs, an die Benutzertoken zur Anmeldung bei der verknüpften Anwendung gesendet werden, oder die Umleitungs-URIs, an die die OAuth 2.0-Autorisierungscodes und Zugriffstoken für die verknüpfte Anwendung gesendet werden.                            **Hinweis:** Lässt keine Nullwerte zu.            |
|samlMetadataUrl|Zeichenfolge|            |
|servicePrincipalNames|String|Die URLs, die die verknüpfte Anwendung identifizieren. Weitere Informationen finden Sie unter [Anwendungsobjekte und Dienstprinzipalobjekte](https://msdn.microsoft.com/library/azure/dn132633.aspx).                            **Notes**: keine Nullwerte zulassen der **any** -Operator ist erforderlich für Filterausdrücke auf mehrwertige Eigenschaften; Weitere Informationen finden Sie unter [unterstützte Abfragen, Filter, und Paging-Optionen](https://msdn.microsoft.com/library/azure/dn727074.aspx).            |
|tags|String|                                        **Hinweis:** Lässt keine Nullwerte zu.            |

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
<!--
{
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
