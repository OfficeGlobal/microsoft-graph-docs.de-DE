---
title: Abrufen von „targetedManagedAppPolicyAssignment“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs targetedManagedAppPolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd65b4ae9cc3b0435fcf0d36b486d4b2715c026c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158394"
---
# <a name="get-targetedmanagedapppolicyassignment"></a><span data-ttu-id="84d28-103">Abrufen von „targetedManagedAppPolicyAssignment“</span><span class="sxs-lookup"><span data-stu-id="84d28-103">Get targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="84d28-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="84d28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84d28-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="84d28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84d28-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="84d28-106">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84d28-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="84d28-107">Prerequisites</span></span>
<span data-ttu-id="84d28-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="84d28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="84d28-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="84d28-110">Permission type</span></span>|<span data-ttu-id="84d28-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="84d28-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84d28-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="84d28-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84d28-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="84d28-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="84d28-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="84d28-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84d28-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84d28-115">Not supported.</span></span>|
|<span data-ttu-id="84d28-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="84d28-116">Application</span></span>|<span data-ttu-id="84d28-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84d28-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84d28-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="84d28-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="84d28-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="84d28-119">Optional query parameters</span></span>
<span data-ttu-id="84d28-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="84d28-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84d28-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="84d28-121">Request headers</span></span>
|<span data-ttu-id="84d28-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="84d28-122">Header</span></span>|<span data-ttu-id="84d28-123">Wert</span><span class="sxs-lookup"><span data-stu-id="84d28-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84d28-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="84d28-124">Authorization</span></span>|<span data-ttu-id="84d28-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="84d28-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84d28-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="84d28-126">Accept</span></span>|<span data-ttu-id="84d28-127">application/json</span><span class="sxs-lookup"><span data-stu-id="84d28-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84d28-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="84d28-128">Request body</span></span>
<span data-ttu-id="84d28-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="84d28-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84d28-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="84d28-130">Response</span></span>
<span data-ttu-id="84d28-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="84d28-131">If successful, this method returns a `200 OK` response code and [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84d28-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="84d28-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="84d28-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="84d28-133">Request</span></span>
<span data-ttu-id="84d28-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="84d28-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="84d28-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="84d28-135">Response</span></span>
<span data-ttu-id="84d28-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="84d28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




