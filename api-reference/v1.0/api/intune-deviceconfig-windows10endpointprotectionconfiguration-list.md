---
title: Auflisten von „windows10EndpointProtectionConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windows10EndpointProtectionConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0b59e4a5275d270016946e79cdf00e862a67f1e3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840936"
---
# <a name="list-windows10endpointprotectionconfigurations"></a><span data-ttu-id="790c2-103">Auflisten von „windows10EndpointProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="790c2-103">List windows10EndpointProtectionConfigurations</span></span>

> <span data-ttu-id="790c2-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="790c2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="790c2-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="790c2-105">List properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="790c2-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="790c2-106">Prerequisites</span></span>
<span data-ttu-id="790c2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="790c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="790c2-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="790c2-109">Permission type</span></span>|<span data-ttu-id="790c2-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="790c2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="790c2-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="790c2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="790c2-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="790c2-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="790c2-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="790c2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="790c2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="790c2-114">Not supported.</span></span>|
|<span data-ttu-id="790c2-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="790c2-115">Application</span></span>|<span data-ttu-id="790c2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="790c2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="790c2-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="790c2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="790c2-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="790c2-118">Request headers</span></span>
|<span data-ttu-id="790c2-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="790c2-119">Header</span></span>|<span data-ttu-id="790c2-120">Wert</span><span class="sxs-lookup"><span data-stu-id="790c2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="790c2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="790c2-121">Authorization</span></span>|<span data-ttu-id="790c2-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="790c2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="790c2-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="790c2-123">Accept</span></span>|<span data-ttu-id="790c2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="790c2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="790c2-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="790c2-125">Request body</span></span>
<span data-ttu-id="790c2-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="790c2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="790c2-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="790c2-127">Response</span></span>
<span data-ttu-id="790c2-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="790c2-128">If successful, this method returns a `200 OK` response code and a collection of [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="790c2-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="790c2-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="790c2-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="790c2-130">Request</span></span>
<span data-ttu-id="790c2-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="790c2-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="790c2-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="790c2-132">Response</span></span>
<span data-ttu-id="790c2-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="790c2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4834

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
      "id": "09709403-9403-0970-0394-700903947009",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "firewallBlockStatefulFTP": true,
      "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
      "firewallPreSharedKeyEncodingMethod": "none",
      "firewallIPSecExemptionsAllowNeighborDiscovery": true,
      "firewallIPSecExemptionsAllowICMP": true,
      "firewallIPSecExemptionsAllowRouterDiscovery": true,
      "firewallIPSecExemptionsAllowDHCP": true,
      "firewallCertificateRevocationListCheckMethod": "none",
      "firewallMergeKeyingModuleSettings": true,
      "firewallPacketQueueingMethod": "disabled",
      "firewallProfileDomain": {
        "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
        "firewallEnabled": "blocked",
        "stealthModeBlocked": true,
        "incomingTrafficBlocked": true,
        "unicastResponsesToMulticastBroadcastsBlocked": true,
        "inboundNotificationsBlocked": true,
        "authorizedApplicationRulesFromGroupPolicyMerged": true,
        "globalPortRulesFromGroupPolicyMerged": true,
        "connectionSecurityRulesFromGroupPolicyMerged": true,
        "outboundConnectionsBlocked": true,
        "inboundConnectionsBlocked": true,
        "securedPacketExemptionAllowed": true,
        "policyRulesFromGroupPolicyMerged": true
      },
      "firewallProfilePublic": {
        "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
        "firewallEnabled": "blocked",
        "stealthModeBlocked": true,
        "incomingTrafficBlocked": true,
        "unicastResponsesToMulticastBroadcastsBlocked": true,
        "inboundNotificationsBlocked": true,
        "authorizedApplicationRulesFromGroupPolicyMerged": true,
        "globalPortRulesFromGroupPolicyMerged": true,
        "connectionSecurityRulesFromGroupPolicyMerged": true,
        "outboundConnectionsBlocked": true,
        "inboundConnectionsBlocked": true,
        "securedPacketExemptionAllowed": true,
        "policyRulesFromGroupPolicyMerged": true
      },
      "firewallProfilePrivate": {
        "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
        "firewallEnabled": "blocked",
        "stealthModeBlocked": true,
        "incomingTrafficBlocked": true,
        "unicastResponsesToMulticastBroadcastsBlocked": true,
        "inboundNotificationsBlocked": true,
        "authorizedApplicationRulesFromGroupPolicyMerged": true,
        "globalPortRulesFromGroupPolicyMerged": true,
        "connectionSecurityRulesFromGroupPolicyMerged": true,
        "outboundConnectionsBlocked": true,
        "inboundConnectionsBlocked": true,
        "securedPacketExemptionAllowed": true,
        "policyRulesFromGroupPolicyMerged": true
      },
      "defenderAttackSurfaceReductionExcludedPaths": [
        "Defender Attack Surface Reduction Excluded Paths value"
      ],
      "defenderGuardedFoldersAllowedAppPaths": [
        "Defender Guarded Folders Allowed App Paths value"
      ],
      "defenderAdditionalGuardedFolders": [
        "Defender Additional Guarded Folders value"
      ],
      "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
      "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
      "defenderSecurityCenterBlockExploitProtectionOverride": true,
      "appLockerApplicationControl": "enforceComponentsAndStoreApps",
      "smartScreenEnableInShell": true,
      "smartScreenBlockOverrideForFiles": true,
      "applicationGuardEnabled": true,
      "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
      "applicationGuardBlockNonEnterpriseContent": true,
      "applicationGuardAllowPersistence": true,
      "applicationGuardForceAuditing": true,
      "applicationGuardBlockClipboardSharing": "blockBoth",
      "applicationGuardAllowPrintToPDF": true,
      "applicationGuardAllowPrintToXPS": true,
      "applicationGuardAllowPrintToLocalPrinters": true,
      "applicationGuardAllowPrintToNetworkPrinters": true,
      "bitLockerDisableWarningForOtherDiskEncryption": true,
      "bitLockerEnableStorageCardEncryptionOnMobile": true,
      "bitLockerEncryptDevice": true,
      "bitLockerRemovableDrivePolicy": {
        "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
        "encryptionMethod": "aesCbc256",
        "requireEncryptionForWriteAccess": true,
        "blockCrossOrganizationWriteAccess": true
      }
    }
  ]
}
```



