---
title: renewUpload-Aktion
description: Erneuert den SAS-URI für einen Anwendungsdateiupload.
ms.openlocfilehash: b2f94ddf98a41dd54348694fa65badd646e12d15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017143"
---
# <a name="renewupload-action"></a><span data-ttu-id="d7580-103">renewUpload-Aktion</span><span class="sxs-lookup"><span data-stu-id="d7580-103">renewUpload action</span></span>

> <span data-ttu-id="d7580-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d7580-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7580-105">Erneuert den SAS-URI für einen Anwendungsdateiupload.</span><span class="sxs-lookup"><span data-stu-id="d7580-105">Renews the SAS URI for an application file upload.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d7580-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d7580-106">Prerequisites</span></span>
<span data-ttu-id="d7580-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7580-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7580-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d7580-109">Permission type</span></span>|<span data-ttu-id="d7580-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d7580-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7580-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d7580-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d7580-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7580-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d7580-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d7580-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7580-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7580-114">Not supported.</span></span>|
|<span data-ttu-id="d7580-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d7580-115">Application</span></span>|<span data-ttu-id="d7580-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7580-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7580-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7580-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/renewUpload
```

## <a name="request-headers"></a><span data-ttu-id="d7580-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d7580-118">Request headers</span></span>
|<span data-ttu-id="d7580-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d7580-119">Header</span></span>|<span data-ttu-id="d7580-120">Wert</span><span class="sxs-lookup"><span data-stu-id="d7580-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7580-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7580-121">Authorization</span></span>|<span data-ttu-id="d7580-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d7580-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7580-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d7580-123">Accept</span></span>|<span data-ttu-id="d7580-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d7580-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7580-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d7580-125">Request body</span></span>
<span data-ttu-id="d7580-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d7580-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7580-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7580-127">Response</span></span>
<span data-ttu-id="d7580-128">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="d7580-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d7580-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d7580-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d7580-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7580-130">Request</span></span>
<span data-ttu-id="d7580-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d7580-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/renewUpload
```

### <a name="response"></a><span data-ttu-id="d7580-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7580-132">Response</span></span>
<span data-ttu-id="d7580-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d7580-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



