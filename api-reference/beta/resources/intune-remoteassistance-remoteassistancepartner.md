---
title: remoteAssistancePartner-Ressourcentyp
description: Die Ressource remoteAssistPartner repräsentiert die Metadaten und den Status eines bestimmten Partnerdienstes für die Remoteunterstützung.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 52badd2ad146f23fba70ab545a459b124e7fae2c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821714"
---
# <a name="remoteassistancepartner-resource-type"></a>remoteAssistancePartner-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Ressource remoteAssistPartner repräsentiert die Metadaten und den Status eines bestimmten Partnerdienstes für die Remoteunterstützung.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[remoteAssistancePartners auflisten](../api/intune-remoteassistance-remoteassistancepartner-list.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekte.|
|[remoteAssistancePartner abrufen](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Lesen von Eigenschaften und Beziehungen des [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekts.|
|[remoteAssistancePartner erstellen](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Erstellen eines neuen [RemoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekts.|
|[remoteAssistancePartner löschen](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|Keine|Löschen eines [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[remoteAssistancePartner aktualisieren](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Aktualisieren der Eigenschaften eines [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)-Objekts.|
|[beginOnboarding-Aktion](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|Keine|Noch nicht dokumentiert.|
|[disconnect-Aktion](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Der eindeutige Bezeichner des Partners.|
|displayName|String|Der Anzeigename des Partners.|
|onboardingUrl|String|Die URL des Onboarding-Portals des Partners, in dem ein Administrator den Remoteunterstützungsdienst konfigurieren kann.|
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





