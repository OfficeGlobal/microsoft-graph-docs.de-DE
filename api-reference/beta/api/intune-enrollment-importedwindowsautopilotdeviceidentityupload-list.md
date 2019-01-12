---
title: Liste importedWindowsAutopilotDeviceIdentityUploads
description: Listeneigenschaften und Beziehungen der ImportedWindowsAutopilotDeviceIdentityUpload-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3d6867ac4d29741f5d223168606c1e5573525c41
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968988"
---
# <a name="list-importedwindowsautopilotdeviceidentityuploads"></a><span data-ttu-id="15827-103">Liste importedWindowsAutopilotDeviceIdentityUploads</span><span class="sxs-lookup"><span data-stu-id="15827-103">List importedWindowsAutopilotDeviceIdentityUploads</span></span>

> <span data-ttu-id="15827-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="15827-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15827-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15827-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15827-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="15827-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15827-107">Listeneigenschaften und Beziehungen der [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="15827-107">List properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="15827-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="15827-108">Prerequisites</span></span>
<span data-ttu-id="15827-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15827-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15827-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="15827-111">Permission type</span></span>|<span data-ttu-id="15827-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="15827-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15827-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="15827-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15827-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="15827-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="15827-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="15827-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15827-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15827-116">Not supported.</span></span>|
|<span data-ttu-id="15827-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="15827-117">Application</span></span>|<span data-ttu-id="15827-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15827-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15827-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="15827-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="15827-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="15827-120">Request headers</span></span>
|<span data-ttu-id="15827-121">Header</span><span class="sxs-lookup"><span data-stu-id="15827-121">Header</span></span>|<span data-ttu-id="15827-122">Wert</span><span class="sxs-lookup"><span data-stu-id="15827-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15827-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="15827-123">Authorization</span></span>|<span data-ttu-id="15827-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="15827-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15827-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="15827-125">Accept</span></span>|<span data-ttu-id="15827-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15827-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15827-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="15827-127">Request body</span></span>
<span data-ttu-id="15827-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="15827-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15827-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="15827-129">Response</span></span>
<span data-ttu-id="15827-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="15827-130">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15827-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="15827-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="15827-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15827-132">Request</span></span>
<span data-ttu-id="15827-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="15827-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

### <a name="response"></a><span data-ttu-id="15827-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="15827-134">Response</span></span>
<span data-ttu-id="15827-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15827-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
      "id": "8d639524-9524-8d63-2495-638d2495638d",
      "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
      "status": "pending"
    }
  ]
}
```





