---
title: ImportedWindowsAutopilotDeviceIdentityUpload aktualisieren
description: Aktualisieren Sie die Eigenschaften eines ImportedWindowsAutopilotDeviceIdentityUpload-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ba5c58b220419cff73e317dcc24e0690eff71b0d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991061"
---
# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="2f475-103">ImportedWindowsAutopilotDeviceIdentityUpload aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2f475-103">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="2f475-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2f475-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f475-105">Aktualisieren Sie die Eigenschaften eines [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2f475-105">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f475-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2f475-106">Prerequisites</span></span>
<span data-ttu-id="2f475-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f475-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f475-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2f475-109">Permission type</span></span>|<span data-ttu-id="2f475-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2f475-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f475-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2f475-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2f475-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f475-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2f475-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2f475-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f475-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f475-114">Not supported.</span></span>|
|<span data-ttu-id="2f475-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2f475-115">Application</span></span>|<span data-ttu-id="2f475-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f475-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f475-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f475-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="2f475-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f475-118">Request headers</span></span>
|<span data-ttu-id="2f475-119">Header</span><span class="sxs-lookup"><span data-stu-id="2f475-119">Header</span></span>|<span data-ttu-id="2f475-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2f475-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f475-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f475-121">Authorization</span></span>|<span data-ttu-id="2f475-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2f475-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f475-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2f475-123">Accept</span></span>|<span data-ttu-id="2f475-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2f475-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f475-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f475-125">Request body</span></span>
<span data-ttu-id="2f475-126">Geben Sie im Textkörper Anforderung für das Objekt [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="2f475-126">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="2f475-127">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="2f475-127">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="2f475-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2f475-128">Property</span></span>|<span data-ttu-id="2f475-129">Typ</span><span class="sxs-lookup"><span data-stu-id="2f475-129">Type</span></span>|<span data-ttu-id="2f475-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f475-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f475-131">id</span><span class="sxs-lookup"><span data-stu-id="2f475-131">id</span></span>|<span data-ttu-id="2f475-132">String</span><span class="sxs-lookup"><span data-stu-id="2f475-132">String</span></span>|<span data-ttu-id="2f475-133">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="2f475-133">The GUID for the object</span></span>|
|<span data-ttu-id="2f475-134">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="2f475-134">createdDateTimeUtc</span></span>|<span data-ttu-id="2f475-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f475-135">DateTimeOffset</span></span>|<span data-ttu-id="2f475-136">DateTime, wenn die Entität erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="2f475-136">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="2f475-137">status</span><span class="sxs-lookup"><span data-stu-id="2f475-137">status</span></span>|[<span data-ttu-id="2f475-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="2f475-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="2f475-139">Hochladen Sie Status.</span><span class="sxs-lookup"><span data-stu-id="2f475-139">Upload status.</span></span> <span data-ttu-id="2f475-140">Mögliche Werte sind: `noUpload`, `pending`, `complete` und `error`.</span><span class="sxs-lookup"><span data-stu-id="2f475-140">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="2f475-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f475-141">Response</span></span>
<span data-ttu-id="2f475-142">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2f475-142">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f475-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f475-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f475-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f475-144">Request</span></span>
<span data-ttu-id="2f475-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f475-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="2f475-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f475-146">Response</span></span>
<span data-ttu-id="2f475-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f475-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "8d639524-9524-8d63-2495-638d2495638d",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```



