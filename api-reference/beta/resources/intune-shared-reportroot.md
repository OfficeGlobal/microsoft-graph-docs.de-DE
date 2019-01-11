---
title: reportRoot-Ressourcentyp
description: Die Ressource, die eine Instanz eines Geräts oder zur Problembehandlung Bericht, je nach Kontext darstellt.
localization_priority: Normal
ms.openlocfilehash: 8a2c1cbc666698eea7f466c32bae6c404264f545
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809646"
---
# <a name="reportroot-resource-type"></a>reportRoot-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Ressource, die eine Instanz eines Geräts oder zur Problembehandlung Bericht, je nach Kontext darstellt.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[reportRoot abrufen](../api/intune-shared-reportroot-get.md)|Lesen von Eigenschaften und Beziehungen des [reportRoot](../resources/intune-shared-reportroot.md)-Objekts.|
|[reportRoot aktualisieren](../api/intune-shared-reportroot-update.md)|Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [reportRoot](../resources/intune-shared-reportroot.md).|
|**deviceConfiguration**|
|[deviceConfigurationUserActivity-Funktion](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|Metadaten für den Gerätekonfigurations-Benutzeraktivitätsbericht|
|[deviceConfigurationDeviceActivity-Funktion](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|Metadaten für den Gerätekonfigurations-Geräteaktivitätsbericht|
|**Problembehandlung**|
|[ManagedDeviceEnrollmentAbandonmentDetails-Funktion](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[report](../resources/intune-shared-report.md)|Metadaten für die Registrierung Aufgabe Detailbericht|
|[ManagedDeviceEnrollmentAbandonmentSummary-Funktion](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[report](../resources/intune-shared-report.md)|Metadaten für die Registrierung Aufgabe Zusammenfassungsbericht|
|[ManagedDeviceEnrollmentFailureDetails-Funktion](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|Noch nicht dokumentiert|
|[ManagedDeviceEnrollmentFailureTrends-Funktion](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|Metadaten für die Registrierung Trends Fehlerbericht|
|[ManagedDeviceEnrollmentTopFailures-Funktion](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Der eindeutige Bezeichner für die Entität.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```



