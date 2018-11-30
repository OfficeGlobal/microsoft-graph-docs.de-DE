---
title: Aktion „assign“
description: Noch nicht dokumentiert
ms.openlocfilehash: 4d4d9b994afd2377cb050712acdee779c98bd420
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061460"
---
# <a name="assign-action"></a><span data-ttu-id="2346e-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="2346e-103">assign action</span></span>

> <span data-ttu-id="2346e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2346e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2346e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2346e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2346e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2346e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2346e-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2346e-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2346e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2346e-108">Prerequisites</span></span>
<span data-ttu-id="2346e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2346e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2346e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2346e-111">Permission type</span></span>|<span data-ttu-id="2346e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2346e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2346e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2346e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2346e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2346e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2346e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2346e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2346e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2346e-116">Not supported.</span></span>|
|<span data-ttu-id="2346e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2346e-117">Application</span></span>|<span data-ttu-id="2346e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2346e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2346e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2346e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="2346e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2346e-120">Request headers</span></span>
|<span data-ttu-id="2346e-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2346e-121">Header</span></span>|<span data-ttu-id="2346e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2346e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2346e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2346e-123">Authorization</span></span>|<span data-ttu-id="2346e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2346e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2346e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2346e-125">Accept</span></span>|<span data-ttu-id="2346e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2346e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2346e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2346e-127">Request body</span></span>
<span data-ttu-id="2346e-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="2346e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2346e-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="2346e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2346e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2346e-130">Property</span></span>|<span data-ttu-id="2346e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2346e-131">Type</span></span>|<span data-ttu-id="2346e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2346e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2346e-133">assignments</span><span class="sxs-lookup"><span data-stu-id="2346e-133">assignments</span></span>|<span data-ttu-id="2346e-134">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2346e-134">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="2346e-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2346e-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2346e-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="2346e-136">Response</span></span>
<span data-ttu-id="2346e-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="2346e-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2346e-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2346e-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="2346e-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2346e-139">Request</span></span>
<span data-ttu-id="2346e-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2346e-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign

Content-type: application/json
Content-length: 293

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="2346e-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="2346e-141">Response</span></span>
<span data-ttu-id="2346e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2346e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





