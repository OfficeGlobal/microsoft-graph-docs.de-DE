---
title: reportRoot-Ressourcentyp
description: Die Ressource, die eine Instanz der Verlaufsberichte darstellt.
author: tfitzmac
ms.openlocfilehash: 46b4844487a1cb714dde791e6867c277c1693f66
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303969"
---
# <a name="reportroot-resource-type"></a>reportRoot-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Ressource, die eine Instanz der Verlaufsberichte darstellt.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[reportRoot abrufen](../api/intune-shared-reportroot-get.md)|[reportRoot](../resources/intune-shared-reportroot.md)|Lesen von Eigenschaften und Beziehungen des [reportRoot](../resources/intune-shared-reportroot.md)-Objekts.|
|[reportRoot aktualisieren](../api/intune-shared-reportroot-update.md)|[reportRoot](../resources/intune-shared-reportroot.md)|Aktualisieren der Eigenschaften eines [reportRoot](../resources/intune-shared-reportroot.md)-Objekts.|
|**deviceConfiguration**|
|[deviceConfigurationDeviceActivity-Funktion](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|[report](../resources/intune-shared-report.md)|Metadaten für den Gerätekonfigurations-Geräteaktivitätsbericht|
|[deviceConfigurationUserActivity-Funktion](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|[report](../resources/intune-shared-report.md)|Metadaten für den Gerätekonfigurations-Benutzeraktivitätsbericht|
|**Problembehandlung**|
|[ManagedDeviceEnrollmentFailureDetails-Funktion](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|[report](../resources/intune-shared-report.md)|Noch nicht dokumentiert.|
|[ManagedDeviceEnrollmentTopFailures-Funktion](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|[report](../resources/intune-shared-report.md)|Noch nicht dokumentiert.|


## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Der eindeutige Bezeichner für die Entität.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```

## <a name="example"></a>Beispiel

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```