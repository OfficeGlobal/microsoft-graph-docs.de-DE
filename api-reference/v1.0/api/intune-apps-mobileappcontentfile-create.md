---
title: Erstellen von „mobileAppContentFile“
description: Diese Methode erstellt ein neues Objekt des Typs mobileAppContentFile.
author: tfitzmac
ms.openlocfilehash: 9fba589cdb04d6c0258b18cb17da4c96441123e2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331507"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="40931-103">Erstellen von „mobileAppContentFile“</span><span class="sxs-lookup"><span data-stu-id="40931-103">Create mobileAppContentFile</span></span>

> <span data-ttu-id="40931-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="40931-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40931-105">Diese Methode erstellt ein neues Objekt des Typs [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="40931-105">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40931-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="40931-106">Prerequisites</span></span>
<span data-ttu-id="40931-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40931-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40931-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="40931-109">Permission type</span></span>|<span data-ttu-id="40931-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="40931-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40931-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="40931-111">Delegated (work or school account)</span></span>|<span data-ttu-id="40931-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40931-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="40931-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="40931-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40931-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40931-114">Not supported.</span></span>|
|<span data-ttu-id="40931-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="40931-115">Application</span></span>|<span data-ttu-id="40931-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40931-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40931-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="40931-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="40931-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="40931-118">Request headers</span></span>
|<span data-ttu-id="40931-119">Header</span><span class="sxs-lookup"><span data-stu-id="40931-119">Header</span></span>|<span data-ttu-id="40931-120">Wert</span><span class="sxs-lookup"><span data-stu-id="40931-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40931-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="40931-121">Authorization</span></span>|<span data-ttu-id="40931-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="40931-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40931-123">Accept</span><span class="sxs-lookup"><span data-stu-id="40931-123">Accept</span></span>|<span data-ttu-id="40931-124">application/json</span><span class="sxs-lookup"><span data-stu-id="40931-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40931-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="40931-125">Request body</span></span>
<span data-ttu-id="40931-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mobileAppContentFile“ an.</span><span class="sxs-lookup"><span data-stu-id="40931-126">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="40931-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mobileAppContentFile“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="40931-127">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="40931-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="40931-128">Property</span></span>|<span data-ttu-id="40931-129">Typ</span><span class="sxs-lookup"><span data-stu-id="40931-129">Type</span></span>|<span data-ttu-id="40931-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40931-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40931-131">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="40931-131">azureStorageUri</span></span>|<span data-ttu-id="40931-132">String</span><span class="sxs-lookup"><span data-stu-id="40931-132">String</span></span>|<span data-ttu-id="40931-133">Azure Storage-URI</span><span class="sxs-lookup"><span data-stu-id="40931-133">The Azure Storage URI.</span></span>|
|<span data-ttu-id="40931-134">isCommitted</span><span class="sxs-lookup"><span data-stu-id="40931-134">isCommitted</span></span>|<span data-ttu-id="40931-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="40931-135">Boolean</span></span>|<span data-ttu-id="40931-136">Wert, der angibt, ob für die Datei ein Commit ausgeführt wurde</span><span class="sxs-lookup"><span data-stu-id="40931-136">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="40931-137">id</span><span class="sxs-lookup"><span data-stu-id="40931-137">id</span></span>|<span data-ttu-id="40931-138">String</span><span class="sxs-lookup"><span data-stu-id="40931-138">String</span></span>|<span data-ttu-id="40931-139">ID der Datei</span><span class="sxs-lookup"><span data-stu-id="40931-139">The File Id.</span></span>|
|<span data-ttu-id="40931-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40931-140">createdDateTime</span></span>|<span data-ttu-id="40931-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40931-141">DateTimeOffset</span></span>|<span data-ttu-id="40931-142">Datum und Uhrzeit der Erstellung der Datei</span><span class="sxs-lookup"><span data-stu-id="40931-142">The time the file was created.</span></span>|
|<span data-ttu-id="40931-143">name</span><span class="sxs-lookup"><span data-stu-id="40931-143">name</span></span>|<span data-ttu-id="40931-144">String</span><span class="sxs-lookup"><span data-stu-id="40931-144">String</span></span>|<span data-ttu-id="40931-145">Name der Datei</span><span class="sxs-lookup"><span data-stu-id="40931-145">the file name.</span></span>|
|<span data-ttu-id="40931-146">size</span><span class="sxs-lookup"><span data-stu-id="40931-146">size</span></span>|<span data-ttu-id="40931-147">Int64</span><span class="sxs-lookup"><span data-stu-id="40931-147">Int64</span></span>|<span data-ttu-id="40931-148">Größe der Datei vor der Verschlüsselung</span><span class="sxs-lookup"><span data-stu-id="40931-148">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="40931-149">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="40931-149">sizeEncrypted</span></span>|<span data-ttu-id="40931-150">Int64</span><span class="sxs-lookup"><span data-stu-id="40931-150">Int64</span></span>|<span data-ttu-id="40931-151">Größe der Datei nach der Verschlüsselung</span><span class="sxs-lookup"><span data-stu-id="40931-151">The size of the file after encryption.</span></span>|
|<span data-ttu-id="40931-152">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="40931-152">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="40931-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40931-153">DateTimeOffset</span></span>|<span data-ttu-id="40931-154">Datum und Uhrzeit des Ablaufs des Azure Storage-URI</span><span class="sxs-lookup"><span data-stu-id="40931-154">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="40931-155">manifest</span><span class="sxs-lookup"><span data-stu-id="40931-155">manifest</span></span>|<span data-ttu-id="40931-156">Binär</span><span class="sxs-lookup"><span data-stu-id="40931-156">Binary</span></span>|<span data-ttu-id="40931-157">Manifestinformationen</span><span class="sxs-lookup"><span data-stu-id="40931-157">The manifest information.</span></span>|
|<span data-ttu-id="40931-158">uploadState</span><span class="sxs-lookup"><span data-stu-id="40931-158">uploadState</span></span>|[<span data-ttu-id="40931-159">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="40931-159">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="40931-160">Status der aktuellen Uploadanforderung.</span><span class="sxs-lookup"><span data-stu-id="40931-160">The state of the current upload request.</span></span> <span data-ttu-id="40931-161">Mögliche Werte sind: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed` und `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="40931-161">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="40931-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="40931-162">Response</span></span>
<span data-ttu-id="40931-163">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="40931-163">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40931-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40931-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="40931-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="40931-165">Request</span></span>
<span data-ttu-id="40931-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="40931-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="40931-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="40931-167">Response</span></span>
<span data-ttu-id="40931-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40931-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



