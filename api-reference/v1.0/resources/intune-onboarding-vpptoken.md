---
title: vppToken-Ressourcentyp
description: Sie erwerben mehrere Lizenzen für iOS-Apps über das Apple Volume Purchase Program for Business oder Education. Dies umfasst das Einrichten eines Apple VPP-Kontos auf der Apple-Website und das Hochladen des Apple VPP Business- oder Education-Tokens in Intune. Dann können Sie Ihre Volumenlizenzierungsinformationen mit Intune synchronisieren und die volumenlizenzierte App-Nutzung nachverfolgen. Sie können mehrere Apple VPP Business- oder Education-Token hochladen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b14a66254d08f365f44e0e4ba1b1d58cdaf80c05
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254807"
---
# <a name="vpptoken-resource-type"></a>vppToken-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Sie erwerben mehrere Lizenzen für iOS-Apps über das Apple Volume Purchase Program for Business oder Education. Dies umfasst das Einrichten eines Apple VPP-Kontos auf der Apple-Website und das Hochladen des Apple VPP Business- oder Education-Tokens in Intune. Dann können Sie Ihre Volumenlizenzierungsinformationen mit Intune synchronisieren und die volumenlizenzierte App-Nutzung nachverfolgen. Sie können mehrere Apple VPP Business- oder Education-Token hochladen.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[VppTokens auflisten](../api/intune-onboarding-vpptoken-list.md)|[VppToken](../resources/intune-onboarding-vpptoken.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [vppToken](../resources/intune-onboarding-vpptoken.md)-Objekte.|
|[VppToken abrufen](../api/intune-onboarding-vpptoken-get.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|Lesen von Eigenschaften und Beziehungen des [vppToken](../resources/intune-onboarding-vpptoken.md)-Objekts.|
|[VppToken erstellen](../api/intune-onboarding-vpptoken-create.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|Erstellen eines neuen [vppToken](../resources/intune-onboarding-vpptoken.md)-Objekts.|
|[VppToken löschen](../api/intune-onboarding-vpptoken-delete.md)|Keine|Löscht ein [vppToken](../resources/intune-onboarding-vpptoken.md).|
|[VppToken aktualisieren](../api/intune-onboarding-vpptoken-update.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|Aktualisieren der Eigenschaften eines [vppToken](../resources/intune-onboarding-vpptoken.md)-Objekts.|
|[syncLicenses-Aktion](../api/intune-onboarding-vpptoken-synclicenses.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|Synchronisiert Lizenzen, die einem bestimmten appleVolumePurchaseProgramToken zugeordnet sind|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Wird automatisch generiert, wenn AppleVolumePurchaseProgramToken erstellt wird. Schlüssel der Entität.|
|organizationName|Zeichenfolge|Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune-shared-vpptokenaccounttype.md)|Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist. Mögliche Werte sind: `business` und `education`. Mögliche Werte sind: `business` und `education`.|
|appleId|Zeichenfolge|Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist.|
|expirationDateTime|DateTimeOffset|Ablaufdatum und -uhrzeit des Apple Volume Purchase Program-Token.|
|lastSyncDateTime|DateTimeOffset|Zeitpunkt der letzten Synchronisierung der Anwendung mit dem Apple Volume Purchase Program Service mithilfe des Apple Volume Purchase Program-Token.|
|token|Zeichenfolge|Aus dem Apple Volume Purchase Program heruntergeladene Zeichenfolge des Apple Volume Purchase Program-Token.|
|lastModifiedDateTime|DateTimeOffset|Letztes Änderungsdatum und letzter Änderungszeitpunkt des Apple Volume Purchase Program-Token.|
|state|[vppTokenState](../resources/intune-onboarding-vpptokenstate.md)|Aktueller Stand des Apple Volume Purchase Program-Token. Mögliche Werte: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`. Mögliche Werte: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.|
|lastSyncStatus|[vppTokenSyncStatus](../resources/intune-onboarding-vpptokensyncstatus.md)|Aktueller Synchronisierungsstatus seit der letzten Synchronisierung der Anwendung, die mit dem Apple Volume Purchase Program-Token durchgeführt wurde. Mögliche Werte sind: `none`, `inProgress`, `completed`, `failed`. Mögliche Werte sind: `none`, `inProgress`, `completed`, `failed`.|
|automaticallyUpdateApps|Boolean|Angabe, ob Anwendungen für das VPP-Token automatisch aktualisiert werden.|
|countryOrRegion|String|Gibt an, ob Apps für das VPP-Token automatisch aktualisiert werden.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vppToken"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "String (identifier)",
  "organizationName": "String",
  "vppTokenAccountType": "String",
  "appleId": "String",
  "expirationDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "token": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "String"
}
```



