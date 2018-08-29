# <a name="planneruserids-resource-type"></a>plannerUserIds-Ressourcentyp

Die **plannerUserIds**-Ressource stellt die Liste der Benutzer-IDs dar, für die ein [Plan](plannerplan.md) freigegeben wird. Es handelt sich um einen offenen Typ. Wenn Sie Office 365 Gruppen nutzen, verwenden Sie die Gruppen-API zum Verwalten von Gruppenmitgliedschaften, um den Plan der [Gruppe](group.md) freizugeben. Sie können auch vorhandene Mitglieder der Gruppe zu dieser Sammlung hinzufügen, dies ist jedoch nicht erforderlich, damit sie auf den im Besitz der Gruppe befindlichen Plan zugreifen können.


## <a name="properties"></a>Eigenschaften
Eigenschaften mit offenem Typ können vom Client definiert werden. In diesem Fall sollte der Client Benutzer-IDs als Eigenschaften angeben, deren Wert das boolesche `true` ist. Wenn für Benutzer-IDs keine Freigabe mehr erfolgt, werden Eigenschaften automatisch entfernt, indem ihre Werte auf das boolesche `false` festgelegt werden.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
  "@odata.type": "microsoft.graph.plannerUserIds"
}-->

```json
{
  "String-value": true
}
```

// Beispiel
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->