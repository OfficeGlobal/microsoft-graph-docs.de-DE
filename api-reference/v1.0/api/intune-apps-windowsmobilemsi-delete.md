---
title: windowsMobileMSI löschen
description: Löscht Objekte des Typs windowsMobileMSI.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d14b1c01f0888a6c2f76f00d0fd7634460ee5dc3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960566"
---
# <a name="delete-windowsmobilemsi"></a><span data-ttu-id="9c36c-103">windowsMobileMSI löschen</span><span class="sxs-lookup"><span data-stu-id="9c36c-103">Delete windowsMobileMSI</span></span>

> <span data-ttu-id="9c36c-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9c36c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c36c-105">Löscht Objekte des Typs [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="9c36c-105">Deletes a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c36c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9c36c-106">Prerequisites</span></span>
<span data-ttu-id="9c36c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c36c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c36c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9c36c-109">Permission type</span></span>|<span data-ttu-id="9c36c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9c36c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c36c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9c36c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9c36c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c36c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9c36c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9c36c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c36c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c36c-114">Not supported.</span></span>|
|<span data-ttu-id="9c36c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9c36c-115">Application</span></span>|<span data-ttu-id="9c36c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c36c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c36c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c36c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="9c36c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9c36c-118">Request headers</span></span>
|<span data-ttu-id="9c36c-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9c36c-119">Header</span></span>|<span data-ttu-id="9c36c-120">Wert</span><span class="sxs-lookup"><span data-stu-id="9c36c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c36c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c36c-121">Authorization</span></span>|<span data-ttu-id="9c36c-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9c36c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c36c-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9c36c-123">Accept</span></span>|<span data-ttu-id="9c36c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9c36c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c36c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9c36c-125">Request body</span></span>
<span data-ttu-id="9c36c-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9c36c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c36c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c36c-127">Response</span></span>
<span data-ttu-id="9c36c-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9c36c-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9c36c-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9c36c-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c36c-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c36c-130">Request</span></span>
<span data-ttu-id="9c36c-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9c36c-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="9c36c-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c36c-132">Response</span></span>
<span data-ttu-id="9c36c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9c36c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



