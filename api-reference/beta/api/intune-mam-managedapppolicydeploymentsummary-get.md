---
title: Abrufen von „managedAppPolicyDeploymentSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppPolicyDeploymentSummary.
author: tfitzmac
ms.openlocfilehash: 7c33021c0bfa31f6a562bfc54efb4d8d195dadd8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334881"
---
# <a name="get-managedapppolicydeploymentsummary"></a><span data-ttu-id="f952f-103">Abrufen von „managedAppPolicyDeploymentSummary“</span><span class="sxs-lookup"><span data-stu-id="f952f-103">Get managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="f952f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f952f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f952f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f952f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f952f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f952f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f952f-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="f952f-107">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f952f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f952f-108">Prerequisites</span></span>
<span data-ttu-id="f952f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f952f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f952f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f952f-111">Permission type</span></span>|<span data-ttu-id="f952f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f952f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f952f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f952f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f952f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f952f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f952f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f952f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f952f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f952f-116">Not supported.</span></span>|
|<span data-ttu-id="f952f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f952f-117">Application</span></span>|<span data-ttu-id="f952f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f952f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f952f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f952f-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="f952f-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f952f-120">Optional query parameters</span></span>
<span data-ttu-id="f952f-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f952f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f952f-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f952f-122">Request headers</span></span>
|<span data-ttu-id="f952f-123">Header</span><span class="sxs-lookup"><span data-stu-id="f952f-123">Header</span></span>|<span data-ttu-id="f952f-124">Wert</span><span class="sxs-lookup"><span data-stu-id="f952f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f952f-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f952f-125">Authorization</span></span>|<span data-ttu-id="f952f-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f952f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f952f-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f952f-127">Accept</span></span>|<span data-ttu-id="f952f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f952f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f952f-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f952f-129">Request body</span></span>
<span data-ttu-id="f952f-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f952f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f952f-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f952f-131">Response</span></span>
<span data-ttu-id="f952f-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f952f-132">If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f952f-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f952f-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="f952f-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f952f-134">Request</span></span>
<span data-ttu-id="f952f-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f952f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### <a name="response"></a><span data-ttu-id="f952f-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f952f-136">Response</span></span>
<span data-ttu-id="f952f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f952f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





