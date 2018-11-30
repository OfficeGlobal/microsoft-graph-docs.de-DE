---
title: Auflisten von „sharedPCConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs sharedPCConfiguration auf.
ms.openlocfilehash: 18cd0562dbb53b796923f76bff5156a306b51962
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016552"
---
# <a name="list-sharedpcconfigurations"></a><span data-ttu-id="fba18-103">Auflisten von „sharedPCConfiguration“</span><span class="sxs-lookup"><span data-stu-id="fba18-103">List sharedPCConfigurations</span></span>

> <span data-ttu-id="fba18-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fba18-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fba18-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="fba18-105">List properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fba18-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fba18-106">Prerequisites</span></span>
<span data-ttu-id="fba18-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fba18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fba18-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fba18-109">Permission type</span></span>|<span data-ttu-id="fba18-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fba18-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fba18-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fba18-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fba18-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fba18-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fba18-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fba18-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fba18-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fba18-114">Not supported.</span></span>|
|<span data-ttu-id="fba18-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fba18-115">Application</span></span>|<span data-ttu-id="fba18-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fba18-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fba18-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fba18-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fba18-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fba18-118">Request headers</span></span>
|<span data-ttu-id="fba18-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fba18-119">Header</span></span>|<span data-ttu-id="fba18-120">Wert</span><span class="sxs-lookup"><span data-stu-id="fba18-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fba18-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fba18-121">Authorization</span></span>|<span data-ttu-id="fba18-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fba18-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fba18-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fba18-123">Accept</span></span>|<span data-ttu-id="fba18-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fba18-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fba18-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fba18-125">Request body</span></span>
<span data-ttu-id="fba18-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fba18-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fba18-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="fba18-127">Response</span></span>
<span data-ttu-id="fba18-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fba18-128">If successful, this method returns a `200 OK` response code and a collection of [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fba18-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fba18-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="fba18-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fba18-130">Request</span></span>
<span data-ttu-id="fba18-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fba18-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="fba18-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="fba18-132">Response</span></span>
<span data-ttu-id="fba18-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fba18-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1165

{
  "value": [
    {
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
  ]
}
```


