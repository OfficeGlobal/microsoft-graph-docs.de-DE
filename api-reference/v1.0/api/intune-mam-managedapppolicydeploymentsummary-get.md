---
title: Abrufen von „managedAppPolicyDeploymentSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppPolicyDeploymentSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a5fda5e69925d7541df62a8747d8e0cb55db51a0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250124"
---
# <a name="get-managedapppolicydeploymentsummary"></a><span data-ttu-id="21229-103">Abrufen von „managedAppPolicyDeploymentSummary“</span><span class="sxs-lookup"><span data-stu-id="21229-103">Get managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="21229-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="21229-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21229-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="21229-105">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21229-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="21229-106">Prerequisites</span></span>
<span data-ttu-id="21229-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="21229-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="21229-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="21229-109">Permission type</span></span>|<span data-ttu-id="21229-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="21229-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21229-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="21229-111">Delegated (work or school account)</span></span>|<span data-ttu-id="21229-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="21229-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="21229-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="21229-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21229-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21229-114">Not supported.</span></span>|
|<span data-ttu-id="21229-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="21229-115">Application</span></span>|<span data-ttu-id="21229-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21229-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21229-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="21229-117">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="21229-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="21229-118">Optional query parameters</span></span>
<span data-ttu-id="21229-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="21229-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="21229-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="21229-120">Request headers</span></span>
|<span data-ttu-id="21229-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="21229-121">Header</span></span>|<span data-ttu-id="21229-122">Wert</span><span class="sxs-lookup"><span data-stu-id="21229-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21229-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21229-123">Authorization</span></span>|<span data-ttu-id="21229-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="21229-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21229-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="21229-125">Accept</span></span>|<span data-ttu-id="21229-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21229-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21229-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="21229-127">Request body</span></span>
<span data-ttu-id="21229-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="21229-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21229-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="21229-129">Response</span></span>
<span data-ttu-id="21229-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="21229-130">If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21229-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="21229-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="21229-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="21229-132">Request</span></span>
<span data-ttu-id="21229-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="21229-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### <a name="response"></a><span data-ttu-id="21229-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="21229-134">Response</span></span>
<span data-ttu-id="21229-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="21229-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



