---
title: Aktion „commit“
description: Diese Aktion führt einen Commit für eine Datei einer App aus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1ef052518a7ac464ee605cfd0779785441ce4cb9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401474"
---
# <a name="commit-action"></a><span data-ttu-id="e1b5c-103">Aktion „commit“</span><span class="sxs-lookup"><span data-stu-id="e1b5c-103">commit action</span></span>

> <span data-ttu-id="e1b5c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e1b5c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e1b5c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e1b5c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1b5c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e1b5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1b5c-107">Diese Aktion führt einen Commit für eine Datei einer App aus.</span><span class="sxs-lookup"><span data-stu-id="e1b5c-107">Commits a file of a given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1b5c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e1b5c-108">Prerequisites</span></span>
<span data-ttu-id="e1b5c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e1b5c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e1b5c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e1b5c-111">Permission type</span></span>|<span data-ttu-id="e1b5c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e1b5c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1b5c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e1b5c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1b5c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1b5c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e1b5c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e1b5c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1b5c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1b5c-116">Not supported.</span></span>|
|<span data-ttu-id="e1b5c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e1b5c-117">Application</span></span>|<span data-ttu-id="e1b5c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1b5c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1b5c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1b5c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="e1b5c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e1b5c-120">Request headers</span></span>
|<span data-ttu-id="e1b5c-121">Header</span><span class="sxs-lookup"><span data-stu-id="e1b5c-121">Header</span></span>|<span data-ttu-id="e1b5c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e1b5c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1b5c-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e1b5c-123">Authorization</span></span>|<span data-ttu-id="e1b5c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e1b5c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1b5c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e1b5c-125">Accept</span></span>|<span data-ttu-id="e1b5c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1b5c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1b5c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e1b5c-127">Request body</span></span>
<span data-ttu-id="e1b5c-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="e1b5c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e1b5c-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="e1b5c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e1b5c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e1b5c-130">Property</span></span>|<span data-ttu-id="e1b5c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e1b5c-131">Type</span></span>|<span data-ttu-id="e1b5c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1b5c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1b5c-133">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="e1b5c-133">fileEncryptionInfo</span></span>|[<span data-ttu-id="e1b5c-134">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="e1b5c-134">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="e1b5c-135">Schlüssel des Parameters mit den Dateiverschlüsselungsinformationen</span><span class="sxs-lookup"><span data-stu-id="e1b5c-135">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="e1b5c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1b5c-136">Response</span></span>
<span data-ttu-id="e1b5c-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="e1b5c-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e1b5c-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e1b5c-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1b5c-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1b5c-139">Request</span></span>
<span data-ttu-id="e1b5c-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e1b5c-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e1b5c-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1b5c-141">Response</span></span>
<span data-ttu-id="e1b5c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1b5c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




