---
title: Abrufen von androidWorkProfileWiFiConfiguration
description: Lesen Sie Eigenschaften und Beziehungen des AndroidWorkProfileWiFiConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 237bbdd5b5075d8ea50ad525745625dab76821ec
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418477"
---
# <a name="get-androidworkprofilewificonfiguration"></a><span data-ttu-id="0f881-103">Abrufen von androidWorkProfileWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f881-103">Get androidWorkProfileWiFiConfiguration</span></span>

> <span data-ttu-id="0f881-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0f881-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0f881-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0f881-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f881-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0f881-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f881-107">Lesen Sie Eigenschaften und Beziehungen des [AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0f881-107">Read properties and relationships of the [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f881-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0f881-108">Prerequisites</span></span>
<span data-ttu-id="0f881-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0f881-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0f881-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0f881-111">Permission type</span></span>|<span data-ttu-id="0f881-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0f881-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f881-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0f881-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f881-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f881-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0f881-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0f881-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f881-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f881-116">Not supported.</span></span>|
|<span data-ttu-id="0f881-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0f881-117">Application</span></span>|<span data-ttu-id="0f881-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f881-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f881-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f881-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0f881-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0f881-120">Optional query parameters</span></span>
<span data-ttu-id="0f881-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0f881-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f881-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0f881-122">Request headers</span></span>
|<span data-ttu-id="0f881-123">Header</span><span class="sxs-lookup"><span data-stu-id="0f881-123">Header</span></span>|<span data-ttu-id="0f881-124">Wert</span><span class="sxs-lookup"><span data-stu-id="0f881-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f881-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0f881-125">Authorization</span></span>|<span data-ttu-id="0f881-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0f881-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f881-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0f881-127">Accept</span></span>|<span data-ttu-id="0f881-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0f881-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f881-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0f881-129">Request body</span></span>
<span data-ttu-id="0f881-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0f881-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f881-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f881-131">Response</span></span>
<span data-ttu-id="0f881-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0f881-132">If successful, this method returns a `200 OK` response code and [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f881-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0f881-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f881-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f881-134">Request</span></span>
<span data-ttu-id="0f881-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0f881-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="0f881-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f881-136">Response</span></span>
<span data-ttu-id="0f881-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f881-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 669

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileWiFiConfiguration",
    "id": "8400d131-d131-8400-31d1-008431d10084",
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
    "wiFiSecurityType": "wpaEnterprise"
  }
}
```




