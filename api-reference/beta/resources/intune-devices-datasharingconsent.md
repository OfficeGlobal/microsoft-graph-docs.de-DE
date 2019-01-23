---
title: Ressourcentyp dataSharingConsent
description: Datenfreigabe stimmen Informationen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bf77a252c323ce83c2dcda44ac294161a4fd4747
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425694"
---
# <a name="datasharingconsent-resource-type"></a>Ressourcentyp dataSharingConsent

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Datenfreigabe stimmen Informationen.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste dataSharingConsents](../api/intune-devices-datasharingconsent-list.md)|[DataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Auflistung|Listeneigenschaften und Beziehungen der [DataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekte.|
|[Abrufen von dataSharingConsent](../api/intune-devices-datasharingconsent-get.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Lesen Sie Eigenschaften und Beziehungen des [DataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekts.|
|[Erstellen von dataSharingConsent](../api/intune-devices-datasharingconsent-create.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Erstellen eines neuen [DataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekts.|
|[DataSharingConsent löschen](../api/intune-devices-datasharingconsent-delete.md)|Keine|Löscht eine [DataSharingConsent](../resources/intune-devices-datasharingconsent.md).|
|[DataSharingConsent aktualisieren](../api/intune-devices-datasharingconsent-update.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Aktualisieren Sie die Eigenschaften eines [DataSharingConsent](../resources/intune-devices-datasharingconsent.md) -Objekts.|
|[ConsentToDataSharing Aktion](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Die Daten sharing Zustimmung Id|
|von Ihnen eingegebene Dienstanzeigename|Zeichenfolge|Der Anzeigename der Dienst Workflow|
|termsUrl|Zeichenfolge|Die TermsUrl für die Datenfreigabe Zustimmung|
|erteilt|Boolean|Den gewährten Status für die Datenfreigabe Zustimmung|
|grantDateTime|DateTimeOffset|Die Zeit Zustimmung wurde für dieses Konto erteilt.|
|grantedByUpn|Zeichenfolge|Den Upn des Benutzers, der für dieses Konto Zustimmung eingeholt|
|grantedByUserId|Zeichenfolge|Die Benutzer-ID des Benutzers, der für dieses Konto Zustimmung eingeholt|

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




