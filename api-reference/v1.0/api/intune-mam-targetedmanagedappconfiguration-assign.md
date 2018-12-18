---
title: Aktion „assign“
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 77fc33eebb170783929eb61b6926089af372efdf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344184"
---
# <a name="assign-action"></a><span data-ttu-id="e930d-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="e930d-103">assign action</span></span>

> <span data-ttu-id="e930d-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e930d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e930d-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e930d-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e930d-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e930d-106">Prerequisites</span></span>
<span data-ttu-id="e930d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e930d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e930d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e930d-109">Permission type</span></span>|<span data-ttu-id="e930d-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e930d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e930d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e930d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e930d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e930d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e930d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e930d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e930d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e930d-114">Not supported.</span></span>|
|<span data-ttu-id="e930d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e930d-115">Application</span></span>|<span data-ttu-id="e930d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e930d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e930d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e930d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="e930d-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e930d-118">Request headers</span></span>
|<span data-ttu-id="e930d-119">Header</span><span class="sxs-lookup"><span data-stu-id="e930d-119">Header</span></span>|<span data-ttu-id="e930d-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e930d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e930d-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e930d-121">Authorization</span></span>|<span data-ttu-id="e930d-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e930d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e930d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e930d-123">Accept</span></span>|<span data-ttu-id="e930d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e930d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e930d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e930d-125">Request body</span></span>
<span data-ttu-id="e930d-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="e930d-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e930d-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="e930d-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e930d-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e930d-128">Property</span></span>|<span data-ttu-id="e930d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e930d-129">Type</span></span>|<span data-ttu-id="e930d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e930d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e930d-131">assignments</span><span class="sxs-lookup"><span data-stu-id="e930d-131">assignments</span></span>|<span data-ttu-id="e930d-132">Collection von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e930d-132">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="e930d-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e930d-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e930d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e930d-134">Response</span></span>
<span data-ttu-id="e930d-135">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="e930d-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e930d-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e930d-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="e930d-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e930d-137">Request</span></span>
<span data-ttu-id="e930d-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e930d-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign

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

### <a name="response"></a><span data-ttu-id="e930d-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="e930d-139">Response</span></span>
<span data-ttu-id="e930d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e930d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



