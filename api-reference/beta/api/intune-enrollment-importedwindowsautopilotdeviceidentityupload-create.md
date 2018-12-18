---
title: Erstellen von importedWindowsAutopilotDeviceIdentityUpload
description: Erstellen eines neuen ImportedWindowsAutopilotDeviceIdentityUpload-Objekts.
author: tfitzmac
ms.openlocfilehash: f4042129f33b617546e32d46435179af5c9d3282
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354810"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="10c3d-103">Erstellen von importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="10c3d-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="10c3d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="10c3d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10c3d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="10c3d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10c3d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="10c3d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10c3d-107">Erstellen eines neuen [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="10c3d-107">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="10c3d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="10c3d-108">Prerequisites</span></span>
<span data-ttu-id="10c3d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10c3d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10c3d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="10c3d-111">Permission type</span></span>|<span data-ttu-id="10c3d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="10c3d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10c3d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="10c3d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10c3d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10c3d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="10c3d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="10c3d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10c3d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10c3d-116">Not supported.</span></span>|
|<span data-ttu-id="10c3d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="10c3d-117">Application</span></span>|<span data-ttu-id="10c3d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10c3d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10c3d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="10c3d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="10c3d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="10c3d-120">Request headers</span></span>
|<span data-ttu-id="10c3d-121">Header</span><span class="sxs-lookup"><span data-stu-id="10c3d-121">Header</span></span>|<span data-ttu-id="10c3d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="10c3d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10c3d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="10c3d-123">Authorization</span></span>|<span data-ttu-id="10c3d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="10c3d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10c3d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="10c3d-125">Accept</span></span>|<span data-ttu-id="10c3d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="10c3d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10c3d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="10c3d-127">Request body</span></span>
<span data-ttu-id="10c3d-128">Geben Sie im Textkörper Anforderung für das Objekt ImportedWindowsAutopilotDeviceIdentityUpload eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="10c3d-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="10c3d-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die ImportedWindowsAutopilotDeviceIdentityUpload erstellen.</span><span class="sxs-lookup"><span data-stu-id="10c3d-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="10c3d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="10c3d-130">Property</span></span>|<span data-ttu-id="10c3d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="10c3d-131">Type</span></span>|<span data-ttu-id="10c3d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10c3d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10c3d-133">id</span><span class="sxs-lookup"><span data-stu-id="10c3d-133">id</span></span>|<span data-ttu-id="10c3d-134">String</span><span class="sxs-lookup"><span data-stu-id="10c3d-134">String</span></span>|<span data-ttu-id="10c3d-135">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="10c3d-135">The GUID for the object</span></span>|
|<span data-ttu-id="10c3d-136">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="10c3d-136">createdDateTimeUtc</span></span>|<span data-ttu-id="10c3d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10c3d-137">DateTimeOffset</span></span>|<span data-ttu-id="10c3d-138">DateTime, wenn die Entität erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="10c3d-138">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="10c3d-139">status</span><span class="sxs-lookup"><span data-stu-id="10c3d-139">status</span></span>|[<span data-ttu-id="10c3d-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="10c3d-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="10c3d-141">Hochladen Sie Status.</span><span class="sxs-lookup"><span data-stu-id="10c3d-141">Upload status.</span></span> <span data-ttu-id="10c3d-142">Mögliche Werte sind: `noUpload`, `pending`, `complete` und `error`.</span><span class="sxs-lookup"><span data-stu-id="10c3d-142">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="10c3d-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="10c3d-143">Response</span></span>
<span data-ttu-id="10c3d-144">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="10c3d-144">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10c3d-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="10c3d-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="10c3d-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="10c3d-146">Request</span></span>
<span data-ttu-id="10c3d-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="10c3d-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="10c3d-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="10c3d-148">Response</span></span>
<span data-ttu-id="10c3d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10c3d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





