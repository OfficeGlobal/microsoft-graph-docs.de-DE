---
title: vppToken-Ressourcentyp
description: Sie erwerben mehrere Lizenzen für iOS-Apps über das Apple Volume Purchase Program for Business oder Education. Dies umfasst das Einrichten eines Apple VPP-Kontos auf der Apple-Website und das Hochladen des Apple VPP Business- oder Education-Tokens in Intune. Dann können Sie Ihre Volumenlizenzierungsinformationen mit Intune synchronisieren und die volumenlizenzierte App-Nutzung nachverfolgen. Sie können mehrere Apple VPP Business- oder Education-Token hochladen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a21ac5a85094692fe52c7817ee31636c872e131e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419877"
---
# <a name="vpptoken-resource-type"></a>vppToken-Ressourcentyp

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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
|[RevokeLicenses Aktion](../api/intune-onboarding-vpptoken-revokelicenses.md)|Keine|REVOKE-Lizenzen, die mit einer bestimmten AppleVolumePurchaseProgramToken verknüpft ist|
|[GetLicensesForApp-Funktion](../api/intune-onboarding-vpptoken-getlicensesforapp.md)|[VppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) -Auflistung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Wird automatisch generiert, wenn AppleVolumePurchaseProgramToken erstellt wird. Schlüssel der Entität.|
|organizationName|String|Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune-shared-vpptokenaccounttype.md)|Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist. Mögliche Werte sind: `business` und `education`. Mögliche Werte sind: `business` und `education`.|
|appleId|String|Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist.|
|expirationDateTime|DateTimeOffset|Ablaufdatum und -uhrzeit des Apple Volume Purchase Program-Token.|
|lastSyncDateTime|DateTimeOffset|Zeitpunkt der letzten Synchronisierung der Anwendung mit dem Apple Volume Purchase Program Service mithilfe des Apple Volume Purchase Program-Token.|
|token|String|Aus dem Apple Volume Purchase Program heruntergeladene Zeichenfolge des Apple Volume Purchase Program-Token.|
|lastModifiedDateTime|DateTimeOffset|Letztes Änderungsdatum und letzter Änderungszeitpunkt des Apple Volume Purchase Program-Token.|
|state|[vppTokenState](../resources/intune-onboarding-vpptokenstate.md)|Aktueller Stand des Apple Volume Purchase Program-Token. Mögliche Werte sind: `unknown`, `valid`, `expired`, `invalid` und `assignedToExternalMDM`. Mögliche Werte sind: `unknown`, `valid`, `expired`, `invalid` und `assignedToExternalMDM`.|
|tokenActionResults|[VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) -Auflistung|Die Auflistung der Status der Aktionen, die auf Apple Volume Purchase Programm Token ausgeführt werden.|
|lastSyncStatus|[vppTokenSyncStatus](../resources/intune-onboarding-vpptokensyncstatus.md)|Aktueller Synchronisierungsstatus seit der letzten Synchronisierung der Anwendung, die mit dem Apple Volume Purchase Program-Token durchgeführt wurde. Mögliche Werte sind: `none`, `inProgress`, `completed`, `failed`. Mögliche Werte sind: `none`, `inProgress`, `completed`, `failed`.|
|automaticallyUpdateApps|Boolean|Angabe, ob Anwendungen für das VPP-Token automatisch aktualisiert werden.|
|countryOrRegion|String|Angabe, ob Anwendungen für das VPP-Token automatisch aktualisiert werden.|
|dataSharingConsentGranted|Boolean|Stimmen Sie für Datenfreigaben über die Apple Volume Purchase Program gewährt.|
|displayName|Zeichenfolge|Ein Administrator angegebene token Anzeigenamen.|
|locationName|Zeichenfolge|Token Speicherort von Apple VPP zurückgegeben.|
|claimTokenManagementFromExternalMdm|Boolean|Admin stimmen ausgibt token Management von externen MDM zulassen|
|roleScopeTagIds|Zeichenfolgenauflistung|Rolle Bereichs Tags-IDs zu dieser Entität zugewiesen.|

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




