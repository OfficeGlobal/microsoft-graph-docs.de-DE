---
title: ImportedWindowsAutopilotDeviceIdentityUpload aktualisieren
description: Aktualisieren der Eigenschaften eines importedWindowsAutopilotDeviceIdentityUpload-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 558cc0552694ad40f3088fbac8a3b3c60b73fd9a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250719"
---
# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="9bdad-103">ImportedWindowsAutopilotDeviceIdentityUpload aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9bdad-103">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="9bdad-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9bdad-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bdad-105">Aktualisieren der Eigenschaften eines [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9bdad-105">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bdad-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9bdad-106">Prerequisites</span></span>
<span data-ttu-id="9bdad-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9bdad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9bdad-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9bdad-109">Permission type</span></span>|<span data-ttu-id="9bdad-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9bdad-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bdad-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9bdad-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9bdad-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bdad-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9bdad-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9bdad-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bdad-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9bdad-114">Not supported.</span></span>|
|<span data-ttu-id="9bdad-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9bdad-115">Application</span></span>|<span data-ttu-id="9bdad-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9bdad-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bdad-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9bdad-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="9bdad-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9bdad-118">Request headers</span></span>
|<span data-ttu-id="9bdad-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9bdad-119">Header</span></span>|<span data-ttu-id="9bdad-120">Wert</span><span class="sxs-lookup"><span data-stu-id="9bdad-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bdad-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bdad-121">Authorization</span></span>|<span data-ttu-id="9bdad-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9bdad-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bdad-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9bdad-123">Accept</span></span>|<span data-ttu-id="9bdad-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9bdad-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bdad-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9bdad-125">Request body</span></span>
<span data-ttu-id="9bdad-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="9bdad-126">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="9bdad-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="9bdad-127">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="9bdad-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9bdad-128">Property</span></span>|<span data-ttu-id="9bdad-129">Typ</span><span class="sxs-lookup"><span data-stu-id="9bdad-129">Type</span></span>|<span data-ttu-id="9bdad-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9bdad-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bdad-131">id</span><span class="sxs-lookup"><span data-stu-id="9bdad-131">id</span></span>|<span data-ttu-id="9bdad-132">String</span><span class="sxs-lookup"><span data-stu-id="9bdad-132">String</span></span>|<span data-ttu-id="9bdad-133">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="9bdad-133">The GUID for the object</span></span>|
|<span data-ttu-id="9bdad-134">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="9bdad-134">createdDateTimeUtc</span></span>|<span data-ttu-id="9bdad-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bdad-135">DateTimeOffset</span></span>|<span data-ttu-id="9bdad-136">DateTime, wenn die Entität erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="9bdad-136">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="9bdad-137">status</span><span class="sxs-lookup"><span data-stu-id="9bdad-137">status</span></span>|[<span data-ttu-id="9bdad-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="9bdad-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="9bdad-139">Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="9bdad-139">Upload status.</span></span> <span data-ttu-id="9bdad-140">Mögliche Werte sind: `noUpload`, `pending`, `complete` und `error`.</span><span class="sxs-lookup"><span data-stu-id="9bdad-140">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="9bdad-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="9bdad-141">Response</span></span>
<span data-ttu-id="9bdad-142">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9bdad-142">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bdad-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9bdad-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bdad-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9bdad-144">Request</span></span>
<span data-ttu-id="9bdad-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9bdad-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9bdad-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="9bdad-146">Response</span></span>
<span data-ttu-id="9bdad-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9bdad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



