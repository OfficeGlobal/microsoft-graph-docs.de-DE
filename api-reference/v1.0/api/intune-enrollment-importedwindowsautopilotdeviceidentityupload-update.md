---
title: ImportedWindowsAutopilotDeviceIdentityUpload aktualisieren
description: Aktualisieren Sie die Eigenschaften eines ImportedWindowsAutopilotDeviceIdentityUpload-Objekts.
author: tfitzmac
ms.openlocfilehash: 4fb2274fdb172b6aeceba11364a6460cbe5cce58
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324416"
---
# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="2acbb-103">ImportedWindowsAutopilotDeviceIdentityUpload aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2acbb-103">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="2acbb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2acbb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2acbb-105">Aktualisieren Sie die Eigenschaften eines [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2acbb-105">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2acbb-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2acbb-106">Prerequisites</span></span>
<span data-ttu-id="2acbb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2acbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2acbb-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2acbb-109">Permission type</span></span>|<span data-ttu-id="2acbb-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2acbb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2acbb-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2acbb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2acbb-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2acbb-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2acbb-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2acbb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2acbb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2acbb-114">Not supported.</span></span>|
|<span data-ttu-id="2acbb-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2acbb-115">Application</span></span>|<span data-ttu-id="2acbb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2acbb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2acbb-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2acbb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="2acbb-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2acbb-118">Request headers</span></span>
|<span data-ttu-id="2acbb-119">Header</span><span class="sxs-lookup"><span data-stu-id="2acbb-119">Header</span></span>|<span data-ttu-id="2acbb-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2acbb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2acbb-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2acbb-121">Authorization</span></span>|<span data-ttu-id="2acbb-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2acbb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2acbb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2acbb-123">Accept</span></span>|<span data-ttu-id="2acbb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2acbb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2acbb-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2acbb-125">Request body</span></span>
<span data-ttu-id="2acbb-126">Geben Sie im Textkörper Anforderung für das Objekt [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="2acbb-126">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="2acbb-127">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="2acbb-127">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="2acbb-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2acbb-128">Property</span></span>|<span data-ttu-id="2acbb-129">Typ</span><span class="sxs-lookup"><span data-stu-id="2acbb-129">Type</span></span>|<span data-ttu-id="2acbb-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2acbb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2acbb-131">id</span><span class="sxs-lookup"><span data-stu-id="2acbb-131">id</span></span>|<span data-ttu-id="2acbb-132">String</span><span class="sxs-lookup"><span data-stu-id="2acbb-132">String</span></span>|<span data-ttu-id="2acbb-133">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="2acbb-133">The GUID for the object</span></span>|
|<span data-ttu-id="2acbb-134">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="2acbb-134">createdDateTimeUtc</span></span>|<span data-ttu-id="2acbb-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2acbb-135">DateTimeOffset</span></span>|<span data-ttu-id="2acbb-136">DateTime, wenn die Entität erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="2acbb-136">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="2acbb-137">status</span><span class="sxs-lookup"><span data-stu-id="2acbb-137">status</span></span>|[<span data-ttu-id="2acbb-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="2acbb-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="2acbb-139">Hochladen Sie Status.</span><span class="sxs-lookup"><span data-stu-id="2acbb-139">Upload status.</span></span> <span data-ttu-id="2acbb-140">Mögliche Werte sind: `noUpload`, `pending`, `complete` und `error`.</span><span class="sxs-lookup"><span data-stu-id="2acbb-140">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="2acbb-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="2acbb-141">Response</span></span>
<span data-ttu-id="2acbb-142">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2acbb-142">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2acbb-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2acbb-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="2acbb-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2acbb-144">Request</span></span>
<span data-ttu-id="2acbb-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2acbb-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2acbb-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="2acbb-146">Response</span></span>
<span data-ttu-id="2acbb-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2acbb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



