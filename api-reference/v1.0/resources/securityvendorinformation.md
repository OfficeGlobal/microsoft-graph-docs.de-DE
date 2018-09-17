# <a name="securityvendorinformation-resource-type"></a>Ressourcentyp securityVendorInformation

Enthält Angaben zum Sicherheitsprodukt/Dienstleister, Anbieter und Unteranbieter (bspw. vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|provider *|Zeichenfolge|Bestimmter Anbieter (Produkt/Dienst - kein Herstellerunternehmen); beispielsweise WindowsDefenderATP.|
|providerVersion|Zeichenfolge|Version des Anbieters oder Unteranbieters, falls vorhanden, die die Warnung ausgelöst hat.|
|subProvider|Zeichenfolge|Bestimmter Unteranbieter (unter einem aggregierten Anbieter); beispielsweise WindowsDefenderATP.SmartScreen.|
|vendor *|Zeichenfolge|Name des Warnungs-Software-Herstellers (beispielsweise Microsoft, Dell, FireEye).|
(\* Kennzeichnet ein Pflichtfeld.)

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
