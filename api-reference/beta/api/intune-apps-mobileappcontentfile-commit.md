---
title: Aktion „commit“
description: Diese Aktion führt einen Commit für eine Datei einer App aus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3fe5733450ee3990ce9ec3c95c1b34ab23d2a5a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962092"
---
# <a name="commit-action"></a><span data-ttu-id="1c74e-103">commit-Aktion</span><span class="sxs-lookup"><span data-stu-id="1c74e-103">commit action</span></span>

> <span data-ttu-id="1c74e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1c74e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c74e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1c74e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c74e-106">Diese Aktion führt einen Commit für eine Datei einer App aus.</span><span class="sxs-lookup"><span data-stu-id="1c74e-106">Commits a file of a given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c74e-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1c74e-107">Prerequisites</span></span>
<span data-ttu-id="1c74e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c74e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c74e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1c74e-110">Permission type</span></span>|<span data-ttu-id="1c74e-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1c74e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c74e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1c74e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1c74e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c74e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1c74e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1c74e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c74e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c74e-115">Not supported.</span></span>|
|<span data-ttu-id="1c74e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1c74e-116">Application</span></span>|<span data-ttu-id="1c74e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c74e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c74e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c74e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="1c74e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1c74e-119">Request headers</span></span>
|<span data-ttu-id="1c74e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1c74e-120">Header</span></span>|<span data-ttu-id="1c74e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1c74e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c74e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c74e-122">Authorization</span></span>|<span data-ttu-id="1c74e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1c74e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c74e-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1c74e-124">Accept</span></span>|<span data-ttu-id="1c74e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1c74e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c74e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1c74e-126">Request body</span></span>
<span data-ttu-id="1c74e-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="1c74e-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1c74e-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="1c74e-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1c74e-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1c74e-129">Property</span></span>|<span data-ttu-id="1c74e-130">Typ</span><span class="sxs-lookup"><span data-stu-id="1c74e-130">Type</span></span>|<span data-ttu-id="1c74e-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c74e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c74e-132">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="1c74e-132">fileEncryptionInfo</span></span>|[<span data-ttu-id="1c74e-133">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="1c74e-133">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="1c74e-134">Schlüssel des Parameters mit den Dateiverschlüsselungsinformationen</span><span class="sxs-lookup"><span data-stu-id="1c74e-134">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="1c74e-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c74e-135">Response</span></span>
<span data-ttu-id="1c74e-136">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c74e-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1c74e-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1c74e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c74e-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c74e-138">Request</span></span>
<span data-ttu-id="1c74e-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1c74e-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit

Content-type: application/json
Content-length: 399

{
  "fileEncryptionInfo": {
    "@odata.type": "microsoft.graph.fileEncryptionInfo",
    "encryptionKey": "ZW5jcnlwdGlvbktleQ==",
    "initializationVector": "aW5pdGlhbGl6YXRpb25WZWN0b3I=",
    "mac": "bWFj",
    "macKey": "bWFjS2V5",
    "profileIdentifier": "Profile Identifier value",
    "fileDigest": "ZmlsZURpZ2VzdA==",
    "fileDigestAlgorithm": "File Digest Algorithm value"
  }
}
```

### <a name="response"></a><span data-ttu-id="1c74e-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c74e-140">Response</span></span>
<span data-ttu-id="1c74e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c74e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




