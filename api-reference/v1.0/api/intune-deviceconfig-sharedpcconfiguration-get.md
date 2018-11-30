---
title: sharedPCConfiguration abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs sharedPCConfiguration.
ms.openlocfilehash: d0b7350441afd582b64bb2854056f2f0fcdee1b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017037"
---
# <a name="get-sharedpcconfiguration"></a><span data-ttu-id="94e7d-103">sharedPCConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="94e7d-103">Get sharedPCConfiguration</span></span>

> <span data-ttu-id="94e7d-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="94e7d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94e7d-105">Liest die Eigenschaften und Beziehungen von Objekten des Typs [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="94e7d-105">Read properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="94e7d-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="94e7d-106">Prerequisites</span></span>
<span data-ttu-id="94e7d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94e7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94e7d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="94e7d-109">Permission type</span></span>|<span data-ttu-id="94e7d-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="94e7d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94e7d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="94e7d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="94e7d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="94e7d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="94e7d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="94e7d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94e7d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="94e7d-114">Not supported.</span></span>|
|<span data-ttu-id="94e7d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="94e7d-115">Application</span></span>|<span data-ttu-id="94e7d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="94e7d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94e7d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="94e7d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94e7d-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="94e7d-118">Optional query parameters</span></span>
<span data-ttu-id="94e7d-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="94e7d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="94e7d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="94e7d-120">Request headers</span></span>
|<span data-ttu-id="94e7d-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="94e7d-121">Header</span></span>|<span data-ttu-id="94e7d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="94e7d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94e7d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="94e7d-123">Authorization</span></span>|<span data-ttu-id="94e7d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="94e7d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94e7d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="94e7d-125">Accept</span></span>|<span data-ttu-id="94e7d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="94e7d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94e7d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="94e7d-127">Request body</span></span>
<span data-ttu-id="94e7d-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="94e7d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94e7d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="94e7d-129">Response</span></span>
<span data-ttu-id="94e7d-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="94e7d-130">If successful, this method returns a `200 OK` response code and [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94e7d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="94e7d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="94e7d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="94e7d-132">Request</span></span>
<span data-ttu-id="94e7d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="94e7d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="94e7d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="94e7d-134">Response</span></span>
<span data-ttu-id="94e7d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="94e7d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1101

{
  "value": {
    "@odata.type": "#microsoft.graph.sharedPCConfiguration",
    "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "accountManagerPolicy": {
      "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
      "accountDeletionPolicy": "diskSpaceThreshold",
      "cacheAccountsAboveDiskFreePercentage": 4,
      "inactiveThresholdDays": 5,
      "removeAccountsBelowDiskFreePercentage": 5
    },
    "allowedAccounts": "domain",
    "allowLocalStorage": true,
    "disableAccountManager": true,
    "disableEduPolicies": true,
    "disablePowerPolicies": true,
    "disableSignInOnResume": true,
    "enabled": true,
    "idleTimeBeforeSleepInSeconds": 12,
    "kioskAppDisplayName": "Kiosk App Display Name value",
    "kioskAppUserModelId": "Kiosk App User Model Id value",
    "maintenanceStartTime": "11:59:24.7240000"
  }
}
```



