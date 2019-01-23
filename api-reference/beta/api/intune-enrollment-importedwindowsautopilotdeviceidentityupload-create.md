---
title: Erstellen von importedWindowsAutopilotDeviceIdentityUpload
description: Erstellen eines neuen ImportedWindowsAutopilotDeviceIdentityUpload-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e47e3c8545335f0f34511e7d0b87bf2bd54d2162
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396812"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="59ca1-103">Erstellen von importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="59ca1-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="59ca1-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="59ca1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="59ca1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="59ca1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="59ca1-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="59ca1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59ca1-107">Erstellen eines neuen [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="59ca1-107">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59ca1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="59ca1-108">Prerequisites</span></span>
<span data-ttu-id="59ca1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="59ca1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="59ca1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="59ca1-111">Permission type</span></span>|<span data-ttu-id="59ca1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="59ca1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59ca1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="59ca1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="59ca1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59ca1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="59ca1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="59ca1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59ca1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="59ca1-116">Not supported.</span></span>|
|<span data-ttu-id="59ca1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="59ca1-117">Application</span></span>|<span data-ttu-id="59ca1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="59ca1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59ca1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="59ca1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="59ca1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="59ca1-120">Request headers</span></span>
|<span data-ttu-id="59ca1-121">Header</span><span class="sxs-lookup"><span data-stu-id="59ca1-121">Header</span></span>|<span data-ttu-id="59ca1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="59ca1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59ca1-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="59ca1-123">Authorization</span></span>|<span data-ttu-id="59ca1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="59ca1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59ca1-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="59ca1-125">Accept</span></span>|<span data-ttu-id="59ca1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="59ca1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59ca1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="59ca1-127">Request body</span></span>
<span data-ttu-id="59ca1-128">Geben Sie im Textkörper Anforderung für das Objekt ImportedWindowsAutopilotDeviceIdentityUpload eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="59ca1-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="59ca1-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die ImportedWindowsAutopilotDeviceIdentityUpload erstellen.</span><span class="sxs-lookup"><span data-stu-id="59ca1-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="59ca1-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="59ca1-130">Property</span></span>|<span data-ttu-id="59ca1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="59ca1-131">Type</span></span>|<span data-ttu-id="59ca1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="59ca1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59ca1-133">id</span><span class="sxs-lookup"><span data-stu-id="59ca1-133">id</span></span>|<span data-ttu-id="59ca1-134">String</span><span class="sxs-lookup"><span data-stu-id="59ca1-134">String</span></span>|<span data-ttu-id="59ca1-135">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="59ca1-135">The GUID for the object</span></span>|
|<span data-ttu-id="59ca1-136">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="59ca1-136">createdDateTimeUtc</span></span>|<span data-ttu-id="59ca1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59ca1-137">DateTimeOffset</span></span>|<span data-ttu-id="59ca1-138">DateTime, wenn die Entität erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="59ca1-138">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="59ca1-139">status</span><span class="sxs-lookup"><span data-stu-id="59ca1-139">status</span></span>|[<span data-ttu-id="59ca1-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="59ca1-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="59ca1-141">Hochladen Sie Status.</span><span class="sxs-lookup"><span data-stu-id="59ca1-141">Upload status.</span></span> <span data-ttu-id="59ca1-142">Mögliche Werte sind: `noUpload`, `pending`, `complete` und `error`.</span><span class="sxs-lookup"><span data-stu-id="59ca1-142">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="59ca1-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="59ca1-143">Response</span></span>
<span data-ttu-id="59ca1-144">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="59ca1-144">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59ca1-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="59ca1-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="59ca1-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="59ca1-146">Request</span></span>
<span data-ttu-id="59ca1-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="59ca1-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="59ca1-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="59ca1-148">Response</span></span>
<span data-ttu-id="59ca1-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="59ca1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




