---
title: ImportedWindowsAutopilotDeviceIdentityUpload erstellen
description: Erstellen eines neuen importedWindowsAutopilotDeviceIdentityUpload-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 124b54760c6fc77668c16562a865912257a3e8e7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169902"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="dd1f4-103">ImportedWindowsAutopilotDeviceIdentityUpload erstellen</span><span class="sxs-lookup"><span data-stu-id="dd1f4-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="dd1f4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dd1f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd1f4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="dd1f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd1f4-106">Erstellen eines neuen [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="dd1f4-106">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd1f4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dd1f4-107">Prerequisites</span></span>
<span data-ttu-id="dd1f4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dd1f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dd1f4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dd1f4-110">Permission type</span></span>|<span data-ttu-id="dd1f4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dd1f4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd1f4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dd1f4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dd1f4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd1f4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dd1f4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dd1f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd1f4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd1f4-115">Not supported.</span></span>|
|<span data-ttu-id="dd1f4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dd1f4-116">Application</span></span>|<span data-ttu-id="dd1f4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd1f4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd1f4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd1f4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="dd1f4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dd1f4-119">Request headers</span></span>
|<span data-ttu-id="dd1f4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dd1f4-120">Header</span></span>|<span data-ttu-id="dd1f4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="dd1f4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd1f4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd1f4-122">Authorization</span></span>|<span data-ttu-id="dd1f4-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dd1f4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd1f4-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dd1f4-124">Accept</span></span>|<span data-ttu-id="dd1f4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dd1f4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd1f4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dd1f4-126">Request body</span></span>
<span data-ttu-id="dd1f4-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das importedWindowsAutopilotDeviceIdentityUpload-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="dd1f4-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="dd1f4-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der importedWindowsAutopilotDeviceIdentityUpload erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="dd1f4-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="dd1f4-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dd1f4-129">Property</span></span>|<span data-ttu-id="dd1f4-130">Typ</span><span class="sxs-lookup"><span data-stu-id="dd1f4-130">Type</span></span>|<span data-ttu-id="dd1f4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd1f4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd1f4-132">id</span><span class="sxs-lookup"><span data-stu-id="dd1f4-132">id</span></span>|<span data-ttu-id="dd1f4-133">String</span><span class="sxs-lookup"><span data-stu-id="dd1f4-133">String</span></span>|<span data-ttu-id="dd1f4-134">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="dd1f4-134">The GUID for the object</span></span>|
|<span data-ttu-id="dd1f4-135">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="dd1f4-135">createdDateTimeUtc</span></span>|<span data-ttu-id="dd1f4-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd1f4-136">DateTimeOffset</span></span>|<span data-ttu-id="dd1f4-137">DateTime, wenn die Entität erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="dd1f4-137">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="dd1f4-138">status</span><span class="sxs-lookup"><span data-stu-id="dd1f4-138">status</span></span>|[<span data-ttu-id="dd1f4-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="dd1f4-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="dd1f4-140">Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="dd1f4-140">Upload status.</span></span> <span data-ttu-id="dd1f4-141">Mögliche Werte sind: `noUpload`, `pending`, `complete` und `error`.</span><span class="sxs-lookup"><span data-stu-id="dd1f4-141">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="dd1f4-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd1f4-142">Response</span></span>
<span data-ttu-id="dd1f4-143">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="dd1f4-143">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd1f4-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dd1f4-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd1f4-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd1f4-145">Request</span></span>
<span data-ttu-id="dd1f4-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dd1f4-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dd1f4-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd1f4-147">Response</span></span>
<span data-ttu-id="dd1f4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd1f4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




