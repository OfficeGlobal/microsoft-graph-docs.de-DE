---
title: sharedPCConfiguration abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fd5188c06d979fb9c81d382ae075b6e3b0fc10aa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823016"
---
# <a name="get-sharedpcconfiguration"></a><span data-ttu-id="f930a-103">sharedPCConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="f930a-103">Get sharedPCConfiguration</span></span>

> <span data-ttu-id="f930a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f930a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f930a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f930a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f930a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f930a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f930a-107">Liest die Eigenschaften und Beziehungen von Objekten des Typs [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f930a-107">Read properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f930a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f930a-108">Prerequisites</span></span>
<span data-ttu-id="f930a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f930a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f930a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f930a-111">Permission type</span></span>|<span data-ttu-id="f930a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f930a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f930a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f930a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f930a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f930a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f930a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f930a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f930a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f930a-116">Not supported.</span></span>|
|<span data-ttu-id="f930a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f930a-117">Application</span></span>|<span data-ttu-id="f930a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f930a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f930a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f930a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f930a-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f930a-120">Optional query parameters</span></span>
<span data-ttu-id="f930a-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f930a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f930a-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f930a-122">Request headers</span></span>
|<span data-ttu-id="f930a-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f930a-123">Header</span></span>|<span data-ttu-id="f930a-124">Wert</span><span class="sxs-lookup"><span data-stu-id="f930a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f930a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f930a-125">Authorization</span></span>|<span data-ttu-id="f930a-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f930a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f930a-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f930a-127">Accept</span></span>|<span data-ttu-id="f930a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f930a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f930a-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f930a-129">Request body</span></span>
<span data-ttu-id="f930a-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f930a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f930a-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f930a-131">Response</span></span>
<span data-ttu-id="f930a-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f930a-132">If successful, this method returns a `200 OK` response code and [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f930a-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f930a-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="f930a-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f930a-134">Request</span></span>
<span data-ttu-id="f930a-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f930a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f930a-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f930a-136">Response</span></span>
<span data-ttu-id="f930a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f930a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1374

{
  "value": {
    "@odata.type": "#microsoft.graph.sharedPCConfiguration",
    "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
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
    "localStorage": "enabled",
    "allowLocalStorage": true,
    "setAccountManager": "enabled",
    "disableAccountManager": true,
    "setEduPolicies": "enabled",
    "disableEduPolicies": true,
    "setPowerPolicies": "enabled",
    "disablePowerPolicies": true,
    "signInOnResume": "enabled",
    "disableSignInOnResume": true,
    "enabled": true,
    "idleTimeBeforeSleepInSeconds": 12,
    "kioskAppDisplayName": "Kiosk App Display Name value",
    "kioskAppUserModelId": "Kiosk App User Model Id value",
    "maintenanceStartTime": "11:59:24.7240000"
  }
}
```





