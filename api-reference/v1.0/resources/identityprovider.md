---
title: identityProvider-Ressourcentyp
description: Stellt einen Identitätsanbieter für Azure Active Directory (Azure AD) dar.
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f251853704edd644f615ab986cc3188608fbbe05
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649410"
---
# <a name="identityprovider-resource-type"></a>identityProvider-Ressourcentyp

Stellt einen Identitätsanbieter für Azure Active Directory (Azure AD) dar. Der Identitätsanbieter kann Microsoft, Google, Facebook, Amazon, LinkedIn oder Twitter sein. Die folgenden Identitätsprovider befinden in der Vorschau: Weibo, QQ, WeChat, GitHub und alle von OpenID Connect unterstützten Anbieter. 

Das Konfigurieren eines Identitätsanbieters in Ihrem Azure AD-B2C-Mandanten ermöglicht Folgendes für Benutzer:

* Registrieren und Anmelden mithilfe eines Kontos für soziale Netzwerke in einer Verbraucheranwendung. Eine Anwendung kann zum Beispiel Azure AD B2C verwenden, damit sich Benutzer für den Dienst mithilfe eines Facebook-Kontos registrieren können.
* Verknüpfen eines vorhandenen lokalen Kontos mit einem Konto für soziale Netzwerke in einer Verbraucheranwendung. Ein Benutzer hat beispielsweise einen Benutzernamen und ein Kennwort (lokales Konto) in der Anwendung erstellt. Der Benutzer entscheidet sich später, das vorhandene lokale Konto mit seinem Facebook-Konto zu verknüpfen, damit er sich mithilfe von Facebook anmelden kann.

Das Konfigurieren eines Identitätsanbieters in Ihrem Azure AD-Mandanten ermöglicht die folgenden B2B-Gastszenarien: Eine Organisation hat beispielsweise Ressourcen in Office 365, die für einen Gmail-Benutzer freigegeben werden müssen. Der Gmail-Benutzer verwendet die Anmeldeinformationen für sein Google-Konto, um sich zu authentifizieren und auf die Dokumente zuzugreifen.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Get identityProvider](../api/identityprovider-get.md) |identityProvider|Lesen der Eigenschaften eines vorhandenen Identitätsanbieters.|
|[Create identityProvider](../api/identityprovider-post-identityproviders.md)|identityProvider|Erstellen eines neuen Identitätsanbieters.|
|[Update identityProvider](../api/identityprovider-update.md)|Keine|Aktualisieren eines vorhandenen Identitätsanbieters.|
|[Delete identityProvider](../api/identityprovider-delete.md)|Keine|Löschen eines vorhandenen Identitätsanbieters.|
|[List identityProviders](../api/identityprovider-list.md)|identityProvider-Auflistung|Auflisten aller in einem Mandanten konfigurierten Identitätsanbieter.|

## <a name="properties"></a>Eigenschaften

|Eigenschaft|Typ|Erforderlich|Nullwerte zulassend.|Beschreibung|
|:---------------|:--------|:--------|:--------|:----------|
|clientId|Zeichenfolge|Ja|Nein|Die Client-ID für die Anwendung. Dies ist die Client-ID, die Sie beim Registrieren der Anwendung beim Identitätsanbieter erhalten.|
|clientSecret|Zeichenfolge|Ja|Nein|Der geheime Clientschlüssel für die Anwendung. Dies ist der geheime Clientschlüssel, den Sie beim Registrieren der Anwendung beim Identitätsanbieter erhalten. Dieser verfügt nur über Schreibzugriff. Ein Lesevorgang gibt „\*\*\*\*“ zurück.|
|id|Zeichenfolge|Nein|Nein|Die ID des Identitätsanbieters.|
|name|Zeichenfolge|Nein|Nein|Der Anzeigename des Identitätsanbieters.|
|type|Zeichenfolge|Ja|Nein|Der Typ des Identitätsanbieters. Der Typ muss einer der folgenden Werte für B2C-Szenarien sein: <ul><li/>Microsoft<li/>Google<li/>Amazon<li/>LinkedIn<li/>Facebook<li/>GitHub<li/>Twitter<li/>Weibo<li/>QQ<li/>WeChat</ul>Für B2B-Szenarien muss der Wert Google sein.|

### <a name="where-to-get-the-client-id-and-secret"></a>Wo Sie die Client-ID und den geheimen Clientschlüssel abrufen

Jeder Identitätsanbieter verfügt über einen Prozess zum Erstellen einer App-Registrierung. Benutzer erstellen zum Beispiel eine App-Registrierung bei Facebook unter [developers.facebook.com](https://developers.facebook.com/). Die resultierende Client-ID und der geheime Clientschlüssel können an [create identityProvider](../api/identityprovider-post-identityproviders.md) übergeben werden. Jedes Benutzerobjekt im Verzeichnis kann dann mit einem der Identitätsanbieter des Mandanten für die Authentifizierung im Verbund stehen. Auf diese Weise kann sich der Benutzer durch Eingeben der Anmeldeinformationen auf der Anmeldeseite des Identitätsanbieters anmelden. Das Token vom Identitätsanbieter wird von Azure AD überprüft, bevor der Mandant ein Token für die Anwendung ausstellt.

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
