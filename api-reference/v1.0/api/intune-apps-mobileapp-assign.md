---
title: Aktion „assign“
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0a29e005326381b7ba8ab8d96f22814b87ecfb63
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979922"
---
# <a name="assign-action"></a><span data-ttu-id="943db-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="943db-103">assign action</span></span>

> <span data-ttu-id="943db-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="943db-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="943db-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="943db-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="943db-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="943db-106">Prerequisites</span></span>
<span data-ttu-id="943db-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="943db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="943db-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="943db-109">Permission type</span></span>|<span data-ttu-id="943db-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="943db-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="943db-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="943db-111">Delegated (work or school account)</span></span>|<span data-ttu-id="943db-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="943db-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="943db-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="943db-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="943db-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="943db-114">Not supported.</span></span>|
|<span data-ttu-id="943db-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="943db-115">Application</span></span>|<span data-ttu-id="943db-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="943db-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="943db-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="943db-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="943db-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="943db-118">Request headers</span></span>
|<span data-ttu-id="943db-119">Header</span><span class="sxs-lookup"><span data-stu-id="943db-119">Header</span></span>|<span data-ttu-id="943db-120">Wert</span><span class="sxs-lookup"><span data-stu-id="943db-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="943db-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="943db-121">Authorization</span></span>|<span data-ttu-id="943db-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="943db-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="943db-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="943db-123">Accept</span></span>|<span data-ttu-id="943db-124">application/json</span><span class="sxs-lookup"><span data-stu-id="943db-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="943db-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="943db-125">Request body</span></span>
<span data-ttu-id="943db-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="943db-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="943db-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="943db-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="943db-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="943db-128">Property</span></span>|<span data-ttu-id="943db-129">Typ</span><span class="sxs-lookup"><span data-stu-id="943db-129">Type</span></span>|<span data-ttu-id="943db-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="943db-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="943db-131">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="943db-131">mobileAppAssignments</span></span>|<span data-ttu-id="943db-132">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="943db-132">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="943db-133">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="943db-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="943db-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="943db-134">Response</span></span>
<span data-ttu-id="943db-135">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="943db-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="943db-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="943db-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="943db-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="943db-137">Request</span></span>
<span data-ttu-id="943db-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="943db-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assign

Content-type: application/json
Content-length: 406

{
  "mobileAppAssignments": [
    {
      "@odata.type": "#microsoft.graph.mobileAppAssignment",
      "id": "591620b7-20b7-5916-b720-1659b7201659",
      "intent": "required",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "settings": {
        "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="943db-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="943db-139">Response</span></span>
<span data-ttu-id="943db-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="943db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



