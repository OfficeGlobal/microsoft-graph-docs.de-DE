# <a name="mediacontentratingunitedkingdom-resource-type"></a>mediaContentRatingUnitedKingdom-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|movieRating|[ratingUnitedKingdomMoviesType](../resources/intune_deviceconfig_ratingunitedkingdommoviestype.md)|Filmbewertung für Großbritannien. Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.|
|tvRating|[ratingUnitedKingdomTelevisionType](../resources/intune_deviceconfig_ratingunitedkingdomtelevisiontype.md)|TV-Bewertung für Großbritannien. Mögliche Werte: `allAllowed`, `allBlocked` und `caution`.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```








