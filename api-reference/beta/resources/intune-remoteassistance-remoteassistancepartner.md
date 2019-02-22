---
title: remoteAssistancePartner-Ressourcentyp
description: Die Ressource remoteAssistPartner repräsentiert die Metadaten und den Status eines bestimmten Partnerdienstes für die Remoteunterstützung.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c09965131e7c1d053f12aad9c7e0c8304ea42cd6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158863"
---
# <a name="remoteassistancepartner-resource-type"></a>remoteAssistancePartner-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die Ressource remoteAssistPartner repräsentiert die Metadaten und den Status eines bestimmten Partnerdienstes für die Remoteunterstützung.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[remoteAssistancePartners auflisten](../api/intune-remoteassistance-remoteassistancepartner-list.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekte.|
|[remoteAssistancePartner abrufen](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Lesen von Eigenschaften und Beziehungen des [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekts.|
|[remoteAssistancePartner erstellen](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Erstellen eines neuen [RemoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekts.|
|[remoteAssistancePartner löschen](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|Keine|Löschen eines [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[remoteAssistancePartner aktualisieren](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Aktualisieren der Eigenschaften eines [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekts.|
|[beginOnboarding-Aktion](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|Keiner|Noch nicht dokumentiert.|
|[disconnect-Aktion](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Der eindeutige Bezeichner des Partners.|
|displayName|Zeichenfolge|Der Anzeigename des Partners.|
|onboardingUrl|Zeichenfolge|Die URL des Onboarding-Portals des Partners, in dem ein Administrator den Remoteunterstützungsdienst konfigurieren kann.|
|onboardingStatus|[remoteAssistanceOnboardingStatus](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|TBD. Mögliche Werte sind: `notOnboarded`, `onboarding` und `onboarded`.|
|lastConnectionDateTime|DateTimeOffset|Zeitstempel der letzten vom TEM-Partner an Intune gesendeten Anforderung|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistancePartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "String (identifier)",
  "displayName": "String",
  "onboardingUrl": "String",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "String (timestamp)"
}
```




