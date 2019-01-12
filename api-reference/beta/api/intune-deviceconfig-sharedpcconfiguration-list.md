---
title: Auflisten von „sharedPCConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs sharedPCConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a65c6d2d678a02e9f69741a63dfb0817747ed975
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914164"
---
# <a name="list-sharedpcconfigurations"></a><span data-ttu-id="027ab-103">Auflisten von „sharedPCConfiguration“</span><span class="sxs-lookup"><span data-stu-id="027ab-103">List sharedPCConfigurations</span></span>

> <span data-ttu-id="027ab-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="027ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="027ab-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="027ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="027ab-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="027ab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="027ab-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="027ab-107">List properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="027ab-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="027ab-108">Prerequisites</span></span>
<span data-ttu-id="027ab-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="027ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="027ab-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="027ab-111">Permission type</span></span>|<span data-ttu-id="027ab-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="027ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="027ab-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="027ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="027ab-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="027ab-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="027ab-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="027ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="027ab-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="027ab-116">Not supported.</span></span>|
|<span data-ttu-id="027ab-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="027ab-117">Application</span></span>|<span data-ttu-id="027ab-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="027ab-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="027ab-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="027ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="027ab-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="027ab-120">Request headers</span></span>
|<span data-ttu-id="027ab-121">Header</span><span class="sxs-lookup"><span data-stu-id="027ab-121">Header</span></span>|<span data-ttu-id="027ab-122">Wert</span><span class="sxs-lookup"><span data-stu-id="027ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="027ab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="027ab-123">Authorization</span></span>|<span data-ttu-id="027ab-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="027ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="027ab-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="027ab-125">Accept</span></span>|<span data-ttu-id="027ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="027ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="027ab-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="027ab-127">Request body</span></span>
<span data-ttu-id="027ab-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="027ab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="027ab-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="027ab-129">Response</span></span>
<span data-ttu-id="027ab-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="027ab-130">If successful, this method returns a `200 OK` response code and a collection of [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="027ab-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="027ab-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="027ab-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="027ab-132">Request</span></span>
<span data-ttu-id="027ab-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="027ab-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="027ab-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="027ab-134">Response</span></span>
<span data-ttu-id="027ab-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="027ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1456

{
  "value": [
    {
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
  ]
}
```





