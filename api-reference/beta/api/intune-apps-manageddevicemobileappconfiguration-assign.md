---
title: Aktion „assign“
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 019abecc0f9d7560f907652166f8e2ba54cfa2c3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974749"
---
# <a name="assign-action"></a><span data-ttu-id="91216-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="91216-103">assign action</span></span>

> <span data-ttu-id="91216-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="91216-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91216-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="91216-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91216-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="91216-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91216-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="91216-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="91216-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="91216-108">Prerequisites</span></span>
<span data-ttu-id="91216-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91216-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91216-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="91216-111">Permission type</span></span>|<span data-ttu-id="91216-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="91216-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91216-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="91216-113">Delegated (work or school account)</span></span>|<span data-ttu-id="91216-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91216-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="91216-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="91216-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91216-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="91216-116">Not supported.</span></span>|
|<span data-ttu-id="91216-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="91216-117">Application</span></span>|<span data-ttu-id="91216-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="91216-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91216-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="91216-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="91216-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="91216-120">Request headers</span></span>
|<span data-ttu-id="91216-121">Header</span><span class="sxs-lookup"><span data-stu-id="91216-121">Header</span></span>|<span data-ttu-id="91216-122">Wert</span><span class="sxs-lookup"><span data-stu-id="91216-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91216-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="91216-123">Authorization</span></span>|<span data-ttu-id="91216-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="91216-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91216-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="91216-125">Accept</span></span>|<span data-ttu-id="91216-126">application/json</span><span class="sxs-lookup"><span data-stu-id="91216-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91216-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="91216-127">Request body</span></span>
<span data-ttu-id="91216-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="91216-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="91216-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="91216-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="91216-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="91216-130">Property</span></span>|<span data-ttu-id="91216-131">Typ</span><span class="sxs-lookup"><span data-stu-id="91216-131">Type</span></span>|<span data-ttu-id="91216-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91216-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91216-133">assignments</span><span class="sxs-lookup"><span data-stu-id="91216-133">assignments</span></span>|<span data-ttu-id="91216-134">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="91216-134">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="91216-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="91216-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="91216-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="91216-136">Response</span></span>
<span data-ttu-id="91216-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="91216-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="91216-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="91216-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="91216-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="91216-139">Request</span></span>
<span data-ttu-id="91216-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="91216-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="91216-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="91216-141">Response</span></span>
<span data-ttu-id="91216-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="91216-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





