---
title: termsAndConditionsAcceptanceStatus-Ressourcentyp
description: Eine termsAndConditionsAcceptanceStatus-Entität stellt den Annahmestatus einer bestimmten Geschäftsbedingungen-Richtlinie durch einen bestimmten Benutzer dar. Benutzer müssen die neueste Version der Geschäftsbedingungen akzeptieren, um weiterhin Zugriff auf das Unternehmensportal zu haben.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35c6c3cd34c21b568f319e6b039856fd1f82ddb4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172163"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a>termsAndConditionsAcceptanceStatus-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Eine termsAndConditionsAcceptanceStatus-Entität stellt den Annahmestatus einer bestimmten Geschäftsbedingungen-Richtlinie durch einen bestimmten Benutzer dar. Benutzer müssen die neueste Version der Geschäftsbedingungen akzeptieren, um weiterhin Zugriff auf das Unternehmensportal zu haben.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[termsAndConditionsAcceptanceStatuses auflisten](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekte.|
|[termsAndConditionsAcceptanceStatus abrufen](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|Lesen von Eigenschaften und Beziehungen des [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekts.|
|[termsAndConditionsAcceptanceStatus erstellen](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|Erstellen eines neuen [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekts.|
|[termsAndConditionsAcceptanceStatus löschen](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|Keine|Löscht ein [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekt.|
|[termsAndConditionsAcceptanceStatus aktualisieren](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|Aktualisieren der Eigenschaften eines [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner der Entität|
|userDisplayName|String|Anzeigename des Benutzers, dessen Zustimmung die Entität darstellt|
|acceptedVersion|Int32|Die Versionsnummer der neuesten Version der Geschäftsbedingungen, die der Benutzer akzeptiert hat|
|acceptedDateTime|DateTimeOffset|Datum und Uhrzeit, zu der die Nutzungsbedingungen zuletzt vom Benutzer akzeptiert wurden.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|termsAndConditions|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Navigationslink zu den Geschäftsbedingungen, die zugewiesen werden.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)"
}
```




