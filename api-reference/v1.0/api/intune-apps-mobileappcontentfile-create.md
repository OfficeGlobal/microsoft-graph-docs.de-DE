---
title: Erstellen von „mobileAppContentFile“
description: Diese Methode erstellt ein neues Objekt des Typs mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 657c6047b1c3de0b66af411c6b890cbf01520824
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261376"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="da352-103">Erstellen von „mobileAppContentFile“</span><span class="sxs-lookup"><span data-stu-id="da352-103">Create mobileAppContentFile</span></span>

> <span data-ttu-id="da352-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="da352-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da352-105">Diese Methode erstellt ein neues Objekt des Typs [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="da352-105">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da352-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="da352-106">Prerequisites</span></span>
<span data-ttu-id="da352-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="da352-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="da352-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="da352-109">Permission type</span></span>|<span data-ttu-id="da352-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="da352-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da352-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="da352-111">Delegated (work or school account)</span></span>|<span data-ttu-id="da352-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da352-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="da352-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="da352-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da352-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da352-114">Not supported.</span></span>|
|<span data-ttu-id="da352-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="da352-115">Application</span></span>|<span data-ttu-id="da352-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da352-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da352-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="da352-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="da352-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="da352-118">Request headers</span></span>
|<span data-ttu-id="da352-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="da352-119">Header</span></span>|<span data-ttu-id="da352-120">Wert</span><span class="sxs-lookup"><span data-stu-id="da352-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da352-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="da352-121">Authorization</span></span>|<span data-ttu-id="da352-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="da352-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da352-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="da352-123">Accept</span></span>|<span data-ttu-id="da352-124">application/json</span><span class="sxs-lookup"><span data-stu-id="da352-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da352-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="da352-125">Request body</span></span>
<span data-ttu-id="da352-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mobileAppContentFile“ an.</span><span class="sxs-lookup"><span data-stu-id="da352-126">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="da352-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mobileAppContentFile“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="da352-127">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="da352-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="da352-128">Property</span></span>|<span data-ttu-id="da352-129">Typ</span><span class="sxs-lookup"><span data-stu-id="da352-129">Type</span></span>|<span data-ttu-id="da352-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da352-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da352-131">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="da352-131">azureStorageUri</span></span>|<span data-ttu-id="da352-132">String</span><span class="sxs-lookup"><span data-stu-id="da352-132">String</span></span>|<span data-ttu-id="da352-133">Azure Storage-URI</span><span class="sxs-lookup"><span data-stu-id="da352-133">The Azure Storage URI.</span></span>|
|<span data-ttu-id="da352-134">isCommitted</span><span class="sxs-lookup"><span data-stu-id="da352-134">isCommitted</span></span>|<span data-ttu-id="da352-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="da352-135">Boolean</span></span>|<span data-ttu-id="da352-136">Wert, der angibt, ob für die Datei ein Commit ausgeführt wurde</span><span class="sxs-lookup"><span data-stu-id="da352-136">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="da352-137">id</span><span class="sxs-lookup"><span data-stu-id="da352-137">id</span></span>|<span data-ttu-id="da352-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da352-138">String</span></span>|<span data-ttu-id="da352-139">ID der Datei</span><span class="sxs-lookup"><span data-stu-id="da352-139">The File Id.</span></span>|
|<span data-ttu-id="da352-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da352-140">createdDateTime</span></span>|<span data-ttu-id="da352-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da352-141">DateTimeOffset</span></span>|<span data-ttu-id="da352-142">Datum und Uhrzeit der Erstellung der Datei</span><span class="sxs-lookup"><span data-stu-id="da352-142">The time the file was created.</span></span>|
|<span data-ttu-id="da352-143">name</span><span class="sxs-lookup"><span data-stu-id="da352-143">name</span></span>|<span data-ttu-id="da352-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da352-144">String</span></span>|<span data-ttu-id="da352-145">Name der Datei</span><span class="sxs-lookup"><span data-stu-id="da352-145">the file name.</span></span>|
|<span data-ttu-id="da352-146">size</span><span class="sxs-lookup"><span data-stu-id="da352-146">size</span></span>|<span data-ttu-id="da352-147">Int64</span><span class="sxs-lookup"><span data-stu-id="da352-147">Int64</span></span>|<span data-ttu-id="da352-148">Größe der Datei vor der Verschlüsselung</span><span class="sxs-lookup"><span data-stu-id="da352-148">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="da352-149">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="da352-149">sizeEncrypted</span></span>|<span data-ttu-id="da352-150">Int64</span><span class="sxs-lookup"><span data-stu-id="da352-150">Int64</span></span>|<span data-ttu-id="da352-151">Größe der Datei nach der Verschlüsselung</span><span class="sxs-lookup"><span data-stu-id="da352-151">The size of the file after encryption.</span></span>|
|<span data-ttu-id="da352-152">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="da352-152">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="da352-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da352-153">DateTimeOffset</span></span>|<span data-ttu-id="da352-154">Datum und Uhrzeit des Ablaufs des Azure Storage-URI</span><span class="sxs-lookup"><span data-stu-id="da352-154">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="da352-155">manifest</span><span class="sxs-lookup"><span data-stu-id="da352-155">manifest</span></span>|<span data-ttu-id="da352-156">Binär</span><span class="sxs-lookup"><span data-stu-id="da352-156">Binary</span></span>|<span data-ttu-id="da352-157">Manifestinformationen</span><span class="sxs-lookup"><span data-stu-id="da352-157">The manifest information.</span></span>|
|<span data-ttu-id="da352-158">uploadState</span><span class="sxs-lookup"><span data-stu-id="da352-158">uploadState</span></span>|[<span data-ttu-id="da352-159">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="da352-159">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="da352-160">Status der aktuellen Uploadanforderung.</span><span class="sxs-lookup"><span data-stu-id="da352-160">The state of the current upload request.</span></span> <span data-ttu-id="da352-161">Mögliche Werte sind: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed` und `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="da352-161">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="da352-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="da352-162">Response</span></span>
<span data-ttu-id="da352-163">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="da352-163">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da352-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="da352-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="da352-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="da352-165">Request</span></span>
<span data-ttu-id="da352-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="da352-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError"
}
```

### <a name="response"></a><span data-ttu-id="da352-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="da352-167">Response</span></span>
<span data-ttu-id="da352-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="da352-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 450

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError"
}
```



