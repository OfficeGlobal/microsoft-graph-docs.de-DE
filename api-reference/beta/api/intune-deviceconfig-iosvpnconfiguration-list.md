---
title: IosVpnConfigurations aufListen
description: AufListen von Eigenschaften und Beziehungen der iosVpnConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 72ab0720e2ce90e436fac66f7fb710f44e90aa2c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964948"
---
# <a name="list-iosvpnconfigurations"></a><span data-ttu-id="b0330-103">IosVpnConfigurations aufListen</span><span class="sxs-lookup"><span data-stu-id="b0330-103">List iosVpnConfigurations</span></span>

> <span data-ttu-id="b0330-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b0330-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0330-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b0330-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0330-106">AufListen von Eigenschaften und Beziehungen der [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="b0330-106">List properties and relationships of the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0330-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b0330-107">Prerequisites</span></span>
<span data-ttu-id="b0330-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0330-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0330-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b0330-110">Permission type</span></span>|<span data-ttu-id="b0330-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b0330-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0330-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b0330-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b0330-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0330-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b0330-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b0330-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0330-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b0330-115">Not supported.</span></span>|
|<span data-ttu-id="b0330-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b0330-116">Application</span></span>|<span data-ttu-id="b0330-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b0330-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0330-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0330-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b0330-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b0330-119">Request headers</span></span>
|<span data-ttu-id="b0330-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b0330-120">Header</span></span>|<span data-ttu-id="b0330-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b0330-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0330-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0330-122">Authorization</span></span>|<span data-ttu-id="b0330-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b0330-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0330-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b0330-124">Accept</span></span>|<span data-ttu-id="b0330-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b0330-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0330-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b0330-126">Request body</span></span>
<span data-ttu-id="b0330-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b0330-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0330-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0330-128">Response</span></span>
<span data-ttu-id="b0330-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b0330-129">If successful, this method returns a `200 OK` response code and a collection of [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0330-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b0330-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0330-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0330-131">Request</span></span>
<span data-ttu-id="b0330-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b0330-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="b0330-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0330-133">Response</span></span>
<span data-ttu-id="b0330-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b0330-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2547

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVpnConfiguration",
      "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "connectionName": "Connection Name value",
      "connectionType": "pulseSecure",
      "loginGroupOrDomain": "Login Group Or Domain value",
      "role": "Role value",
      "realm": "Realm value",
      "server": {
        "@odata.type": "microsoft.graph.vpnServer",
        "description": "Description value",
        "address": "Address value",
        "isDefaultServer": true
      },
      "identifier": "Identifier value",
      "customData": [
        {
          "@odata.type": "microsoft.graph.keyValue",
          "key": "Key value",
          "value": "Value value"
        }
      ],
      "customKeyValueData": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "enableSplitTunneling": true,
      "authenticationMethod": "usernameAndPassword",
      "enablePerApp": true,
      "safariDomains": [
        "Safari Domains value"
      ],
      "onDemandRules": [
        {
          "@odata.type": "microsoft.graph.vpnOnDemandRule",
          "ssids": [
            "Ssids value"
          ],
          "dnsSearchDomains": [
            "Dns Search Domains value"
          ],
          "probeUrl": "https://example.com/probeUrl/",
          "action": "evaluateConnection",
          "domainAction": "neverConnect",
          "domains": [
            "Domains value"
          ],
          "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
        }
      ],
      "proxyServer": {
        "@odata.type": "microsoft.graph.vpnProxyServer",
        "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
        "address": "Address value",
        "port": 4
      },
      "optInToDeviceIdSharing": true,
      "providerType": "appProxy",
      "userDomain": "User Domain value",
      "strictEnforcement": true,
      "cloudName": "Cloud Name value",
      "excludeList": [
        "Exclude List value"
      ]
    }
  ]
}
```




