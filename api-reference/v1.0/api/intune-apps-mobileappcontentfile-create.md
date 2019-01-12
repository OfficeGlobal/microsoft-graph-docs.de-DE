---
title: Erstellen von „mobileAppContentFile“
description: Diese Methode erstellt ein neues Objekt des Typs mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9061a3b44d80d7182af321502afa84a3a8cb68fb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972635"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="acb99-103">Erstellen von „mobileAppContentFile“</span><span class="sxs-lookup"><span data-stu-id="acb99-103">Create mobileAppContentFile</span></span>

> <span data-ttu-id="acb99-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="acb99-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="acb99-105">Diese Methode erstellt ein neues Objekt des Typs [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="acb99-105">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="acb99-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="acb99-106">Prerequisites</span></span>
<span data-ttu-id="acb99-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acb99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acb99-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="acb99-109">Permission type</span></span>|<span data-ttu-id="acb99-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="acb99-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acb99-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="acb99-111">Delegated (work or school account)</span></span>|<span data-ttu-id="acb99-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acb99-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="acb99-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="acb99-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acb99-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="acb99-114">Not supported.</span></span>|
|<span data-ttu-id="acb99-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="acb99-115">Application</span></span>|<span data-ttu-id="acb99-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="acb99-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acb99-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="acb99-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="acb99-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="acb99-118">Request headers</span></span>
|<span data-ttu-id="acb99-119">Header</span><span class="sxs-lookup"><span data-stu-id="acb99-119">Header</span></span>|<span data-ttu-id="acb99-120">Wert</span><span class="sxs-lookup"><span data-stu-id="acb99-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acb99-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="acb99-121">Authorization</span></span>|<span data-ttu-id="acb99-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="acb99-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acb99-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="acb99-123">Accept</span></span>|<span data-ttu-id="acb99-124">application/json</span><span class="sxs-lookup"><span data-stu-id="acb99-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acb99-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="acb99-125">Request body</span></span>
<span data-ttu-id="acb99-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mobileAppContentFile“ an.</span><span class="sxs-lookup"><span data-stu-id="acb99-126">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="acb99-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mobileAppContentFile“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="acb99-127">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="acb99-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="acb99-128">Property</span></span>|<span data-ttu-id="acb99-129">Typ</span><span class="sxs-lookup"><span data-stu-id="acb99-129">Type</span></span>|<span data-ttu-id="acb99-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="acb99-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acb99-131">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="acb99-131">azureStorageUri</span></span>|<span data-ttu-id="acb99-132">String</span><span class="sxs-lookup"><span data-stu-id="acb99-132">String</span></span>|<span data-ttu-id="acb99-133">Azure Storage-URI</span><span class="sxs-lookup"><span data-stu-id="acb99-133">The Azure Storage URI.</span></span>|
|<span data-ttu-id="acb99-134">isCommitted</span><span class="sxs-lookup"><span data-stu-id="acb99-134">isCommitted</span></span>|<span data-ttu-id="acb99-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="acb99-135">Boolean</span></span>|<span data-ttu-id="acb99-136">Wert, der angibt, ob für die Datei ein Commit ausgeführt wurde</span><span class="sxs-lookup"><span data-stu-id="acb99-136">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="acb99-137">id</span><span class="sxs-lookup"><span data-stu-id="acb99-137">id</span></span>|<span data-ttu-id="acb99-138">String</span><span class="sxs-lookup"><span data-stu-id="acb99-138">String</span></span>|<span data-ttu-id="acb99-139">ID der Datei</span><span class="sxs-lookup"><span data-stu-id="acb99-139">The File Id.</span></span>|
|<span data-ttu-id="acb99-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="acb99-140">createdDateTime</span></span>|<span data-ttu-id="acb99-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acb99-141">DateTimeOffset</span></span>|<span data-ttu-id="acb99-142">Datum und Uhrzeit der Erstellung der Datei</span><span class="sxs-lookup"><span data-stu-id="acb99-142">The time the file was created.</span></span>|
|<span data-ttu-id="acb99-143">name</span><span class="sxs-lookup"><span data-stu-id="acb99-143">name</span></span>|<span data-ttu-id="acb99-144">String</span><span class="sxs-lookup"><span data-stu-id="acb99-144">String</span></span>|<span data-ttu-id="acb99-145">Name der Datei</span><span class="sxs-lookup"><span data-stu-id="acb99-145">the file name.</span></span>|
|<span data-ttu-id="acb99-146">size</span><span class="sxs-lookup"><span data-stu-id="acb99-146">size</span></span>|<span data-ttu-id="acb99-147">Int64</span><span class="sxs-lookup"><span data-stu-id="acb99-147">Int64</span></span>|<span data-ttu-id="acb99-148">Größe der Datei vor der Verschlüsselung</span><span class="sxs-lookup"><span data-stu-id="acb99-148">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="acb99-149">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="acb99-149">sizeEncrypted</span></span>|<span data-ttu-id="acb99-150">Int64</span><span class="sxs-lookup"><span data-stu-id="acb99-150">Int64</span></span>|<span data-ttu-id="acb99-151">Größe der Datei nach der Verschlüsselung</span><span class="sxs-lookup"><span data-stu-id="acb99-151">The size of the file after encryption.</span></span>|
|<span data-ttu-id="acb99-152">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="acb99-152">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="acb99-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acb99-153">DateTimeOffset</span></span>|<span data-ttu-id="acb99-154">Datum und Uhrzeit des Ablaufs des Azure Storage-URI</span><span class="sxs-lookup"><span data-stu-id="acb99-154">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="acb99-155">manifest</span><span class="sxs-lookup"><span data-stu-id="acb99-155">manifest</span></span>|<span data-ttu-id="acb99-156">Binär</span><span class="sxs-lookup"><span data-stu-id="acb99-156">Binary</span></span>|<span data-ttu-id="acb99-157">Manifestinformationen</span><span class="sxs-lookup"><span data-stu-id="acb99-157">The manifest information.</span></span>|
|<span data-ttu-id="acb99-158">uploadState</span><span class="sxs-lookup"><span data-stu-id="acb99-158">uploadState</span></span>|[<span data-ttu-id="acb99-159">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="acb99-159">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="acb99-160">Status der aktuellen Uploadanforderung.</span><span class="sxs-lookup"><span data-stu-id="acb99-160">The state of the current upload request.</span></span> <span data-ttu-id="acb99-161">Mögliche Werte sind: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed` und `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="acb99-161">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="acb99-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="acb99-162">Response</span></span>
<span data-ttu-id="acb99-163">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="acb99-163">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acb99-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="acb99-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="acb99-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="acb99-165">Request</span></span>
<span data-ttu-id="acb99-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="acb99-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="acb99-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="acb99-167">Response</span></span>
<span data-ttu-id="acb99-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="acb99-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



