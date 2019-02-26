---
title: mobileAppContentFile-Ressourcentyp
description: Enthält Eigenschaften für eine einzelne Installationsdatei, die mit einer bestimmten mobileAppContent-Version verknüpft ist.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f8edeebdc3df12d3e1a458ae57e805052e47e3d8
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262293"
---
# <a name="mobileappcontentfile-resource-type"></a>mobileAppContentFile-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften für eine einzelne Installationsdatei, die mit einer bestimmten mobileAppContent-Version verknüpft ist.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[MobileAppContentFiles auflisten](../api/intune-apps-mobileappcontentfile-list.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)-Objekte.|
|[MobileAppContentFile abrufen](../api/intune-apps-mobileappcontentfile-get.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|Lesen von Eigenschaften und Beziehungen des [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)-Objekts.|
|[MobileAppContentFile erstellen](../api/intune-apps-mobileappcontentfile-create.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|Erstellen eines neuen [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)-Objekts.|
|[MobileAppContentFile löschen](../api/intune-apps-mobileappcontentfile-delete.md)|Keine|Löscht ein [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)-Objekt.|
|[MobileAppContentFile aktualisieren](../api/intune-apps-mobileappcontentfile-update.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|Aktualisieren der Eigenschaften eines [MobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)-Objekts.|
|[commit-Aktion](../api/intune-apps-mobileappcontentfile-commit.md)|Keine|Führt einen Commit für eine Datei einer bestimmten App aus.|
|[renewUpload-Aktion](../api/intune-apps-mobileappcontentfile-renewupload.md)|Keine|Erneuert den SAS-URI für einen Anwendungsdateiupload.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|azureStorageUri|String|Azure Storage-URI|
|isCommitted|Boolean|Wert, der angibt, ob für die Datei ein Commit ausgeführt wurde|
|id|Zeichenfolge|ID der Datei|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der Datei|
|name|Zeichenfolge|Name der Datei|
|size|Int64|Größe der Datei vor der Verschlüsselung|
|sizeEncrypted|Int64|Größe der Datei nach der Verschlüsselung|
|azureStorageUriExpirationDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs des Azure Storage-URI|
|manifest|Binär|Manifestinformationen|
|uploadState|[mobileAppContentFileUploadState](../resources/intune-apps-mobileappcontentfileuploadstate.md)|Status der aktuellen Uploadanforderung. Mögliche Werte sind: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContentFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "String",
  "isCommitted": true,
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "name": "String",
  "size": 1024,
  "sizeEncrypted": 1024,
  "azureStorageUriExpirationDateTime": "String (timestamp)",
  "manifest": "binary",
  "uploadState": "String"
}
```



