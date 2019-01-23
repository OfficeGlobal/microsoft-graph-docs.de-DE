---
title: Aktion „assign“
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bebc8864db76525fc34d21325ec1f67750525617
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396000"
---
# <a name="assign-action"></a><span data-ttu-id="9192a-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="9192a-103">assign action</span></span>

> <span data-ttu-id="9192a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="9192a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9192a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9192a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9192a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9192a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9192a-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9192a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9192a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9192a-108">Prerequisites</span></span>
<span data-ttu-id="9192a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9192a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9192a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9192a-111">Permission type</span></span>|<span data-ttu-id="9192a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9192a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9192a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9192a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9192a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9192a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9192a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9192a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9192a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9192a-116">Not supported.</span></span>|
|<span data-ttu-id="9192a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9192a-117">Application</span></span>|<span data-ttu-id="9192a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9192a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9192a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9192a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="9192a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9192a-120">Request headers</span></span>
|<span data-ttu-id="9192a-121">Header</span><span class="sxs-lookup"><span data-stu-id="9192a-121">Header</span></span>|<span data-ttu-id="9192a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9192a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9192a-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9192a-123">Authorization</span></span>|<span data-ttu-id="9192a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9192a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9192a-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9192a-125">Accept</span></span>|<span data-ttu-id="9192a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9192a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9192a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9192a-127">Request body</span></span>
<span data-ttu-id="9192a-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="9192a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9192a-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="9192a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9192a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9192a-130">Property</span></span>|<span data-ttu-id="9192a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9192a-131">Type</span></span>|<span data-ttu-id="9192a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9192a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9192a-133">assignments</span><span class="sxs-lookup"><span data-stu-id="9192a-133">assignments</span></span>|<span data-ttu-id="9192a-134">Collection von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9192a-134">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="9192a-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9192a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9192a-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9192a-136">Response</span></span>
<span data-ttu-id="9192a-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="9192a-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9192a-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9192a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="9192a-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9192a-139">Request</span></span>
<span data-ttu-id="9192a-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9192a-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9192a-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="9192a-141">Response</span></span>
<span data-ttu-id="9192a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9192a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




