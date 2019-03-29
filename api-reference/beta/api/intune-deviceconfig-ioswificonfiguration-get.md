---
title: IosWiFiConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des iosWiFiConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 98cdcabd389c98d9a339d0c647600e913375c481
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975700"
---
# <a name="get-ioswificonfiguration"></a><span data-ttu-id="e589b-103">IosWiFiConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="e589b-103">Get iosWiFiConfiguration</span></span>

> <span data-ttu-id="e589b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e589b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e589b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e589b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e589b-106">Lesen von Eigenschaften und Beziehungen des [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e589b-106">Read properties and relationships of the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e589b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e589b-107">Prerequisites</span></span>
<span data-ttu-id="e589b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e589b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e589b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e589b-110">Permission type</span></span>|<span data-ttu-id="e589b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e589b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e589b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e589b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e589b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e589b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e589b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e589b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e589b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e589b-115">Not supported.</span></span>|
|<span data-ttu-id="e589b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e589b-116">Application</span></span>|<span data-ttu-id="e589b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e589b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e589b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e589b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e589b-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e589b-119">Optional query parameters</span></span>
<span data-ttu-id="e589b-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e589b-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e589b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e589b-121">Request headers</span></span>
|<span data-ttu-id="e589b-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e589b-122">Header</span></span>|<span data-ttu-id="e589b-123">Wert</span><span class="sxs-lookup"><span data-stu-id="e589b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e589b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e589b-124">Authorization</span></span>|<span data-ttu-id="e589b-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e589b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e589b-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e589b-126">Accept</span></span>|<span data-ttu-id="e589b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e589b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e589b-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e589b-128">Request body</span></span>
<span data-ttu-id="e589b-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e589b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e589b-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="e589b-130">Response</span></span>
<span data-ttu-id="e589b-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e589b-131">If successful, this method returns a `200 OK` response code and [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e589b-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e589b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e589b-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e589b-133">Request</span></span>
<span data-ttu-id="e589b-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e589b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e589b-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="e589b-135">Response</span></span>
<span data-ttu-id="e589b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e589b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 908

{
  "value": {
    "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
    "id": "516f9ef9-9ef9-516f-f99e-6f51f99e6f51",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "networkName": "Network Name value",
    "ssid": "Ssid value",
    "connectAutomatically": true,
    "connectWhenNetworkNameIsHidden": true,
    "wiFiSecurityType": "wpaPersonal",
    "proxySettings": "manual",
    "proxyManualAddress": "Proxy Manual Address value",
    "proxyManualPort": 15,
    "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
    "preSharedKey": "Pre Shared Key value"
  }
}
```




