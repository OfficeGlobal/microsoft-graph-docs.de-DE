---
title: Geräteressourcentyp
description: Stellt ein Gerät dar, das in der Organisation registriert ist. Geräte werden mithilfe des Geräteregistrierungsdiensts oder von Intune in der Cloud erstellt. Sie werden von Richtlinien für bedingten Zugriff für mehrstufige Authentifizierung verwendet. Diese Geräte können Desktopcomputer, Laptops sowie Mobiltelefone und Tablets umfassen. Erbt von directoryObject.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e72777691f0c599067c885168c0c58bb49cec3cb
ms.sourcegitcommit: 159cf5aaa39d3721d96d3fd800f6a8b91159f74d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2019
ms.locfileid: "30379528"
---
# <a name="device-resource-type"></a>Geräteressourcentyp

Stellt ein Gerät dar, das in der Organisation registriert ist. Geräte werden mithilfe des Geräteregistrierungsdiensts oder von Intune in der Cloud erstellt. Sie werden von Richtlinien für bedingten Zugriff für mehrstufige Authentifizierung verwendet. Diese Geräte können Desktopcomputer, Laptops sowie Mobiltelefone und Tablets umfassen. Erbt von [directoryObject](directoryobject.md).

Diese Ressource ermöglicht es Ihnen, benutzerdefinierten Eigenschaften mithilfe von [Erweiterungen](/graph/extensibility-overview) eigene Daten hinzuzufügen.


## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Get device](../api/device-get.md) | [device](device.md) |Dient zum Lesen der Eigenschaften und der Beziehungen eines Geräteobjekts.|
|[List devices](../api/device-list.md) | [Geräte](device.md)sammlung| Dient zum Abrufen einer Liste von Geräten, die in dem Verzeichnis registriert sind. |
|[Update device](../api/device-update.md) | [Gerät](device.md) |Dient zum Aktualisieren der Eigenschaften eines Geräteobjekts. |
|[Delete device](../api/device-delete.md) | Keine |Dient zum Löschen eines Geräteobjekts. |
|[List memberOf](../api/device-list-memberof.md) |[directoryObject](directoryobject.md) collection| Listet die Gruppen auf, von denen das Gerät direkt Mitglied ist. |
|[List registeredOwners](../api/device-list-registeredowners.md) |[directoryObject](directoryobject.md) collection| Dient zum Abrufen der Benutzer, die registrierte Besitzer des Geräts in der registeredOwners-Navigationseigenschaft sind.|
|[List registeredUsers](../api/device-list-registeredusers.md) |[directoryObject](directoryobject.md)-Sammlung| Dient zum Abrufen registrierter Benutzer des Geräts aus der registeredUsers-Navigationseigenschaft.|
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften zu einer neuen oder vorhandenen Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Dient zum Abrufen einer offenen Erweiterung, die durch den Erweiterungsnamen identifiziert wird.|
|**Schemaerweiterungen**| | |
|[Schemaerweiterungswerte hinzufügen](/graph/extensibility-schema-groups) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| **true**, wenn das Konto aktiviert ist; andernfalls **false**. Erforderlich.|
|alternativeSecurityIds|alternativeSecurityId-Sammlung| Nur für internen Gebrauch. Lässt keine Nullwerte zu. |
|approximateLastSignInDateTime|DateTimeOffset| Der timestamp-Typ stellt Datums-und Uhrzeitinformationen unter Verwendung des ISO 8601-Formats dar und ist immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt. |
|complianceExpirationDateTime|DateTimeOffset| Der Zeitstempel, wenn das Gerät nicht mehr als kompatibel angesehen wird. Der timestamp-Typ stellt Datums-und Uhrzeitinformationen unter Verwendung des ISO 8601-Formats dar und ist immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt. |
|deviceId|string| Der eindeutige Bezeichner, der vom Azure-Geräteregistrierungsdienst bei der Registrierung festgelegt wird. |
|deviceMetadata|Zeichenfolge| Nur für internen Gebrauch. Auf Null festgelegt. |
|deviceVersion|Int32| Nur für internen Gebrauch. |
|displayName|String|Der Anzeigename für das Gerät. Erforderlich. |
|id|Zeichenfolge|Die eindeutige ID für das Gerät. Geerbt von [directoryObject](directoryobject.md). Schlüssel, lässt keine Nullwerte zu. Schreibgeschützt.|
|isCompliant|Boolean|**true**, wenn das Gerät den Richtlinien für mobile Geräteverwaltung ( Mobile Device Management, MDM) entspricht; andernfalls **false**. Schreibgeschützt. Dies kann nur von InTune für beliebige Gerätebetriebssystem-Typen oder von einer [genehmigtEN MDM-App](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) für Windows-Betriebssystem Geräte aktualisiert werden.|
|isManaged|Boolescher Wert|**true**, wenn das Gerät durch die mobile Geräteverwaltungs-App verwaltet wird; andernfalls **false**. Dies kann nur von InTune für beliebige Gerätebetriebssystem-Typen oder von einer [genehmigtEN MDM-App](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) für Windows-Betriebssystem Geräte aktualisiert werden. |
|onPremisesLastSyncDateTime|DateTimeOffset|Der Zeitpunkt der letzten Synchronisierung des Objekts mit dem lokalen Verzeichnis. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'` Schreibgeschützt.|
|onPremisesSyncEnabled|Boolean|**true**, wenn das Objekt aus einem lokalen Verzeichnis synchronisiert wird; **false**, wenn das Objekt ursprünglich aus einem lokalen Verzeichnis synchronisiert wurde, aber nicht mehr synchronisiert wird; **NULL**, wenn dieses Objekt nie aus einem lokalen Verzeichnis synchronisiert wurde (Standard). Schreibgeschützt. |
|operatingSystem|Zeichenfolge| Der Typ des Betriebssystems auf dem Gerät. Erforderlich. |
|operatingSystemVersion|Zeichenfolge|Die Version des Betriebssystems auf dem Gerät. Erforderlich. |
|physicalIds|Zeichenfolgenauflistung| Nur für internen Gebrauch. Lässt keine Nullwerte zu. |
|Profile Type|Zeichenfolge|Der Profiltyp des Geräts. Mögliche Werte:<br />**RegisteredDevice** Standard<br />**SecureVM**<br />**Printer**<br />**Shared**<br />**IoT**|
|systemLabels|String collection| Liste der Bezeichnungen, die vom System auf das Gerät angewendet werden. |
|trustType|String| Typ von Vertrauensstellung für das beigetretene Gerät. Schreibgeschützt. Mögliche Werte: <br />**Arbeitsplatz** - Gibt an *, dass eigene persönliche Geräte mitgebracht werden sollen*<br />**AzureAd** - Nur Geräte, die mit der Cloud verknüpft sind<br />**ServerAd** - Lokale Geräte, die der Domäne beigetreten sind, die mit Azure AD verknüpft sind. Weitere Informationen hierzu finden Sie unter [Einführung in die Geräteverwaltung in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Erweiterungen|[extension](extension.md)-Sammlung|Die Sammlung der für das Gerät definierten offenen Erweiterungen. Schreibgeschützt. Lässt Nullwerte zu.|
|memberOf|[directoryObject](directoryobject.md) collection|Gruppen, bei denen diese Gruppe Mitglied ist. HTTP-Methoden: GET (unterstützt für alle Gruppen). Schreibgeschützt. Lässt NULL-Werte zu.|
|[Transitive memberOf auflisten](../api/device-list-transitivememberof.md) |[directoryObject](directoryobject.md)-Sammlung| Listet die Gruppen auf, in denen das Gerät Mitglied ist. Dieser Vorgang ist transitiv. |
|registeredOwners|[directoryObject](directoryobject.md) collection|Der Benutzer, dessen Gerät mit der Cloud verknüpft ist oder der sein persönliches Gerät registriert hat. Der registrierte Besitzer wird zum Zeitpunkt der Registrierung festgelegt. Derzeit kann jeweils nur ein Besitzer vorhanden sein. Schreibgeschützt. Nullwerte zulassend. |
|registeredUsers|[directoryObject](directoryobject.md)-Sammlung|Auflistung von Benutzern, die registrierte Benutzer des Geräts sind. Für mit der Cloud verknüpfte Geräte und registrierte persönliche Geräte werden registrierte Benutzer bei der Registrierung auf den gleichen Wert wie registrierte Besitzer festgelegt. Schreibgeschützt. Nullwerte zulassend.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "extensions",
    "registeredOwners",
    "registeredUsers"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.device"
}-->

```json
{
  "accountEnabled": true,
  "alternativeSecurityIds": [{"@odata.type": "microsoft.graph.alternativeSecurityId"}],
  "approximateLastSignInDateTime": "String (timestamp)",
  "complianceExpirationDateTime": "String (timestamp)",
  "deviceId": "string",
  "deviceMetadata": "string",
  "deviceVersion": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "isCompliant": true,
  "isManaged": true,
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "operatingSystem": "string",
  "operatingSystemVersion": "string",
  "physicalIds": ["string"],
  "profileType": "string",
  "systemLabels": ["string"],
  "trustType": "string"
}
```

## <a name="see-also"></a>Siehe auch

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](/graph/extensibility-open-users)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "device resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
