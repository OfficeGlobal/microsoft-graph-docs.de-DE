---
title: Aktion „assign“
description: Noch nicht dokumentiert
ms.openlocfilehash: 92a72fe9fce0f1bcbe458608a02cb939e20ed3ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016287"
---
# <a name="assign-action"></a><span data-ttu-id="35c07-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="35c07-103">assign action</span></span>

> <span data-ttu-id="35c07-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="35c07-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35c07-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="35c07-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="35c07-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="35c07-106">Prerequisites</span></span>
<span data-ttu-id="35c07-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35c07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35c07-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="35c07-109">Permission type</span></span>|<span data-ttu-id="35c07-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="35c07-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35c07-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="35c07-111">Delegated (work or school account)</span></span>|<span data-ttu-id="35c07-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35c07-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="35c07-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="35c07-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35c07-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="35c07-114">Not supported.</span></span>|
|<span data-ttu-id="35c07-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="35c07-115">Application</span></span>|<span data-ttu-id="35c07-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="35c07-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35c07-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="35c07-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="35c07-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="35c07-118">Request headers</span></span>
|<span data-ttu-id="35c07-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="35c07-119">Header</span></span>|<span data-ttu-id="35c07-120">Wert</span><span class="sxs-lookup"><span data-stu-id="35c07-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35c07-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="35c07-121">Authorization</span></span>|<span data-ttu-id="35c07-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="35c07-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35c07-123">Accept</span><span class="sxs-lookup"><span data-stu-id="35c07-123">Accept</span></span>|<span data-ttu-id="35c07-124">application/json</span><span class="sxs-lookup"><span data-stu-id="35c07-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35c07-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="35c07-125">Request body</span></span>
<span data-ttu-id="35c07-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="35c07-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="35c07-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="35c07-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="35c07-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="35c07-128">Property</span></span>|<span data-ttu-id="35c07-129">Typ</span><span class="sxs-lookup"><span data-stu-id="35c07-129">Type</span></span>|<span data-ttu-id="35c07-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35c07-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35c07-131">assignments</span><span class="sxs-lookup"><span data-stu-id="35c07-131">assignments</span></span>|<span data-ttu-id="35c07-132">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="35c07-132">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="35c07-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="35c07-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="35c07-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="35c07-134">Response</span></span>
<span data-ttu-id="35c07-135">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="35c07-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="35c07-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="35c07-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="35c07-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="35c07-137">Request</span></span>
<span data-ttu-id="35c07-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="35c07-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign

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

### <a name="response"></a><span data-ttu-id="35c07-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="35c07-139">Response</span></span>
<span data-ttu-id="35c07-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="35c07-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



