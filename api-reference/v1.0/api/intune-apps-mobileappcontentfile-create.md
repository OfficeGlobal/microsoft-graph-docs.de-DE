---
title: Erstellen von „mobileAppContentFile“
description: Diese Methode erstellt ein neues Objekt des Typs mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2cef9b1d496ca4838f5e4f8be6f155180913118b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850827"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="16a98-103">Erstellen von „mobileAppContentFile“</span><span class="sxs-lookup"><span data-stu-id="16a98-103">Create mobileAppContentFile</span></span>

> <span data-ttu-id="16a98-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="16a98-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16a98-105">Diese Methode erstellt ein neues Objekt des Typs [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="16a98-105">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16a98-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="16a98-106">Prerequisites</span></span>
<span data-ttu-id="16a98-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16a98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16a98-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="16a98-109">Permission type</span></span>|<span data-ttu-id="16a98-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="16a98-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16a98-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="16a98-111">Delegated (work or school account)</span></span>|<span data-ttu-id="16a98-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16a98-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="16a98-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="16a98-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16a98-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16a98-114">Not supported.</span></span>|
|<span data-ttu-id="16a98-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="16a98-115">Application</span></span>|<span data-ttu-id="16a98-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16a98-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16a98-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="16a98-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="16a98-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="16a98-118">Request headers</span></span>
|<span data-ttu-id="16a98-119">Header</span><span class="sxs-lookup"><span data-stu-id="16a98-119">Header</span></span>|<span data-ttu-id="16a98-120">Wert</span><span class="sxs-lookup"><span data-stu-id="16a98-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16a98-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="16a98-121">Authorization</span></span>|<span data-ttu-id="16a98-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="16a98-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16a98-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="16a98-123">Accept</span></span>|<span data-ttu-id="16a98-124">application/json</span><span class="sxs-lookup"><span data-stu-id="16a98-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16a98-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="16a98-125">Request body</span></span>
<span data-ttu-id="16a98-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mobileAppContentFile“ an.</span><span class="sxs-lookup"><span data-stu-id="16a98-126">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="16a98-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mobileAppContentFile“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="16a98-127">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="16a98-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="16a98-128">Property</span></span>|<span data-ttu-id="16a98-129">Typ</span><span class="sxs-lookup"><span data-stu-id="16a98-129">Type</span></span>|<span data-ttu-id="16a98-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16a98-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16a98-131">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="16a98-131">azureStorageUri</span></span>|<span data-ttu-id="16a98-132">String</span><span class="sxs-lookup"><span data-stu-id="16a98-132">String</span></span>|<span data-ttu-id="16a98-133">Azure Storage-URI</span><span class="sxs-lookup"><span data-stu-id="16a98-133">The Azure Storage URI.</span></span>|
|<span data-ttu-id="16a98-134">isCommitted</span><span class="sxs-lookup"><span data-stu-id="16a98-134">isCommitted</span></span>|<span data-ttu-id="16a98-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="16a98-135">Boolean</span></span>|<span data-ttu-id="16a98-136">Wert, der angibt, ob für die Datei ein Commit ausgeführt wurde</span><span class="sxs-lookup"><span data-stu-id="16a98-136">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="16a98-137">id</span><span class="sxs-lookup"><span data-stu-id="16a98-137">id</span></span>|<span data-ttu-id="16a98-138">String</span><span class="sxs-lookup"><span data-stu-id="16a98-138">String</span></span>|<span data-ttu-id="16a98-139">ID der Datei</span><span class="sxs-lookup"><span data-stu-id="16a98-139">The File Id.</span></span>|
|<span data-ttu-id="16a98-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16a98-140">createdDateTime</span></span>|<span data-ttu-id="16a98-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16a98-141">DateTimeOffset</span></span>|<span data-ttu-id="16a98-142">Datum und Uhrzeit der Erstellung der Datei</span><span class="sxs-lookup"><span data-stu-id="16a98-142">The time the file was created.</span></span>|
|<span data-ttu-id="16a98-143">name</span><span class="sxs-lookup"><span data-stu-id="16a98-143">name</span></span>|<span data-ttu-id="16a98-144">String</span><span class="sxs-lookup"><span data-stu-id="16a98-144">String</span></span>|<span data-ttu-id="16a98-145">Name der Datei</span><span class="sxs-lookup"><span data-stu-id="16a98-145">the file name.</span></span>|
|<span data-ttu-id="16a98-146">size</span><span class="sxs-lookup"><span data-stu-id="16a98-146">size</span></span>|<span data-ttu-id="16a98-147">Int64</span><span class="sxs-lookup"><span data-stu-id="16a98-147">Int64</span></span>|<span data-ttu-id="16a98-148">Größe der Datei vor der Verschlüsselung</span><span class="sxs-lookup"><span data-stu-id="16a98-148">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="16a98-149">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="16a98-149">sizeEncrypted</span></span>|<span data-ttu-id="16a98-150">Int64</span><span class="sxs-lookup"><span data-stu-id="16a98-150">Int64</span></span>|<span data-ttu-id="16a98-151">Größe der Datei nach der Verschlüsselung</span><span class="sxs-lookup"><span data-stu-id="16a98-151">The size of the file after encryption.</span></span>|
|<span data-ttu-id="16a98-152">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="16a98-152">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="16a98-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16a98-153">DateTimeOffset</span></span>|<span data-ttu-id="16a98-154">Datum und Uhrzeit des Ablaufs des Azure Storage-URI</span><span class="sxs-lookup"><span data-stu-id="16a98-154">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="16a98-155">manifest</span><span class="sxs-lookup"><span data-stu-id="16a98-155">manifest</span></span>|<span data-ttu-id="16a98-156">Binär</span><span class="sxs-lookup"><span data-stu-id="16a98-156">Binary</span></span>|<span data-ttu-id="16a98-157">Manifestinformationen</span><span class="sxs-lookup"><span data-stu-id="16a98-157">The manifest information.</span></span>|
|<span data-ttu-id="16a98-158">uploadState</span><span class="sxs-lookup"><span data-stu-id="16a98-158">uploadState</span></span>|[<span data-ttu-id="16a98-159">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="16a98-159">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="16a98-160">Status der aktuellen Uploadanforderung.</span><span class="sxs-lookup"><span data-stu-id="16a98-160">The state of the current upload request.</span></span> <span data-ttu-id="16a98-161">Mögliche Werte sind: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed` und `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="16a98-161">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="16a98-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="16a98-162">Response</span></span>
<span data-ttu-id="16a98-163">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="16a98-163">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16a98-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="16a98-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="16a98-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="16a98-165">Request</span></span>
<span data-ttu-id="16a98-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="16a98-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="16a98-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="16a98-167">Response</span></span>
<span data-ttu-id="16a98-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="16a98-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



