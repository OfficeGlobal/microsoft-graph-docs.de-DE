# <a name="termsandconditions-resource-type"></a>Ressourcentyp „termsAndConditions“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine Entität des Typs „termsAndConditions“ repräsentiert die Metadaten und Inhalte einer Geschäftsbedingungen-Richtlinie. Die Inhalte von Geschäftsbedingungen-Richtlinien werden Benutzern angezeigt, wenn sie sich erstmals bei Intune registrieren. Sie werden ebenfalls angezeigt, wenn ein Administrator Bearbeitungen vorgenommen hat und festlegt, dass eine erneute Annahme der Bedingungen nötig ist. Mithilfe dieser Richtlinien können Administratoren die Bedingungen festlegen, die Benutzer akzeptieren müssen, bevor sie ihre Geräte in Intune registrieren dürfen.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „termsAndConditions“](../api/intune_companyterms_termsandconditions_list.md)|Sammlung von Objekten des Typs [termsAndConditions](../resources/intune_companyterms_termsandconditions.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) auf.|
|[Abrufen von „termsAndConditions“](../api/intune_companyterms_termsandconditions_get.md)|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [termsAndConditions](../resources/intune_companyterms_termsandconditions.md).|
|[Erstellen von „termsAndConditions“](../api/intune_companyterms_termsandconditions_create.md)|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md)|Erstellt neue Objekte des Typs [termsAndConditions](../resources/intune_companyterms_termsandconditions.md).|
|[Löschen von „termsAndConditions“](../api/intune_companyterms_termsandconditions_delete.md)|Keiner|Löscht Objekte des Typs [termsAndConditions](../resources/intune_companyterms_termsandconditions.md).|
|[Aktualisieren von „termsAndConditions“](../api/intune_companyterms_termsandconditions_update.md)|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md)|Aktualisiert die Eigenschaften von Objekten des Typs [termsAndConditions](../resources/intune_companyterms_termsandconditions.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner der Geschäftsbedingungen-Richtlinie|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts|
|displayName|String|Name der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt) |
|description|String|Beschreibung der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)|
|title|String|Titel der Geschäftsbedingungen (vom Administrator festgelegt). Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.|
|bodyText|String|Text der Geschäftsbedingungen (vom Administrator festgelegt). In der Regel handelt es sich um die Bedingungen selbst. Dieser Text wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.|
|acceptanceStatement|String|Erläuterung der Geschäftsbedingungen (vom Administrator bereitgestellt). Sie beschreiben in der Regel, was es für den Benutzer bedeutet, wenn er die Geschäftsbedingungen in der Geschäftsbedingungen-Richtlinie annimmt. Dieser Text wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.|
|version|Int32|Ganze Zahl, die die aktuelle Version der Geschäftsbedingungen angibt. Sie wird heraufgesetzt, wenn ein Administrator die Bedingungen ändert und festlegt, dass Benutzer die geänderten Bedingungen erneut annehmen müssen.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|Sammlung von Objekten des Typs [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)|Liste der Zuweisungen der Geschäftsbedingungen-Richtlinie|
|acceptanceStatuses|Sammlung von Objekten des Typs [TermsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|Liste der Annahmestatus der Geschäftsbedingungen-Richtlinie|

## <a name="json-representation"></a>JSON-Darstellung
Unten sehen Sie eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "title": "String",
  "bodyText": "String",
  "acceptanceStatement": "String",
  "version": 1024
}
```


