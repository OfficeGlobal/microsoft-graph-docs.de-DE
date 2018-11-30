---
title: Abrufen von „targetedManagedAppPolicyAssignment“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs targetedManagedAppPolicyAssignment.
ms.openlocfilehash: 863c3aad782e7badc97008df1c8fb755b77f2f89
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27057910"
---
# <a name="get-targetedmanagedapppolicyassignment"></a><span data-ttu-id="028d8-103">Abrufen von „targetedManagedAppPolicyAssignment“</span><span class="sxs-lookup"><span data-stu-id="028d8-103">Get targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="028d8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="028d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="028d8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="028d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="028d8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="028d8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="028d8-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="028d8-107">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="028d8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="028d8-108">Prerequisites</span></span>
<span data-ttu-id="028d8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="028d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="028d8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="028d8-111">Permission type</span></span>|<span data-ttu-id="028d8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="028d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="028d8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="028d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="028d8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="028d8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="028d8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="028d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="028d8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="028d8-116">Not supported.</span></span>|
|<span data-ttu-id="028d8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="028d8-117">Application</span></span>|<span data-ttu-id="028d8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="028d8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="028d8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="028d8-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="028d8-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="028d8-120">Optional query parameters</span></span>
<span data-ttu-id="028d8-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="028d8-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="028d8-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="028d8-122">Request headers</span></span>
|<span data-ttu-id="028d8-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="028d8-123">Header</span></span>|<span data-ttu-id="028d8-124">Wert</span><span class="sxs-lookup"><span data-stu-id="028d8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="028d8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="028d8-125">Authorization</span></span>|<span data-ttu-id="028d8-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="028d8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="028d8-127">Accept</span><span class="sxs-lookup"><span data-stu-id="028d8-127">Accept</span></span>|<span data-ttu-id="028d8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="028d8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="028d8-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="028d8-129">Request body</span></span>
<span data-ttu-id="028d8-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="028d8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="028d8-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="028d8-131">Response</span></span>
<span data-ttu-id="028d8-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="028d8-132">If successful, this method returns a `200 OK` response code and [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="028d8-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="028d8-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="028d8-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="028d8-134">Request</span></span>
<span data-ttu-id="028d8-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="028d8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="028d8-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="028d8-136">Response</span></span>
<span data-ttu-id="028d8-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="028d8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





