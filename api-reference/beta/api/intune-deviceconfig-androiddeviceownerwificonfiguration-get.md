---
title: Abrufen von androidDeviceOwnerWiFiConfiguration
description: Lesen Sie Eigenschaften und Beziehungen des AndroidDeviceOwnerWiFiConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: 040fc0223fa1a6922013c2ec747f3ac9cd87c769
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354985"
---
# <a name="get-androiddeviceownerwificonfiguration"></a><span data-ttu-id="f1751-103">Abrufen von androidDeviceOwnerWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1751-103">Get androidDeviceOwnerWiFiConfiguration</span></span>

> <span data-ttu-id="f1751-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f1751-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1751-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f1751-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1751-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f1751-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1751-107">Lesen Sie Eigenschaften und Beziehungen des [AndroidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f1751-107">Read properties and relationships of the [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1751-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f1751-108">Prerequisites</span></span>
<span data-ttu-id="f1751-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1751-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1751-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f1751-111">Permission type</span></span>|<span data-ttu-id="f1751-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f1751-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1751-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f1751-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1751-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1751-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f1751-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f1751-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1751-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1751-116">Not supported.</span></span>|
|<span data-ttu-id="f1751-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f1751-117">Application</span></span>|<span data-ttu-id="f1751-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1751-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1751-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1751-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f1751-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f1751-120">Optional query parameters</span></span>
<span data-ttu-id="f1751-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f1751-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f1751-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f1751-122">Request headers</span></span>
|<span data-ttu-id="f1751-123">Header</span><span class="sxs-lookup"><span data-stu-id="f1751-123">Header</span></span>|<span data-ttu-id="f1751-124">Wert</span><span class="sxs-lookup"><span data-stu-id="f1751-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1751-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f1751-125">Authorization</span></span>|<span data-ttu-id="f1751-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f1751-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1751-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f1751-127">Accept</span></span>|<span data-ttu-id="f1751-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f1751-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1751-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f1751-129">Request body</span></span>
<span data-ttu-id="f1751-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f1751-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1751-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1751-131">Response</span></span>
<span data-ttu-id="f1751-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [AndroidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f1751-132">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1751-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f1751-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1751-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1751-134">Request</span></span>
<span data-ttu-id="f1751-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f1751-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f1751-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1751-136">Response</span></span>
<span data-ttu-id="f1751-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1751-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 736

{
  "value": {
    "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
    "id": "8d25beba-beba-8d25-babe-258dbabe258d",
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
    "wiFiSecurityType": "wep",
    "preSharedKey": "Pre Shared Key value",
    "preSharedKeyIsSet": true
  }
}
```





