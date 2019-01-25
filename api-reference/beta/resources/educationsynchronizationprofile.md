---
title: Ressourcentyp educationSynchronizationProfile
description: Stellt eine Reihe von Konfigurationen, die zum Synchronisieren von Education Entitäten und der Teilnehmerliste einer Informationen aus einem Quellverzeichnis in Azure Active Directory (AD Azure) verwendet. Diese Ressource enthält eine programmgesteuerte Darstellung in Schule Daten Sync verwendet.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e1b81ff14aca2b0f81a7f50e01aed6281d03d14d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523463"
---
# <a name="educationsynchronizationprofile-resource-type"></a>Ressourcentyp educationSynchronizationProfile

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine Reihe von Konfigurationen, die zum Synchronisieren von Education Entitäten und der Teilnehmerliste einer Informationen aus einem Quellverzeichnis in Azure Active Directory (AD Azure) verwendet. Diese Ressource enthält eine programmgesteuerte Darstellung in [Schule Daten Sync](https://sds.microsoft.com)verwendet.

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:-|:-|:-|
| [Liste Synchronisierungsprofile](../api/educationsynchronizationprofile-list.md) | **EducationSynchronizationProfile** -Auflistung | Abrufen von Listen aller Profile für die Synchronisierung im Mandanten. |
| [Synchronisierung Profil abrufen](../api/educationsynchronizationprofile-get.md) | **educationSynchronizationProfile** | Abrufen von einem bestimmten Profil, wenn der Bezeichner Profil. |
| [Erstellen Sie Synchronisierung Profil](../api/educationsynchronizationprofile-post.md) | Keine | Erstellen Sie ein neues Profil Synchronisierung. |
| [Synchronisierung Profil löschen](../api/educationsynchronizationprofile-delete.md) | **educationSynchronizationProfile** | Löschen von einem bestimmten Profil, wenn der Bezeichner Profil. |
| [Eine laufende Synchronisierung anhalten](../api/educationsynchronizationprofile-pause.md) | Keine | Halten Sie eine laufende Synchronisation. |
| [Fortsetzen einer angehaltenen sync](../api/educationsynchronizationprofile-resume.md) | Keine | Fortzusetzen Sie eine angehaltene Synchronisierung. |
| [Zurücksetzen einer Synchronisierung](../api/educationsynchronizationprofile-reset.md) | Keine | Zurücksetzen Sie den Zustand des Profils und starten Sie Synchronisierung. |
| [Synchronisierung für Uploaddateien starten](../api/educationsynchronizationprofile-start.md) | [EducationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md) -Auflistung| Überprüfen der hochgeladenen Dateien, und starten Sie die Synchronisierung. Gilt nur, wenn der Datenanbieter [EducationCsvDataProvider](educationcsvdataprovider.md)ist. |
| [Abrufen einer Upload-URL](../api/educationsynchronizationprofile-uploadurl.md) | string | Zurückgeben der kurzlebigen URL zum Hochladen der CSV-Datendateien. Gilt nur, wenn der Datenanbieter [EducationCsvDataProvider](educationcsvdataprovider.md)ist. |
| [Abrufen des Status der Synchronisierung](../api/educationsynchronizationprofilestatus-get.md) | [status](educationsynchronizationprofilestatus.md) | Der Status eines bestimmten Synchronisierungsprofils zurückgegeben. |
| [Abrufen von Synchronisierungsfehler](../api/educationsynchronizationerrors-get.md) | [EducationSynchronizationError](educationsynchronizationerror.md) -Auflistung| Rufen Sie alle Fehler während der Synchronisierung. |

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **displayName** | string |  Name des Konfigurationsprofils zum Synchronisieren von Identitäten.         |
| **Datenprovider** | [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md) |  Der Datenanbieter für das Profil verwendet.         |
| **identitySynchronizationConfiguration** | [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md) | Identität [Erstellung](educationidentitycreationconfiguration.md) oder [übereinstimmenden](educationidentitymatchingconfiguration.md) Konfiguration.        |
| **licensesToAssign** | [EducationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md) -Auflistung|  Lizenz-Setup-Konfiguration.        |
| **state** | educationSynchronizationProfileState |  Der Zustand des Profils. Mögliche Werte sind: `provisioning`, `provisioned`, `provisioningFailed`, `deleting` und `deletionFailed`.          |

## <a name="relationships"></a>Beziehungen

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **errors** | [EducationSynchronizationError](educationsynchronizationerror.md) -Auflistung| Alle Fehler im Zusammenhang mit diesem Profil Synchronisierung. |
| **profileStatus** | [educationSynchronizationProfileStatus](educationsynchronizationprofilestatus.md) | Der Synchronisierungsstatus. |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource **EducationSynchronizationProfile** .

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfile"
}-->

```json
{
    "displayName": "String",
    "state": { "@odata.type": "microsoft.graph.educationSynchronizationProfileState" },
    "profileStatus": {"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"},
    "errors": [{"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus" }],
    "dataProvider": { "@odata.type": "microsoft.graph.educationCsvDataProvider" },
    "identitySynchronizationConfiguration": { "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration" },
    "licensesToAssign": [{"@odata.type":"microsoft.graph.educationSynchronizationLicenseAssignment"}],
    "handleSpecialCharacterConstraint": "Boolean"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationprofile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
