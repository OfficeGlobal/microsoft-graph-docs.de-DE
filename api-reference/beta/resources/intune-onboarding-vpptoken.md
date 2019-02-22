---
title: vppToken-Ressourcentyp
description: Sie erwerben mehrere Lizenzen für iOS-Apps über das Apple Volume Purchase Program for Business oder Education. Dies umfasst das Einrichten eines Apple VPP-Kontos auf der Apple-Website und das Hochladen des Apple VPP Business- oder Education-Tokens in Intune. Dann können Sie Ihre Volumenlizenzierungsinformationen mit Intune synchronisieren und die volumenlizenzierte App-Nutzung nachverfolgen. Sie können mehrere Apple VPP Business- oder Education-Token hochladen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f6f964c2d69da7dbb8407b33e5d9503e9a8ac49e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158450"
---
# <a name="vpptoken-resource-type"></a>vppToken-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

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
|[revokeLicenses-Aktion](../api/intune-onboarding-vpptoken-revokelicenses.md)|Keine|Widerrufen von Lizenzen, die einem bestimmten appleVolumePurchaseProgramToken zugeordnet sind|
|[getLicensesForApp-Funktion](../api/intune-onboarding-vpptoken-getlicensesforapp.md)|[vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) -Sammlung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Wird automatisch generiert, wenn AppleVolumePurchaseProgramToken erstellt wird. Schlüssel der Entität.|
|organizationName|Zeichenfolge|Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune-shared-vpptokenaccounttype.md)|Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist. Mögliche Werte sind: `business` und `education`. Mögliche Werte sind: `business` und `education`.|
|appleId|Zeichenfolge|Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist.|
|expirationDateTime|DateTimeOffset|Ablaufdatum und -uhrzeit des Apple Volume Purchase Program-Token.|
|lastSyncDateTime|DateTimeOffset|Zeitpunkt der letzten Synchronisierung der Anwendung mit dem Apple Volume Purchase Program Service mithilfe des Apple Volume Purchase Program-Token.|
|token|Zeichenfolge|Aus dem Apple Volume Purchase Program heruntergeladene Zeichenfolge des Apple Volume Purchase Program-Token.|
|lastModifiedDateTime|DateTimeOffset|Letztes Änderungsdatum und letzter Änderungszeitpunkt des Apple Volume Purchase Program-Token.|
|state|[vppTokenState](../resources/intune-onboarding-vpptokenstate.md)|Aktueller Stand des Apple Volume Purchase Program-Token. Mögliche Werte: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`. Mögliche Werte: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.|
|tokenActionResults|[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) -Sammlung|Die Sammlung von Status der Aktionen, die für das Apple Volume Purchase Program-Token ausgeführt wurden.|
|lastSyncStatus|[vppTokenSyncStatus](../resources/intune-onboarding-vpptokensyncstatus.md)|Aktueller Synchronisierungsstatus seit der letzten Synchronisierung der Anwendung, die mit dem Apple Volume Purchase Program-Token durchgeführt wurde. Mögliche Werte sind: `none`, `inProgress`, `completed`, `failed`. Mögliche Werte sind: `none`, `inProgress`, `completed`, `failed`.|
|automaticallyUpdateApps|Boolean|Angabe, ob Anwendungen für das VPP-Token automatisch aktualisiert werden.|
|countryOrRegion|String|Angabe, ob Anwendungen für das VPP-Token automatisch aktualisiert werden.|
|dataSharingConsentGranted|Boolescher Wert|Einwilligung zur Datenfreigabe mit dem Apple Volume Purchase-Programm.|
|displayName|Zeichenfolge|Ein vom Administrator angegebener, von Token angezeigter Name.|
|LocationName|Zeichenfolge|Von Apple VSS zurückgegebener Tokensort.|
|claimTokenManagementFromExternalMdm|Boolescher Wert|Zustimmung des Administrators, um die Forderungs Tokenverwaltung über externes MDM zu ermöglichen.|
|Rolescopetagids zur|String collection|Rollenbereichs Tags-IDs, die dieser Entität zugewiesen sind.|

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
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ],
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "String",
  "dataSharingConsentGranted": true,
  "displayName": "String",
  "locationName": "String",
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```




