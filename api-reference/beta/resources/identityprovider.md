---
title: Ressourcentyp identityProvider
description: Stellt einen Identitätsanbieter Azure Active Directory (AD Azure). Der Identitätsanbieter kann Microsoft, Google, Facebook, LinkedIn oder Amazon sein.
localization_priority: Normal
ms.openlocfilehash: afd21635d932582f2a9ee6c2cde1cf45a9d4260f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511618"
---
# <a name="identityprovider-resource-type"></a>Ressourcentyp identityProvider

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt einen Identitätsanbieter Azure Active Directory (AD Azure). Der Identitätsanbieter kann Microsoft, Google, Facebook, LinkedIn oder Amazon sein.

Konfigurieren einen Identitätsanbieter in Ihrem Mandanten Azure AD B2C ermöglicht:

* Benutzer anmelden, und melden Sie sich über ein Konto für soziale Netzwerke in einer Consumeranwendung. Beispielsweise kann eine Anwendung Azure AD B2C verwenden, um Benutzern für den Dienst mit Facebook-Konto anmelden zu ermöglichen.
* Verknüpfen eine vorhandene lokalen Benutzer in ein Konto für soziale Netzwerke in einer Consumeranwendung berücksichtigt werden. Beispielsweise hat ein Benutzer einen Benutzernamen und ein Kennwort (lokales Konto) in der Anwendung erstellt. Der Benutzer entscheidet sich später, verknüpfen das vorhandene lokale Konto mit ihren Facebook-Konto, so dass Anmeldung kann über Facebook.

Konfigurieren einen Identitätsanbieter in Ihrem Azure AD-Mandanten ermöglicht künftige B2B Gast Szenarien. Beispielsweise verfügt über eine Organisation Ressourcen in Office 365, die mit einem Gmail-Benutzer freigegeben werden müssen. Der Gmail-Benutzer verwenden die Anmeldeinformationen ihres Google zur Authentifizierung und Zugriff auf die Dokumente.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von identityProvider](../api/identityprovider-get.md) |identityProvider|Lesen Sie die Eigenschaften einer vorhandenen IdentityProvider.|
|[Erstellen von identityProvider](../api/identityprovider-post-identityproviders.md)|identityProvider|Erstellen Sie eine neue IdentityProvider.|
|[IdentityProvider aktualisieren](../api/identityprovider-update.md)|Keine|Aktualisieren einer vorhandenen IdentityProvider.|
|[IdentityProvider löschen](../api/identityprovider-delete.md)|Keine|Löschen einer vorhandenen IdentityProvider.|
|[Liste identityProviders](../api/identityprovider-list.md)|IdentityProvider-Auflistung|Listen Sie alle IdentityProviders in einem Mandanten konfiguriert.|

## <a name="properties"></a>Eigenschaften

|Eigenschaft|Typ|Erforderlich|Nullwerte zulassen|Beschreibung|
|:---------------|:--------|:--------|:--------|:----------|
|clientId|String|Ja|No|Die Client-ID für die Anwendung. Dies ist die Client-ID abgerufen wird, wenn die Anwendung mit dem Identitätsanbieter registrieren.|
|client_secret|String|Ja|No|Der geheime Clientschlüssel für die Anwendung. Dies ist der geheime Clientschlüssel erhalten Sie, wenn die Anwendung mit dem Identitätsanbieter registrieren. Dies ist lesegeschützt. Ein Lesevorgang zurückgegebenen "\*\*\*\*".|
|id|String|Nein|No|Die ID des Identitätsanbieters.|
|name|String|Nein|No|Der Anzeigename des Identitätsanbieters.|
|type|String|Ja|No|Der Typ der Identität Anbieter. Es muss eine der folgenden Werte sein: <ul><li/>Microsoft<li/>Google<li/>Amazon<li/>LinkedIn<li/>Facebook</ul>|

### <a name="where-to-get-the-client-id-and-secret"></a>Wo Sie die Client-ID und geheimen Schlüssel erhalten

Jede Identitätsanbieter verfügt über einen Prozess für das Erstellen einer app-Registrierung. Beispielsweise erstellen Benutzer eine app-Registrierung mit Facebook am [developers.facebook.com](https://developers.facebook.com/). Die resultierende Client-ID und den geheimen Clientschlüssel können zum [Erstellen von IdentityProvider](../api/identityprovider-post-identityproviders.md)übergeben werden. Klicken Sie dann kann jedes Benutzerobjekt in das Verzeichnis aller Identitätsanbieter für die Authentifizierung des Mandanten verbunden sein. Dies ermöglicht dem Benutzer anmelden, indem Sie auf der Anmeldeseite des Identitätsanbieters Anmeldeinformationen eingeben. Von Azure Active Directory vor der Mandanten für die Anwendung ein Token ausstellt, wird das Token vom Identitätsanbieter überprüft.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->

```json
{
    "id": "String",
    "type": "String",
    "name": "String",
    "clientId": "String",
    "clientSecret": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/identityprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
