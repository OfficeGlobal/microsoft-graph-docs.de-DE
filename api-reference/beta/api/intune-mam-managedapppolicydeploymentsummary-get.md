---
title: Abrufen von „managedAppPolicyDeploymentSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppPolicyDeploymentSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 19eef6e2595e396cabd9cc4f3ae8fbf1198c39d9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983113"
---
# <a name="get-managedapppolicydeploymentsummary"></a><span data-ttu-id="dedeb-103">Abrufen von „managedAppPolicyDeploymentSummary“</span><span class="sxs-lookup"><span data-stu-id="dedeb-103">Get managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="dedeb-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dedeb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dedeb-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="dedeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dedeb-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="dedeb-106">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dedeb-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dedeb-107">Prerequisites</span></span>
<span data-ttu-id="dedeb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dedeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dedeb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dedeb-110">Permission type</span></span>|<span data-ttu-id="dedeb-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dedeb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dedeb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dedeb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dedeb-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dedeb-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="dedeb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dedeb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dedeb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dedeb-115">Not supported.</span></span>|
|<span data-ttu-id="dedeb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dedeb-116">Application</span></span>|<span data-ttu-id="dedeb-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dedeb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dedeb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dedeb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/deploymentSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dedeb-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="dedeb-119">Optional query parameters</span></span>
<span data-ttu-id="dedeb-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dedeb-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dedeb-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dedeb-121">Request headers</span></span>
|<span data-ttu-id="dedeb-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dedeb-122">Header</span></span>|<span data-ttu-id="dedeb-123">Wert</span><span class="sxs-lookup"><span data-stu-id="dedeb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dedeb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dedeb-124">Authorization</span></span>|<span data-ttu-id="dedeb-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dedeb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dedeb-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dedeb-126">Accept</span></span>|<span data-ttu-id="dedeb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="dedeb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dedeb-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dedeb-128">Request body</span></span>
<span data-ttu-id="dedeb-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dedeb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dedeb-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="dedeb-130">Response</span></span>
<span data-ttu-id="dedeb-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="dedeb-131">If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dedeb-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dedeb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="dedeb-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dedeb-133">Request</span></span>
<span data-ttu-id="dedeb-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dedeb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### <a name="response"></a><span data-ttu-id="dedeb-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="dedeb-135">Response</span></span>
<span data-ttu-id="dedeb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dedeb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 688

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
    "displayName": "Display Name value",
    "configurationDeployedUserCount": 14,
    "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
    "configurationDeploymentSummaryPerApp": [
      {
        "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
        "mobileAppIdentifier": {
          "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
          "packageId": "Package Id value"
        },
        "configurationAppliedUserCount": 13
      }
    ],
    "id": "61f2f688-f688-61f2-88f6-f26188f6f261",
    "version": "Version value"
  }
}
```




