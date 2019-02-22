---
title: Aktion zuweisen
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9800d1d25952aab283a50f098532501875f3e267
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144548"
---
# <a name="assign-action"></a><span data-ttu-id="00ec0-103">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="00ec0-103">assign action</span></span>

> <span data-ttu-id="00ec0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="00ec0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00ec0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="00ec0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00ec0-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="00ec0-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00ec0-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="00ec0-107">Prerequisites</span></span>
<span data-ttu-id="00ec0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="00ec0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="00ec0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="00ec0-110">Permission type</span></span>|<span data-ttu-id="00ec0-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="00ec0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00ec0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="00ec0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="00ec0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00ec0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="00ec0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="00ec0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00ec0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="00ec0-115">Not supported.</span></span>|
|<span data-ttu-id="00ec0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="00ec0-116">Application</span></span>|<span data-ttu-id="00ec0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="00ec0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00ec0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="00ec0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="00ec0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="00ec0-119">Request headers</span></span>
|<span data-ttu-id="00ec0-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="00ec0-120">Header</span></span>|<span data-ttu-id="00ec0-121">Wert</span><span class="sxs-lookup"><span data-stu-id="00ec0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00ec0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="00ec0-122">Authorization</span></span>|<span data-ttu-id="00ec0-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="00ec0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00ec0-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="00ec0-124">Accept</span></span>|<span data-ttu-id="00ec0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="00ec0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00ec0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="00ec0-126">Request body</span></span>
<span data-ttu-id="00ec0-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="00ec0-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="00ec0-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="00ec0-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="00ec0-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="00ec0-129">Property</span></span>|<span data-ttu-id="00ec0-130">Typ</span><span class="sxs-lookup"><span data-stu-id="00ec0-130">Type</span></span>|<span data-ttu-id="00ec0-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00ec0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00ec0-132">assignments</span><span class="sxs-lookup"><span data-stu-id="00ec0-132">assignments</span></span>|<span data-ttu-id="00ec0-133">Collection von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="00ec0-133">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="00ec0-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="00ec0-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="00ec0-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="00ec0-135">Response</span></span>
<span data-ttu-id="00ec0-136">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="00ec0-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="00ec0-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="00ec0-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="00ec0-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="00ec0-138">Request</span></span>
<span data-ttu-id="00ec0-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="00ec0-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign

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

### <a name="response"></a><span data-ttu-id="00ec0-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="00ec0-140">Response</span></span>
<span data-ttu-id="00ec0-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="00ec0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




