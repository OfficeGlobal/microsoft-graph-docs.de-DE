---
title: Aktualisieren von „deviceManagement“
description: Aktualisieren der Eigenschaften eines deviceManagement-Objekts.
author: tfitzmac
ms.openlocfilehash: 1808c18fd5e305871e0be2e47def97938384488c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323765"
---
# <a name="update-devicemanagement"></a>Aktualisieren von „deviceManagement“

> **Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune-shared-devicemanagement.md)-Objekts.

## <a name="prerequisites"></a>Voraussetzungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

Beachten Sie, dass die Berechtigung abhängig vom Workflow variieren.

| Berechtigung&nbsp;Typ&nbsp;(durch&nbsp;Workflow) | Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten) |
|:---|:---|
| Delegiert (Geschäfts-, Schul- oder Unikonto) ||
| &nbsp;&nbsp; **Für die Arbeit android** | DeviceManagementConfiguration.ReadWrite.All  |
| &nbsp; &nbsp; **Überwachung** | DeviceManagementApps.ReadWrite.All |
| &nbsp;&nbsp; **Unternehmen Begriffe** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Gerätekonfiguration** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp; &nbsp; **Geräteverwaltung** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; **Elektronische SIM** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp; &nbsp; **Registrierung** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Zauns** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp; **Benachrichtigung** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Onboarding** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Role-based Access Control (RBAC)** | DeviceManagementRBAC.ReadWrite.All |
| &nbsp;&nbsp; **Remotezugriff** | DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **Remoteunterstützung** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Telekommunikation Ausgaben Management** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Erleichterung** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; **Windows Information Protection** | DeviceManagementApps.ReadWrite.All |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt|
| Anwendung | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a>Anforderungsheader

|Header|Wert|
|:---|:---|
|Autorisierung|Bearer&lt;token&gt; erforderlich|
|Accept|application/json|

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) an.

In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für das Gerät.|
|**deviceConfiguration**|
|intuneAccountId|GUID|Intune Konto-ID für die angegebenen Mandanten|
|legacyPcManangementEnabled|Boolesch|Die Eigenschaft zum Aktivieren von nicht-MDM verwaltet legacy PC-Verwaltung für dieses Konto. Diese Eigenschaft ist schreibgeschützt.|
|maximumDepTokens|Int32|Maximal zulässige Anzahl von DEP Token pro Mandant.|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Einstellungen auf Kontoebene|
|**deviceManagement**|
|accountMoveCompletionDateTime|DateTimeOffset|Datum & Zeit bei Mandantendaten zwischen Scaleunits verschoben.|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|Informationen zum Unternehmensadministrator Zustimmung.|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)|Gerät Protection Overview.|
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)|Cleanup-Regel|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|Status des Abonnements bei der Lösung für Mobilgeräteverwaltung des Mandanten. Mögliche Werte sind: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked` und `lockedOut`.|
|Abonnements|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|Mandanten-Abonnement. Mögliche Werte sind: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU` und `intune_SMB`.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Übersicht über die Malware für Windows-Geräte.|
|**Onboarding**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|„intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.|

Anforderung Body-Eigenschaft Unterstützung variiert je nach Workflow.

## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung

Es folgt ein Beispiel für eine Anforderung nach des Geräts-Workflows:

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```

### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort. 

Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Zurückgegebene Eigenschaften variieren je nach Workflow und Kontext.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```



