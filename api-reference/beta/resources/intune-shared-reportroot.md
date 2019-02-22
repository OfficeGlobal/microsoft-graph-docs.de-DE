---
title: reportRoot-Ressourcentyp
description: Die Ressource, die eine Instanz eines Geräts oder Problem Behandlungs Berichts darstellt, je nach Kontext.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: a2e41d9b17ca7acafa98dad65db5d2ff5ce30925
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151296"
---
# <a name="reportroot-resource-type"></a>reportRoot-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die Ressource, die eine Instanz eines Geräts oder Problem Behandlungs Berichts darstellt, je nach Kontext.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[reportRoot abrufen](../api/intune-shared-reportroot-get.md)|Lesen von Eigenschaften und Beziehungen des [reportRoot](../resources/intune-shared-reportroot.md)-Objekts.|
|[reportRoot aktualisieren](../api/intune-shared-reportroot-update.md)|Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [reportRoot](../resources/intune-shared-reportroot.md).|
|**deviceConfiguration**|
|[deviceConfigurationUserActivity-Funktion](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|Metadaten für den Gerätekonfigurations-Benutzeraktivitätsbericht|
|[deviceConfigurationDeviceActivity-Funktion](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|Metadaten für den Gerätekonfigurations-Geräteaktivitätsbericht|
|**Problembehandlung**|
|[managedDeviceEnrollmentAbandonmentDetails-Funktion](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[report](../resources/intune-shared-report.md)|Metadaten für den Bericht über Registrierungs Verzichts Details|
|[managedDeviceEnrollmentAbandonmentSummary-Funktion](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[report](../resources/intune-shared-report.md)|Zusammenfassungsbericht zu Metadaten für die Registrierung|
|[managedDeviceEnrollmentFailureDetails-Funktion](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|Noch nicht dokumentiert|
|[managedDeviceEnrollmentFailureTrends-Funktion](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|Metadaten für den Bericht über Registrierungs Fehlermeldungen|
|[managedDeviceEnrollmentTopFailures-Funktion](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|Noch nicht dokumentiert|

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



