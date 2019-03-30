---
title: ImportedWindowsAutopilotDeviceIdentityUpload aktualisieren
description: Aktualisieren der Eigenschaften eines importedWindowsAutopilotDeviceIdentityUpload-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 16d3e1377223a80db20403085562d736c44228ac
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969834"
---
# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="0d071-103">ImportedWindowsAutopilotDeviceIdentityUpload aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0d071-103">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="0d071-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0d071-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d071-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0d071-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d071-106">Aktualisieren der Eigenschaften eines [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0d071-106">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d071-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0d071-107">Prerequisites</span></span>
<span data-ttu-id="0d071-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d071-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d071-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0d071-110">Permission type</span></span>|<span data-ttu-id="0d071-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0d071-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d071-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0d071-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0d071-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d071-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0d071-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0d071-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d071-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d071-115">Not supported.</span></span>|
|<span data-ttu-id="0d071-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0d071-116">Application</span></span>|<span data-ttu-id="0d071-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d071-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d071-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d071-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="0d071-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0d071-119">Request headers</span></span>
|<span data-ttu-id="0d071-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0d071-120">Header</span></span>|<span data-ttu-id="0d071-121">Wert</span><span class="sxs-lookup"><span data-stu-id="0d071-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d071-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d071-122">Authorization</span></span>|<span data-ttu-id="0d071-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0d071-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d071-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0d071-124">Accept</span></span>|<span data-ttu-id="0d071-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0d071-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d071-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0d071-126">Request body</span></span>
<span data-ttu-id="0d071-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="0d071-127">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="0d071-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0d071-128">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="0d071-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0d071-129">Property</span></span>|<span data-ttu-id="0d071-130">Typ</span><span class="sxs-lookup"><span data-stu-id="0d071-130">Type</span></span>|<span data-ttu-id="0d071-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d071-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d071-132">id</span><span class="sxs-lookup"><span data-stu-id="0d071-132">id</span></span>|<span data-ttu-id="0d071-133">String</span><span class="sxs-lookup"><span data-stu-id="0d071-133">String</span></span>|<span data-ttu-id="0d071-134">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="0d071-134">The GUID for the object</span></span>|
|<span data-ttu-id="0d071-135">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="0d071-135">createdDateTimeUtc</span></span>|<span data-ttu-id="0d071-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d071-136">DateTimeOffset</span></span>|<span data-ttu-id="0d071-137">DateTime, wenn die Entität erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="0d071-137">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="0d071-138">status</span><span class="sxs-lookup"><span data-stu-id="0d071-138">status</span></span>|[<span data-ttu-id="0d071-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="0d071-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="0d071-140">Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="0d071-140">Upload status.</span></span> <span data-ttu-id="0d071-141">Mögliche Werte sind: `noUpload`, `pending`, `complete` und `error`.</span><span class="sxs-lookup"><span data-stu-id="0d071-141">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="0d071-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d071-142">Response</span></span>
<span data-ttu-id="0d071-143">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0d071-143">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d071-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0d071-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d071-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d071-145">Request</span></span>
<span data-ttu-id="0d071-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0d071-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="0d071-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d071-147">Response</span></span>
<span data-ttu-id="0d071-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d071-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




