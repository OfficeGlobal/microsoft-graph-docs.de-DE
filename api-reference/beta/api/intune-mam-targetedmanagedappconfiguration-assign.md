---
title: Aktion „assign“
description: Noch nicht dokumentiert
ms.openlocfilehash: bb38ae7db4614a15900cee9ad48f61bb622c8233
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065355"
---
# <a name="assign-action"></a><span data-ttu-id="a8228-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="a8228-103">assign action</span></span>

> <span data-ttu-id="a8228-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a8228-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8228-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a8228-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8228-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a8228-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8228-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a8228-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a8228-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a8228-108">Prerequisites</span></span>
<span data-ttu-id="a8228-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8228-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8228-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a8228-111">Permission type</span></span>|<span data-ttu-id="a8228-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a8228-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8228-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a8228-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8228-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8228-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a8228-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a8228-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8228-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8228-116">Not supported.</span></span>|
|<span data-ttu-id="a8228-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a8228-117">Application</span></span>|<span data-ttu-id="a8228-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8228-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8228-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8228-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="a8228-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a8228-120">Request headers</span></span>
|<span data-ttu-id="a8228-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a8228-121">Header</span></span>|<span data-ttu-id="a8228-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a8228-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8228-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8228-123">Authorization</span></span>|<span data-ttu-id="a8228-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a8228-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8228-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a8228-125">Accept</span></span>|<span data-ttu-id="a8228-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8228-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8228-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a8228-127">Request body</span></span>
<span data-ttu-id="a8228-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="a8228-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a8228-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="a8228-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a8228-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a8228-130">Property</span></span>|<span data-ttu-id="a8228-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a8228-131">Type</span></span>|<span data-ttu-id="a8228-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8228-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8228-133">assignments</span><span class="sxs-lookup"><span data-stu-id="a8228-133">assignments</span></span>|<span data-ttu-id="a8228-134">Collection von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a8228-134">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="a8228-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a8228-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a8228-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8228-136">Response</span></span>
<span data-ttu-id="a8228-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="a8228-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a8228-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a8228-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="a8228-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8228-139">Request</span></span>
<span data-ttu-id="a8228-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a8228-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign

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

### <a name="response"></a><span data-ttu-id="a8228-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8228-141">Response</span></span>
<span data-ttu-id="a8228-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8228-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





