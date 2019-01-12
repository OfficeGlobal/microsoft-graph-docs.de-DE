---
title: applePushNotificationCertificate-Ressourcentyp
description: Apple Push Notification-Zertifikat.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9c8d968e48b1aa5e02c554dc8a5392165f0a3f9e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917734"
---
# <a name="applepushnotificationcertificate-resource-type"></a>applePushNotificationCertificate-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Apple Push Notification-Zertifikat.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[applePushNotificationCertificate abrufen](../api/intune-devices-applepushnotificationcertificate-get.md)|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Lesen von Eigenschaften und Beziehungen des [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)-Objekts.|
|[applePushNotificationCertificate aktualisieren](../api/intune-devices-applepushnotificationcertificate-update.md)|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Aktualisieren der Eigenschaften eines [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)-Objekts.|
|[downloadApplePushNotificationCertificateSigningRequest-Funktion](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|String|Signieranforderung für Apple Push Notification-Zertifikat herunterladen|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für das Zertifikat|
|appleIdentifier|String|Apple-ID des Kontos, mit dem das MDM-Push-Zertifikat erstellt wurde|
|topicIdentifier|String|Thema-ID|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Apple Push Notification-Zertifikats|
|expirationDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs des Apple Push Notification-Zertifikats|
|certificateUploadStatus|Zeichenfolge|Der Status des Zertifikats hochladen.|
|certificateUploadFailureReason|Zeichenfolge|Der Grund dafür ist das Zertifikat Upload ist fehlgeschlagen.|
|certificate|String|Noch nicht dokumentiert.|

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





