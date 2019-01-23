---
title: Liste importedWindowsAutopilotDeviceIdentityUploads
description: Listeneigenschaften und Beziehungen der ImportedWindowsAutopilotDeviceIdentityUpload-Objekte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 418f950eb2ecce3ac8400bbd022c937978c21b48
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416321"
---
# <a name="list-importedwindowsautopilotdeviceidentityuploads"></a><span data-ttu-id="a9f04-103">Liste importedWindowsAutopilotDeviceIdentityUploads</span><span class="sxs-lookup"><span data-stu-id="a9f04-103">List importedWindowsAutopilotDeviceIdentityUploads</span></span>

> <span data-ttu-id="a9f04-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a9f04-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a9f04-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a9f04-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9f04-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a9f04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9f04-107">Listeneigenschaften und Beziehungen der [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="a9f04-107">List properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9f04-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a9f04-108">Prerequisites</span></span>
<span data-ttu-id="a9f04-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a9f04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a9f04-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a9f04-111">Permission type</span></span>|<span data-ttu-id="a9f04-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a9f04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9f04-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a9f04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9f04-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9f04-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a9f04-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a9f04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9f04-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a9f04-116">Not supported.</span></span>|
|<span data-ttu-id="a9f04-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a9f04-117">Application</span></span>|<span data-ttu-id="a9f04-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a9f04-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9f04-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9f04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="a9f04-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a9f04-120">Request headers</span></span>
|<span data-ttu-id="a9f04-121">Header</span><span class="sxs-lookup"><span data-stu-id="a9f04-121">Header</span></span>|<span data-ttu-id="a9f04-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a9f04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9f04-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a9f04-123">Authorization</span></span>|<span data-ttu-id="a9f04-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a9f04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9f04-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a9f04-125">Accept</span></span>|<span data-ttu-id="a9f04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9f04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9f04-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a9f04-127">Request body</span></span>
<span data-ttu-id="a9f04-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a9f04-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9f04-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9f04-129">Response</span></span>
<span data-ttu-id="a9f04-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="a9f04-130">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9f04-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a9f04-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9f04-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9f04-132">Request</span></span>
<span data-ttu-id="a9f04-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a9f04-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

### <a name="response"></a><span data-ttu-id="a9f04-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9f04-134">Response</span></span>
<span data-ttu-id="a9f04-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a9f04-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




