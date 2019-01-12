---
title: Erstellen von importedWindowsAutopilotDeviceIdentityUpload
description: Erstellen eines neuen ImportedWindowsAutopilotDeviceIdentityUpload-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c99426a3f8f3f3568ea251532042a028a94d35cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923397"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="fa795-103">Erstellen von importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="fa795-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="fa795-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fa795-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa795-105">Erstellen eines neuen [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fa795-105">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fa795-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fa795-106">Prerequisites</span></span>
<span data-ttu-id="fa795-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa795-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa795-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fa795-109">Permission type</span></span>|<span data-ttu-id="fa795-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fa795-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa795-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fa795-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fa795-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa795-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fa795-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fa795-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa795-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa795-114">Not supported.</span></span>|
|<span data-ttu-id="fa795-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fa795-115">Application</span></span>|<span data-ttu-id="fa795-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa795-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa795-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa795-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="fa795-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa795-118">Request headers</span></span>
|<span data-ttu-id="fa795-119">Header</span><span class="sxs-lookup"><span data-stu-id="fa795-119">Header</span></span>|<span data-ttu-id="fa795-120">Wert</span><span class="sxs-lookup"><span data-stu-id="fa795-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa795-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa795-121">Authorization</span></span>|<span data-ttu-id="fa795-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fa795-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa795-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fa795-123">Accept</span></span>|<span data-ttu-id="fa795-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fa795-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa795-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fa795-125">Request body</span></span>
<span data-ttu-id="fa795-126">Geben Sie im Textkörper Anforderung für das Objekt ImportedWindowsAutopilotDeviceIdentityUpload eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="fa795-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="fa795-127">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die ImportedWindowsAutopilotDeviceIdentityUpload erstellen.</span><span class="sxs-lookup"><span data-stu-id="fa795-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="fa795-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa795-128">Property</span></span>|<span data-ttu-id="fa795-129">Typ</span><span class="sxs-lookup"><span data-stu-id="fa795-129">Type</span></span>|<span data-ttu-id="fa795-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa795-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa795-131">id</span><span class="sxs-lookup"><span data-stu-id="fa795-131">id</span></span>|<span data-ttu-id="fa795-132">String</span><span class="sxs-lookup"><span data-stu-id="fa795-132">String</span></span>|<span data-ttu-id="fa795-133">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="fa795-133">The GUID for the object</span></span>|
|<span data-ttu-id="fa795-134">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="fa795-134">createdDateTimeUtc</span></span>|<span data-ttu-id="fa795-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa795-135">DateTimeOffset</span></span>|<span data-ttu-id="fa795-136">DateTime, wenn die Entität erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="fa795-136">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="fa795-137">status</span><span class="sxs-lookup"><span data-stu-id="fa795-137">status</span></span>|[<span data-ttu-id="fa795-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="fa795-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="fa795-139">Hochladen Sie Status.</span><span class="sxs-lookup"><span data-stu-id="fa795-139">Upload status.</span></span> <span data-ttu-id="fa795-140">Mögliche Werte sind: `noUpload`, `pending`, `complete` und `error`.</span><span class="sxs-lookup"><span data-stu-id="fa795-140">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="fa795-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa795-141">Response</span></span>
<span data-ttu-id="fa795-142">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="fa795-142">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa795-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa795-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="fa795-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa795-144">Request</span></span>
<span data-ttu-id="fa795-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fa795-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="fa795-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa795-146">Response</span></span>
<span data-ttu-id="fa795-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa795-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "8d639524-9524-8d63-2495-638d2495638d",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```



