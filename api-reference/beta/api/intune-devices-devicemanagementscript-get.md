---
title: Abrufen von deviceManagementScript
description: Lesen Sie Eigenschaften und Beziehungen des DeviceManagementScript-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: db4fbc951983e5d6fb44ce65ae55de366e91957e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926519"
---
# <a name="get-devicemanagementscript"></a><span data-ttu-id="3f280-103">Abrufen von deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="3f280-103">Get deviceManagementScript</span></span>

> <span data-ttu-id="3f280-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3f280-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f280-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3f280-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3f280-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3f280-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3f280-107">Lesen Sie Eigenschaften und Beziehungen des [DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3f280-107">Read properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3f280-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3f280-108">Prerequisites</span></span>
<span data-ttu-id="3f280-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f280-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f280-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3f280-111">Permission type</span></span>|<span data-ttu-id="3f280-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3f280-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f280-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3f280-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f280-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f280-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3f280-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3f280-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f280-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3f280-116">Not supported.</span></span>|
|<span data-ttu-id="3f280-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3f280-117">Application</span></span>|<span data-ttu-id="3f280-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3f280-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f280-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3f280-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3f280-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3f280-120">Optional query parameters</span></span>
<span data-ttu-id="3f280-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3f280-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3f280-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3f280-122">Request headers</span></span>
|<span data-ttu-id="3f280-123">Header</span><span class="sxs-lookup"><span data-stu-id="3f280-123">Header</span></span>|<span data-ttu-id="3f280-124">Wert</span><span class="sxs-lookup"><span data-stu-id="3f280-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f280-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f280-125">Authorization</span></span>|<span data-ttu-id="3f280-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3f280-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f280-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3f280-127">Accept</span></span>|<span data-ttu-id="3f280-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3f280-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f280-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3f280-129">Request body</span></span>
<span data-ttu-id="3f280-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3f280-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f280-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="3f280-131">Response</span></span>
<span data-ttu-id="3f280-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3f280-132">If successful, this method returns a `200 OK` response code and [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f280-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3f280-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="3f280-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3f280-134">Request</span></span>
<span data-ttu-id="3f280-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3f280-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

### <a name="response"></a><span data-ttu-id="3f280-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="3f280-136">Response</span></span>
<span data-ttu-id="3f280-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3f280-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 575

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScript",
    "id": "59ea4525-4525-59ea-2545-ea592545ea59",
    "displayName": "Display Name value",
    "description": "Description value",
    "runSchedule": {
      "@odata.type": "microsoft.graph.runSchedule"
    },
    "scriptContent": "c2NyaXB0Q29udGVudA==",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "runAsAccount": "user",
    "enforceSignatureCheck": true,
    "fileName": "File Name value"
  }
}
```





