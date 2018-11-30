---
title: Abrufen von „targetedManagedAppPolicyAssignment“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs targetedManagedAppPolicyAssignment.
ms.openlocfilehash: 1d318a63f731fd3b28f2dd67a0e3c2ce8cff4740
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016821"
---
# <a name="get-targetedmanagedapppolicyassignment"></a><span data-ttu-id="68b12-103">Abrufen von „targetedManagedAppPolicyAssignment“</span><span class="sxs-lookup"><span data-stu-id="68b12-103">Get targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="68b12-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="68b12-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68b12-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="68b12-105">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="68b12-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="68b12-106">Prerequisites</span></span>
<span data-ttu-id="68b12-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68b12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68b12-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="68b12-109">Permission type</span></span>|<span data-ttu-id="68b12-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="68b12-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68b12-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="68b12-111">Delegated (work or school account)</span></span>|<span data-ttu-id="68b12-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="68b12-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="68b12-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="68b12-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68b12-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="68b12-114">Not supported.</span></span>|
|<span data-ttu-id="68b12-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="68b12-115">Application</span></span>|<span data-ttu-id="68b12-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="68b12-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68b12-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="68b12-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68b12-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="68b12-118">Optional query parameters</span></span>
<span data-ttu-id="68b12-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="68b12-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="68b12-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="68b12-120">Request headers</span></span>
|<span data-ttu-id="68b12-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="68b12-121">Header</span></span>|<span data-ttu-id="68b12-122">Wert</span><span class="sxs-lookup"><span data-stu-id="68b12-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68b12-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="68b12-123">Authorization</span></span>|<span data-ttu-id="68b12-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="68b12-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68b12-125">Accept</span><span class="sxs-lookup"><span data-stu-id="68b12-125">Accept</span></span>|<span data-ttu-id="68b12-126">application/json</span><span class="sxs-lookup"><span data-stu-id="68b12-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68b12-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="68b12-127">Request body</span></span>
<span data-ttu-id="68b12-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="68b12-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68b12-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="68b12-129">Response</span></span>
<span data-ttu-id="68b12-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="68b12-130">If successful, this method returns a `200 OK` response code and [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68b12-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="68b12-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="68b12-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="68b12-132">Request</span></span>
<span data-ttu-id="68b12-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="68b12-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="68b12-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="68b12-134">Response</span></span>
<span data-ttu-id="68b12-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="68b12-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 252

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
    "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```


