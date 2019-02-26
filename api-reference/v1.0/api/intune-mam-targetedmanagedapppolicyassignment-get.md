---
title: Abrufen von „targetedManagedAppPolicyAssignment“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs targetedManagedAppPolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8956cb9b3877fa3f53ce65b306b8d1384ad12b8d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259997"
---
# <a name="get-targetedmanagedapppolicyassignment"></a><span data-ttu-id="d6c54-103">Abrufen von „targetedManagedAppPolicyAssignment“</span><span class="sxs-lookup"><span data-stu-id="d6c54-103">Get targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="d6c54-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d6c54-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6c54-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d6c54-105">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6c54-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d6c54-106">Prerequisites</span></span>
<span data-ttu-id="d6c54-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d6c54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d6c54-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d6c54-109">Permission type</span></span>|<span data-ttu-id="d6c54-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d6c54-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6c54-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d6c54-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d6c54-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6c54-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d6c54-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d6c54-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6c54-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d6c54-114">Not supported.</span></span>|
|<span data-ttu-id="d6c54-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d6c54-115">Application</span></span>|<span data-ttu-id="d6c54-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d6c54-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6c54-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d6c54-117">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="d6c54-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d6c54-118">Optional query parameters</span></span>
<span data-ttu-id="d6c54-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d6c54-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6c54-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d6c54-120">Request headers</span></span>
|<span data-ttu-id="d6c54-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d6c54-121">Header</span></span>|<span data-ttu-id="d6c54-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d6c54-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6c54-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6c54-123">Authorization</span></span>|<span data-ttu-id="d6c54-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d6c54-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6c54-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d6c54-125">Accept</span></span>|<span data-ttu-id="d6c54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6c54-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6c54-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d6c54-127">Request body</span></span>
<span data-ttu-id="d6c54-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d6c54-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6c54-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d6c54-129">Response</span></span>
<span data-ttu-id="d6c54-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d6c54-130">If successful, this method returns a `200 OK` response code and [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6c54-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d6c54-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6c54-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d6c54-132">Request</span></span>
<span data-ttu-id="d6c54-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d6c54-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="d6c54-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d6c54-134">Response</span></span>
<span data-ttu-id="d6c54-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d6c54-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



