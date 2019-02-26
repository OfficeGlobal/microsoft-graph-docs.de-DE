---
title: dataSharingConsent-Ressourcentyp
description: Einwilligungs Informationen zur Datenfreigabe.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75ef8b899c6fa7645b31cd77ada7420b0f753a60
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174650"
---
# <a name="datasharingconsent-resource-type"></a>dataSharingConsent-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Einwilligungs Informationen zur Datenfreigabe.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DataSharingConsents aufListen](../api/intune-devices-datasharingconsent-list.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekte.|
|[DataSharingConsent abrufen](../api/intune-devices-datasharingconsent-get.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Lesen von Eigenschaften und Beziehungen des [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekts.|
|[DataSharingConsent erstellen](../api/intune-devices-datasharingconsent-create.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Erstellen eines neuen [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekts.|
|[DataSharingConsent löschen](../api/intune-devices-datasharingconsent-delete.md)|Keine|Löscht eine [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).|
|[DataSharingConsent aktualisieren](../api/intune-devices-datasharingconsent-update.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Aktualisieren der Eigenschaften eines [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekts.|
|[consentToDataSharing-Aktion](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Die Einwilligungs-ID für die Datenfreigabe|
|serviceDisplayName|Zeichenfolge|Der Anzeigename des Dienst-Arbeitsflusses|
|termsUrl|Zeichenfolge|Die TermsUrl für die Einwilligung zur Datenfreigabe|
|granted|Boolean|Der erteilte Status für die Einwilligung zur Datenfreigabe|
|grantDateTime|DateTimeOffset|Die Zeit Genehmigung für dieses Konto wurde erteilt.|
|grantedByUpn|Zeichenfolge|Der UPN des Benutzers, der die Einwilligung für dieses Konto erteilt hat.|
|grantedByUserId|Zeichenfolge|Die UserId des Benutzers, der die Einwilligung für dieses Konto erteilt hat|

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




