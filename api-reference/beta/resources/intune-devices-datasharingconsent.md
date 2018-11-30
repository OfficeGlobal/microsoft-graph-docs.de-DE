---
title: Ressourcentyp dataSharingConsent
description: Datenfreigabe stimmen Informationen.
ms.openlocfilehash: 152b367161dc9a734a20e007ac1b2c0d02d0c99f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065920"
---
# <a name="datasharingconsent-resource-type"></a>Ressourcentyp dataSharingConsent

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Datenfreigabe stimmen Informationen.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste dataSharingConsents](../api/intune-devices-datasharingconsent-list.md)|[DataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Auflistung|Listeneigenschaften und Beziehungen der [DataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekte.|
|[Abrufen von dataSharingConsent](../api/intune-devices-datasharingconsent-get.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Lesen Sie Eigenschaften und Beziehungen des [DataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekts.|
|[Erstellen von dataSharingConsent](../api/intune-devices-datasharingconsent-create.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Erstellen eines neuen [DataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekts.|
|[DataSharingConsent löschen](../api/intune-devices-datasharingconsent-delete.md)|Keines|Löscht eine [DataSharingConsent](../resources/intune-devices-datasharingconsent.md).|
|[DataSharingConsent aktualisieren](../api/intune-devices-datasharingconsent-update.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Aktualisieren Sie die Eigenschaften eines [DataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekts.|
|[ConsentToDataSharing Aktion](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Die Daten sharing Zustimmung Id|
|von Ihnen eingegebene Dienstanzeigename|String|Der Anzeigename der Dienst Workflow|
|termsUrl|String|Die TermsUrl für die Datenfreigabe Zustimmung|
|erteilt|Boolesch|Den gewährten Status für die Datenfreigabe Zustimmung|
|grantDateTime|DateTimeOffset|Die Zeit Zustimmung wurde für dieses Konto erteilt.|
|grantedByUpn|String|Den Upn des Benutzers, der für dieses Konto Zustimmung eingeholt|
|grantedByUserId|String|Die Benutzer-ID des Benutzers, der für dieses Konto Zustimmung eingeholt|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSharingConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "String (identifier)",
  "serviceDisplayName": "String",
  "termsUrl": "String",
  "granted": true,
  "grantDateTime": "String (timestamp)",
  "grantedByUpn": "String",
  "grantedByUserId": "String"
}
```





