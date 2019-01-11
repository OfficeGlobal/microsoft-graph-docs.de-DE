---
title: Ressourcentyp „termsAndConditions“
description: C-Richtlinien Inhalt zur Verfügung gestellt Benutzer ihre ersten Versuch in Intune registrieren und anschließend bearbeitet, wobei ein Administrator Re-Annahme erforderlich ist. Mithilfe dieser Richtlinien können Administratoren die Bedingungen festlegen, die Benutzer akzeptieren müssen, bevor sie ihre Geräte in Intune registrieren dürfen.
localization_priority: Normal
ms.openlocfilehash: 2f435f08c306f8dadd76257e19a53c9a6cee95d7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881578"
---
# <a name="termsandconditions-resource-type"></a>Ressourcentyp „termsAndConditions“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine Entität des Typs „termsAndConditions“ repräsentiert die Metadaten und Inhalte einer Geschäftsbedingungen-Richtlinie. Die Inhalte von Geschäftsbedingungen-Richtlinien werden Benutzern angezeigt, wenn sie sich erstmals bei Intune registrieren. Sie werden ebenfalls angezeigt, wenn ein Administrator Bearbeitungen vorgenommen hat und festlegt, dass eine erneute Annahme der Bedingungen nötig ist. Mithilfe dieser Richtlinien können Administratoren die Bedingungen festlegen, die Benutzer akzeptieren müssen, bevor sie ihre Geräte in Intune registrieren dürfen.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „termsAndConditions“](../api/intune-companyterms-termsandconditions-list.md)|Sammlung von Objekten des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) auf.|
|[Abrufen von „termsAndConditions“](../api/intune-companyterms-termsandconditions-get.md)|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).|
|[Erstellen von „termsAndConditions“](../api/intune-companyterms-termsandconditions-create.md)|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Erstellt neue Objekte des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).|
|[Löschen von „termsAndConditions“](../api/intune-companyterms-termsandconditions-delete.md)|Keiner|Löscht Objekte des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).|
|[Aktualisieren von „termsAndConditions“](../api/intune-companyterms-termsandconditions-update.md)|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Aktualisiert die Eigenschaften von Objekten des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner der Geschäftsbedingungen-Richtlinie|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts.|
|displayName|Zeichenfolge|Name der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt) |
|description|Zeichenfolge|Beschreibung der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)|
|title|Zeichenfolge|Titel der Geschäftsbedingungen (vom Administrator festgelegt). Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.|
|bodyText|Zeichenfolge|Text der Geschäftsbedingungen (vom Administrator festgelegt). In der Regel handelt es sich um die Bedingungen selbst. Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.|
|acceptanceStatement|Zeichenfolge|Erläuterung der Geschäftsbedingungen (vom Administrator bereitgestellt). Sie beschreibt in der Regel, was es für den Benutzer bedeutet, wenn er die Geschäftsbedingungen in der Geschäftsbedingungen-Richtlinie annimmt. Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.|
|Version|Int32|Ganze Zahl, die die aktuelle Version der Geschäftsbedingungen angibt. Sie wird heraufgesetzt, wenn ein Administrator die Bedingungen ändert und festlegt, dass Benutzer die geänderten Bedingungen erneut annehmen müssen.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|Sammlung von Objekten des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)|Liste der Zuweisungen der Geschäftsbedingungen-Richtlinie|
|acceptanceStatuses|Sammlung von Objekten des Typs [TermsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|Liste der Annahmestatus der Geschäftsbedingungen-Richtlinie|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
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



