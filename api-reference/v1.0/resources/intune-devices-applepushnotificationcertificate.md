---
title: applePushNotificationCertificate-Ressourcentyp
description: Apple Push Notification-Zertifikat.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 43a697feaab14589540747ff0f4f79ca194918ef
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856842"
---
# <a name="applepushnotificationcertificate-resource-type"></a>applePushNotificationCertificate-Ressourcentyp

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
  "certificate": "String"
}
```



