---
title: reportRoot-Ressourcentyp
description: Die Ressource, die eine Instanz eines Geräts oder zur Problembehandlung Bericht, je nach Kontext darstellt.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 378f1758773bfcffda5d9039d3b60d4ac4bd5cc5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421333"
---
# <a name="reportroot-resource-type"></a>reportRoot-Ressourcentyp

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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



