---
title: Abrufen von „managedAppPolicyDeploymentSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppPolicyDeploymentSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c2ed611feda18f90cd5bebe7ec0a510f462d0511
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974112"
---
# <a name="get-managedapppolicydeploymentsummary"></a><span data-ttu-id="15dbf-103">Abrufen von „managedAppPolicyDeploymentSummary“</span><span class="sxs-lookup"><span data-stu-id="15dbf-103">Get managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="15dbf-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="15dbf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15dbf-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="15dbf-105">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="15dbf-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="15dbf-106">Prerequisites</span></span>
<span data-ttu-id="15dbf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15dbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15dbf-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="15dbf-109">Permission type</span></span>|<span data-ttu-id="15dbf-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="15dbf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15dbf-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="15dbf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="15dbf-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="15dbf-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="15dbf-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="15dbf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15dbf-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15dbf-114">Not supported.</span></span>|
|<span data-ttu-id="15dbf-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="15dbf-115">Application</span></span>|<span data-ttu-id="15dbf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15dbf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15dbf-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="15dbf-117">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="15dbf-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="15dbf-118">Optional query parameters</span></span>
<span data-ttu-id="15dbf-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="15dbf-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="15dbf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="15dbf-120">Request headers</span></span>
|<span data-ttu-id="15dbf-121">Header</span><span class="sxs-lookup"><span data-stu-id="15dbf-121">Header</span></span>|<span data-ttu-id="15dbf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="15dbf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15dbf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="15dbf-123">Authorization</span></span>|<span data-ttu-id="15dbf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="15dbf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15dbf-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="15dbf-125">Accept</span></span>|<span data-ttu-id="15dbf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15dbf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15dbf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="15dbf-127">Request body</span></span>
<span data-ttu-id="15dbf-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="15dbf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15dbf-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="15dbf-129">Response</span></span>
<span data-ttu-id="15dbf-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="15dbf-130">If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15dbf-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="15dbf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="15dbf-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15dbf-132">Request</span></span>
<span data-ttu-id="15dbf-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="15dbf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### <a name="response"></a><span data-ttu-id="15dbf-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="15dbf-134">Response</span></span>
<span data-ttu-id="15dbf-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15dbf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



