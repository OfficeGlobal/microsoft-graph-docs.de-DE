# <a name="teamsapp-resource-type"></a>Ressourcentyp teamsApp



Eine app in den [Microsoft-Teams,](teams_api_overview.md) app-Katalog.

Benutzer können diese apps im Microsoft-Teams Store anzeigen, und diese apps in [Teams](team.md) mithilfe der [Add-app an das Team](../api/teamsappinstallation_add.md) -Methode installiert werden können.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Liste der veröffentlichten apps](../api/teamsapp_list.md) | [TeamsApp](teamsApp.md) -Auflistung | Veröffentlichte apps aus dem Microsoft-Teams, apps Katalog aufgelistet.|
|[Veröffentlichen einer app](../api/teamsapp_publish.md) | [teamsApp](teamsApp.md) | Veröffentlichen einer app in Ihrer Organisation app-Katalog.|
|[Aktualisieren einer veröffentlichten Anwendung](../api/teamsapp_update.md) | [teamsApp](teamsApp.md) | Aktualisieren einer veröffentlichten-app in Ihrer Organisation app-Katalog.|
|[Entfernen einer veröffentlichten Anwendung](../api/teamsapp_delete.md) | Keine | Entfernen Sie eine veröffentlichte app aus Ihrer Organisation app-Katalog.|

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

# <a name="see-also"></a>Siehe auch

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

