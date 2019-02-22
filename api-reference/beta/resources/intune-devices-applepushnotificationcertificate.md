---
title: applePushNotificationCertificate-Ressourcentyp
description: Apple Push Notification-Zertifikat.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c1bf303a3d0acee799819177bfca4b186a69ee3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154957"
---
# <a name="applepushnotificationcertificate-resource-type"></a>applePushNotificationCertificate-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Apple Push Notification-Zertifikat.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[applePushNotificationCertificate abrufen](../api/intune-devices-applepushnotificationcertificate-get.md)|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Lesen von Eigenschaften und Beziehungen des [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)-Objekts.|
|[applePushNotificationCertificate aktualisieren](../api/intune-devices-applepushnotificationcertificate-update.md)|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Aktualisieren der Eigenschaften eines [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)-Objekts.|
|[downloadApplePushNotificationCertificateSigningRequest-Funktion](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|Zeichenfolge|Signieranforderung für Apple Push Notification-Zertifikat herunterladen|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner für das Zertifikat|
|appleIdentifier|Zeichenfolge|Apple-ID des Kontos, mit dem das MDM-Push-Zertifikat erstellt wurde|
|topicIdentifier|String|Thema-ID|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Apple Push Notification-Zertifikats|
|expirationDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs des Apple Push Notification-Zertifikats|
|certificateUploadStatus|Zeichenfolge|Der Zertifikat Uploadstatus.|
|certificateUploadFailureReason|Zeichenfolge|Der Grund, warum der Zertifikat Upload fehlgeschlagen ist.|
|certificate|Zeichenfolge|Noch nicht dokumentiert.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificateUploadStatus": "String",
  "certificateUploadFailureReason": "String",
  "certificate": "String"
}
```




