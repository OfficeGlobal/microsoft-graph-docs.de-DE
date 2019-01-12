---
title: Aktion „commit“
description: Diese Aktion führt einen Commit für eine Datei einer App aus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0b225a74f3a273e9e5dda7752b94e4a445d9794c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952342"
---
# <a name="commit-action"></a><span data-ttu-id="52658-103">Aktion „commit“</span><span class="sxs-lookup"><span data-stu-id="52658-103">commit action</span></span>

> <span data-ttu-id="52658-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="52658-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52658-105">Diese Aktion führt einen Commit für eine Datei einer App aus.</span><span class="sxs-lookup"><span data-stu-id="52658-105">Commits a file of a given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="52658-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="52658-106">Prerequisites</span></span>
<span data-ttu-id="52658-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52658-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52658-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="52658-109">Permission type</span></span>|<span data-ttu-id="52658-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="52658-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52658-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="52658-111">Delegated (work or school account)</span></span>|<span data-ttu-id="52658-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52658-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="52658-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="52658-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52658-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="52658-114">Not supported.</span></span>|
|<span data-ttu-id="52658-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="52658-115">Application</span></span>|<span data-ttu-id="52658-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="52658-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52658-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="52658-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="52658-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="52658-118">Request headers</span></span>
|<span data-ttu-id="52658-119">Header</span><span class="sxs-lookup"><span data-stu-id="52658-119">Header</span></span>|<span data-ttu-id="52658-120">Wert</span><span class="sxs-lookup"><span data-stu-id="52658-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52658-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="52658-121">Authorization</span></span>|<span data-ttu-id="52658-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="52658-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52658-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="52658-123">Accept</span></span>|<span data-ttu-id="52658-124">application/json</span><span class="sxs-lookup"><span data-stu-id="52658-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52658-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="52658-125">Request body</span></span>
<span data-ttu-id="52658-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="52658-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="52658-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="52658-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="52658-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="52658-128">Property</span></span>|<span data-ttu-id="52658-129">Typ</span><span class="sxs-lookup"><span data-stu-id="52658-129">Type</span></span>|<span data-ttu-id="52658-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52658-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52658-131">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="52658-131">fileEncryptionInfo</span></span>|[<span data-ttu-id="52658-132">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="52658-132">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="52658-133">Schlüssel des Parameters mit den Dateiverschlüsselungsinformationen</span><span class="sxs-lookup"><span data-stu-id="52658-133">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="52658-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="52658-134">Response</span></span>
<span data-ttu-id="52658-135">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="52658-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="52658-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="52658-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="52658-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="52658-137">Request</span></span>
<span data-ttu-id="52658-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="52658-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit

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

### <a name="response"></a><span data-ttu-id="52658-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="52658-139">Response</span></span>
<span data-ttu-id="52658-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="52658-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



