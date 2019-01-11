---
title: Ressourcentyp teamsApp
description: Eine app in den Microsoft-Teams, app-Katalog.
author: nkramer
localization_priority: Priority
ms.openlocfilehash: 8f3e5b094b46376bd9ad5e9e888d76f8a995fed3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880829"
---
# <a name="teamsapp-resource-type"></a>Ressourcentyp teamsApp



Eine app in den [Microsoft-Teams,](teams-api-overview.md) app-Katalog.

Benutzer können diese apps im Microsoft-Teams Store anzeigen, und diese apps in [Teams](team.md) mithilfe der [Add-app an das Team](../api/teamsappinstallation-add.md) -Methode installiert werden können.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Liste der veröffentlichten apps](../api/teamsapp-list.md) | [TeamsApp](teamsapp.md) -Auflistung | Veröffentlichte apps aus dem Microsoft-Teams, apps Katalog aufgelistet.|
|[Veröffentlichen einer app](../api/teamsapp-publish.md) | [teamsApp](teamsapp.md) | Veröffentlichen einer app in Ihrer Organisation app-Katalog.|
|[Aktualisieren einer veröffentlichten Anwendung](../api/teamsapp-update.md) | [teamsApp](teamsapp.md) | Aktualisieren einer veröffentlichten-app in Ihrer Organisation app-Katalog.|
|[Entfernen einer veröffentlichten Anwendung](../api/teamsapp-delete.md) | Keine | Entfernen Sie eine veröffentlichte app aus Ihrer Organisation app-Katalog.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ     | Beschreibung |
|:------------------- |:-------- |:----------- |
| id                  | string   | Der app Katalog generierte app-ID (andere Entwickler bereitgestellter ID in der [Microsoft-Teams, Zip-app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). |
| externalId          | string   | Die ID des Katalogs von der app-Entwickler in der [Microsoft-Teams, zip-app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)bereitgestellt. |
| displayName                | string   | Der Name der Katalog app von der app-Entwickler in der [Microsoft-Teams, zip-app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)bereitgestellt. |
| distributionMethod  | teamsAppDistributionMethod     | Die Methode der Verteilung für die app. |

### <a name="teamsappdistributionmethod-values"></a>TeamsAppDistributionMethod Werte

|Element|Wert|Beschreibung|
|:---|:---|:---|
|Speichern|0| Die app ist für alle Mandanten über Microsoft-Teams app Store verfügbar.|
|Organisation|1|Die app ist nur in diesen Mandanten verfügbar.|
|sideloaded|2|Die app steht nur für die Benutzer/Team seine installierten an.|

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ   | Beschreibung |
|:---------------|:--------|:----------|
|appDefinitions|[TeamsAppDefinition](teamsappdefinition.md) -Auflistung| Die Details für jede Version der app. |

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsApp",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "externalId": "string",
  "displayName": "Test App",
  "distributionMethod": "Organization"
}
```

# <a name="see-also"></a>Weitere Artikel

- [teamsAppInstallation](teamsappinstallation.md)
- [teamsAppDefinition](teamsappdefinition.md)
- [teamsTab](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

