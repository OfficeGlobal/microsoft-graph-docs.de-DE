---
title: Aktion zuweisen
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb6186afa6e535f6089709572205b85015bb29d5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981181"
---
# <a name="assign-action"></a><span data-ttu-id="a7d55-103">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="a7d55-103">assign action</span></span>

> <span data-ttu-id="a7d55-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a7d55-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7d55-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a7d55-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7d55-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a7d55-106">Prerequisites</span></span>
<span data-ttu-id="a7d55-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7d55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7d55-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a7d55-109">Permission type</span></span>|<span data-ttu-id="a7d55-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a7d55-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7d55-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a7d55-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a7d55-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7d55-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a7d55-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a7d55-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7d55-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a7d55-114">Not supported.</span></span>|
|<span data-ttu-id="a7d55-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a7d55-115">Application</span></span>|<span data-ttu-id="a7d55-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a7d55-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7d55-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a7d55-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="a7d55-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a7d55-118">Request headers</span></span>
|<span data-ttu-id="a7d55-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a7d55-119">Header</span></span>|<span data-ttu-id="a7d55-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a7d55-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7d55-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7d55-121">Authorization</span></span>|<span data-ttu-id="a7d55-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a7d55-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7d55-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a7d55-123">Accept</span></span>|<span data-ttu-id="a7d55-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a7d55-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7d55-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a7d55-125">Request body</span></span>
<span data-ttu-id="a7d55-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="a7d55-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a7d55-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="a7d55-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a7d55-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a7d55-128">Property</span></span>|<span data-ttu-id="a7d55-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a7d55-129">Type</span></span>|<span data-ttu-id="a7d55-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a7d55-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7d55-131">assignments</span><span class="sxs-lookup"><span data-stu-id="a7d55-131">assignments</span></span>|<span data-ttu-id="a7d55-132">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a7d55-132">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="a7d55-133">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="a7d55-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a7d55-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a7d55-134">Response</span></span>
<span data-ttu-id="a7d55-135">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a7d55-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a7d55-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a7d55-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7d55-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a7d55-137">Request</span></span>
<span data-ttu-id="a7d55-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a7d55-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign

Content-type: application/json
Content-length: 282

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a7d55-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="a7d55-139">Response</span></span>
<span data-ttu-id="a7d55-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a7d55-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



