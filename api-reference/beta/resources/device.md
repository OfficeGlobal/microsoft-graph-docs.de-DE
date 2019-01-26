---
title: Geräteressourcentyp
description: Stellt ein Gerät im Verzeichnis registriert. Geräte werden mithilfe des Geräteregistrierungsdiensts oder von Intune in der Cloud erstellt. Sie werden von Richtlinien für bedingten Zugriff für mehrstufige Authentifizierung verwendet. Diese Geräte können Desktopcomputer, Laptops sowie Mobiltelefone und Tablets umfassen. Erbt von directoryObject.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 42b1f0625cfa14f7beff1d4206bd93abb9f9a9e9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574873"
---
# <a name="device-resource-type"></a>Geräteressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt ein Gerät im Verzeichnis registriert. Geräte werden mithilfe des Geräteregistrierungsdiensts oder von Intune in der Cloud erstellt. Sie werden von Richtlinien für bedingten Zugriff für mehrstufige Authentifizierung verwendet. Diese Geräte können Desktopcomputer, Laptops sowie Mobiltelefone und Tablets umfassen. Erbt von [directoryObject](directoryobject.md).

Diese Ressource ermöglicht es Ihnen, benutzerdefinierten Eigenschaften mithilfe von [Erweiterungen](/graph/extensibility-overview) eigene Daten hinzuzufügen.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Get device](../api/device-get.md) | [Gerät](device.md) |Lesen Sie Eigenschaften und Beziehungen des Geräts-Objekts.|
|[List devices](../api/device-list.md) | [Geräte](device.md)sammlung| Dient zum Abrufen einer Liste von Geräten, die in dem Verzeichnis registriert sind. |
|[Update device](../api/device-update.md) | [Gerät](device.md)  |Aktualisieren Sie die Eigenschaften des Geräts-Objekts. |
|[Delete device](../api/device-delete.md) | Keine |Das Objekt zu löschen. |
|[memberOf auflisten](../api/device-list-memberof.md) |[directoryObject](directoryobject.md)-Sammlung| Auflisten der Gruppen, denen das Gerät ein direktes Mitglied ist. |
|[Transitive memberOf auflisten](../api/device-list-transitivememberof.md) |[directoryObject](directoryobject.md)-Sammlung| Auflisten der Gruppen, denen das Gerät ein Mitglied ist. Dieser Vorgang ist transitiv. |
|[List registeredOwners](../api/device-list-registeredowners.md) |[directoryObject](directoryobject.md)-Sammlung| Dient zum Abrufen der Benutzer, die registrierte Besitzer des Geräts in der registeredOwners-Navigationseigenschaft sind.|
|[List registeredUsers](../api/device-list-registeredusers.md) |[directoryObject](directoryobject.md)-Sammlung| Dient zum Abrufen registrierter Benutzer des Geräts aus der registeredUsers-Navigationseigenschaft.|
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften zu einer neuen oder vorhandenen Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Dient zum Abrufen einer offenen Erweiterung, die durch den Erweiterungsnamen identifiziert wird.|
|**Schemaerweiterungen**| | |
|[Schemaerweiterungswerte hinzufügen](/graph/extensibility-schema-groups) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| **true**, wenn das Konto aktiviert ist; andernfalls **false**. Der Standardwert ist true.|
|alternativeSecurityIds| microsoft.graph.alternativeSecurityId-Auflistung | Nur für internen Gebrauch. Lässt keine Nullwerte zu. |
|approximateLastSignInDateTime|DateTimeOffset| Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt. |
|deviceId|Zeichenfolge (ID)| Der eindeutige Bezeichner, der vom Azure-Geräteregistrierungsdienst bei der Registrierung festgelegt wird. |
|deviceMetadata|String| Nur für internen Gebrauch. Auf Null festgelegt. |
|deviceVersion|Int32| Nur für internen Gebrauch. |
|displayName|String| Der Anzeigename für das Gerät. Erforderlich. |
|id|String|Die eindeutige ID für das Gerät. Geerbt von [directoryObject](directoryobject.md). Schlüssel, lässt keine Nullwerte zu. Schreibgeschützt.|
|isCompliant|Boolean|**true**, wenn das Gerät den Richtlinien für mobile Geräteverwaltung ( Mobile Device Management, MDM) entspricht; andernfalls **false**. Schreibgeschützt. Dies kann nur durch Intune für einen beliebigen Gerätetyp Betriebssystem oder durch eine [genehmigt MDM-app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) für Windows-Betriebssystem Geräte aktualisiert werden.|
|isManaged|Boolean|**true**, wenn das Gerät durch die mobile Geräteverwaltungs-App verwaltet wird; andernfalls **false**. Dies kann nur durch Intune für einen beliebigen Gerätetyp Betriebssystem oder durch eine [genehmigt MDM-app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) für Windows-Betriebssystem Geräte aktualisiert werden. |
|onPremisesLastSyncDateTime|DateTimeOffset|Der Zeitpunkt der letzten Synchronisierung des Objekts mit dem lokalen Verzeichnis. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'` Schreibgeschützt. |
|onPremisesSyncEnabled|Boolean|**true**, wenn das Objekt aus einem lokalen Verzeichnis synchronisiert wird; **false**, wenn das Objekt ursprünglich aus einem lokalen Verzeichnis synchronisiert wurde, aber nicht mehr synchronisiert wird; **NULL**, wenn dieses Objekt nie aus einem lokalen Verzeichnis synchronisiert wurde (Standard). Schreibgeschützt.|
|operatingSystem|String| Der Typ des Betriebssystems auf dem Gerät. Erforderlich. |
|operatingSystemVersion|String| Auf dem Gerät installierte Betriebssystemversion.
 Erforderlich. |
|physicalIds|Zeichenfolgenauflistung| Nur für internen Gebrauch. Lässt keine Nullwerte zu. |
|trustType|String| Typ von Vertrauensstellung für das beigetretene Gerät. Schreibgeschützt. Mögliche Werte: <br />**Arbeitsplatz** - Gibt an *, dass eigene persönliche Geräte mitgebracht werden sollen*<br />**AzureAd** - Nur Geräte, die mit der Cloud verknüpft sind<br />**ServerAd** - Lokale Geräte, die der Domäne beigetreten sind, die mit Azure AD verknüpft sind. Weitere Informationen hierzu finden Sie unter [Einführung in die Geräteverwaltung in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) |
|Name| String | Der Anzeigename eines Geräts. Nur zurückgegeben, wenn sich Benutzer mit einem Microsoft-Konto als Teil des Project-ROM anmeldet. |
|Status | String| Gerät ist online oder offline. Nur zurückgegeben, wenn sich Benutzer mit einem Microsoft-Konto als Teil des Project-ROM anmeldet. |
|Plattform |String|Plattform des Geräts. Nur zurückgegeben, wenn sich Benutzer mit einem Microsoft-Konto als Teil des Project-ROM anmeldet. Nur zurückgegeben, wenn sich Benutzer mit einem Microsoft-Konto als Teil des Project-ROM anmeldet.|
|Art| String| Formfaktor des Geräts. Nur zurückgegeben, wenn sich Benutzer mit einem Microsoft-Konto als Teil des Project-ROM anmeldet. |
|Model| String| Modell des Geräts. Nur zurückgegeben, wenn sich Benutzer mit einem Microsoft-Konto als Teil des Project-ROM anmeldet. |
|Hersteller| String| Hersteller des Geräts. Nur zurückgegeben, wenn sich Benutzer mit einem Microsoft-Konto als Teil des Project-ROM anmeldet. |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Erweiterungen|[extension](extension.md)-Sammlung|Die Sammlung der für das Gerät definierten offenen Erweiterungen. Schreibgeschützt. Lässt Nullwerte zu.|
|registeredOwners|[directoryObject](directoryobject.md)-Sammlung| Der Benutzer, dessen Gerät mit der Cloud verknüpft ist oder der sein persönliches Gerät registriert hat. Der registrierte Besitzer wird zum Zeitpunkt der Registrierung festgelegt. Derzeit kann jeweils nur ein Besitzer vorhanden sein. Schreibgeschützt. Lässt Nullwerte zu.|
|registeredUsers|[directoryObject](directoryobject.md)-Sammlung| Auflistung von Benutzern, die registrierte Benutzer des Geräts sind. Für mit der Cloud verknüpfte Geräte und registrierte persönliche Geräte werden registrierte Benutzer bei der Registrierung auf den gleichen Wert wie registrierte Besitzer festgelegt. Schreibgeschützt. Nullwerte zulassend.|
|extensions|[extension](extension.md)-Sammlung|Die Auflistung der open-Erweiterungen für das Gerät definiert. Nullwerte zulassend.|
|registeredOwners|[directoryObject](directoryobject.md)-Sammlung|Benutzer, die registrierte Besitzer des Geräts sind. Schreibgeschützt. Lässt Nullwerte zu.|
|registeredUsers|[directoryObject](directoryobject.md)-Sammlung|Benutzer, die registrierte Benutzer des Geräts sind. Schreibgeschützt. Lässt Nullwerte zu.|
|Befehle | Microsoft.Graph.Command-Auflistung | Befehle, die an dieses Gerät gesendet|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions",
    "registeredOwners",
    "registeredUsers"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.device"
}-->

```json
{
  "accountEnabled": true,
  "alternativeSecurityIds": [{"@odata.type": "microsoft.graph.alternativeSecurityId"}],
  "approximateLastSignInDateTime": "String (timestamp)",
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
  "trustType": "string",
  "Name": "string",
  "Status": "string",
  "Platform": "string",
  "Kind": "string",
  "Model": "string",
  "Manufacturer": "string"
}
```

## <a name="see-also"></a>Siehe auch

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](/graph/extensibility-open-users)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "device resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/device.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
