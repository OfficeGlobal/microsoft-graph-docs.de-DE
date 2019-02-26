---
title: ImportedWindowsAutopilotDeviceIdentityUpload erstellen
description: Erstellen eines neuen importedWindowsAutopilotDeviceIdentityUpload-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2fd4230b0ecdb4279380255b1fa62cbe697a4843
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264393"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="a70cf-103">ImportedWindowsAutopilotDeviceIdentityUpload erstellen</span><span class="sxs-lookup"><span data-stu-id="a70cf-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="a70cf-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a70cf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a70cf-105">Erstellen eines neuen [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a70cf-105">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a70cf-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a70cf-106">Prerequisites</span></span>
<span data-ttu-id="a70cf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a70cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a70cf-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a70cf-109">Permission type</span></span>|<span data-ttu-id="a70cf-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a70cf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a70cf-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a70cf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a70cf-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a70cf-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a70cf-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a70cf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a70cf-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a70cf-114">Not supported.</span></span>|
|<span data-ttu-id="a70cf-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a70cf-115">Application</span></span>|<span data-ttu-id="a70cf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a70cf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a70cf-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a70cf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="a70cf-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a70cf-118">Request headers</span></span>
|<span data-ttu-id="a70cf-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a70cf-119">Header</span></span>|<span data-ttu-id="a70cf-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a70cf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a70cf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a70cf-121">Authorization</span></span>|<span data-ttu-id="a70cf-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a70cf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a70cf-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a70cf-123">Accept</span></span>|<span data-ttu-id="a70cf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a70cf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a70cf-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a70cf-125">Request body</span></span>
<span data-ttu-id="a70cf-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das importedWindowsAutopilotDeviceIdentityUpload-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="a70cf-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="a70cf-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der importedWindowsAutopilotDeviceIdentityUpload erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a70cf-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="a70cf-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a70cf-128">Property</span></span>|<span data-ttu-id="a70cf-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a70cf-129">Type</span></span>|<span data-ttu-id="a70cf-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a70cf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a70cf-131">id</span><span class="sxs-lookup"><span data-stu-id="a70cf-131">id</span></span>|<span data-ttu-id="a70cf-132">String</span><span class="sxs-lookup"><span data-stu-id="a70cf-132">String</span></span>|<span data-ttu-id="a70cf-133">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="a70cf-133">The GUID for the object</span></span>|
|<span data-ttu-id="a70cf-134">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="a70cf-134">createdDateTimeUtc</span></span>|<span data-ttu-id="a70cf-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a70cf-135">DateTimeOffset</span></span>|<span data-ttu-id="a70cf-136">DateTime, wenn die Entität erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="a70cf-136">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="a70cf-137">status</span><span class="sxs-lookup"><span data-stu-id="a70cf-137">status</span></span>|[<span data-ttu-id="a70cf-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="a70cf-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="a70cf-139">Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="a70cf-139">Upload status.</span></span> <span data-ttu-id="a70cf-140">Mögliche Werte sind: `noUpload`, `pending`, `complete` und `error`.</span><span class="sxs-lookup"><span data-stu-id="a70cf-140">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="a70cf-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="a70cf-141">Response</span></span>
<span data-ttu-id="a70cf-142">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a70cf-142">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a70cf-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a70cf-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="a70cf-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a70cf-144">Request</span></span>
<span data-ttu-id="a70cf-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a70cf-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a70cf-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="a70cf-146">Response</span></span>
<span data-ttu-id="a70cf-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a70cf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



