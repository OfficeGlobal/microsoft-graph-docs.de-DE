---
title: Abrufen von „managedAppPolicyDeploymentSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppPolicyDeploymentSummary.
ms.openlocfilehash: 46abf9b5c0eedb8c8990646cf96317a8083e2a21
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066086"
---
# <a name="get-managedapppolicydeploymentsummary"></a><span data-ttu-id="7a7a4-103">Abrufen von „managedAppPolicyDeploymentSummary“</span><span class="sxs-lookup"><span data-stu-id="7a7a4-103">Get managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="7a7a4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7a7a4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a7a4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7a7a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a7a4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7a7a4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a7a4-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="7a7a4-107">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7a7a4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7a7a4-108">Prerequisites</span></span>
<span data-ttu-id="7a7a4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a7a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a7a4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7a7a4-111">Permission type</span></span>|<span data-ttu-id="7a7a4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7a7a4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a7a4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7a7a4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a7a4-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a7a4-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7a7a4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7a7a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a7a4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a7a4-116">Not supported.</span></span>|
|<span data-ttu-id="7a7a4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7a7a4-117">Application</span></span>|<span data-ttu-id="7a7a4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a7a4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a7a4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a7a4-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="7a7a4-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7a7a4-120">Optional query parameters</span></span>
<span data-ttu-id="7a7a4-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7a7a4-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7a7a4-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7a7a4-122">Request headers</span></span>
|<span data-ttu-id="7a7a4-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7a7a4-123">Header</span></span>|<span data-ttu-id="7a7a4-124">Wert</span><span class="sxs-lookup"><span data-stu-id="7a7a4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a7a4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a7a4-125">Authorization</span></span>|<span data-ttu-id="7a7a4-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7a7a4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a7a4-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7a7a4-127">Accept</span></span>|<span data-ttu-id="7a7a4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7a7a4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a7a4-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7a7a4-129">Request body</span></span>
<span data-ttu-id="7a7a4-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7a7a4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a7a4-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a7a4-131">Response</span></span>
<span data-ttu-id="7a7a4-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7a7a4-132">If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a7a4-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7a7a4-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="7a7a4-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a7a4-134">Request</span></span>
<span data-ttu-id="7a7a4-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7a7a4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### <a name="response"></a><span data-ttu-id="7a7a4-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a7a4-136">Response</span></span>
<span data-ttu-id="7a7a4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a7a4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





