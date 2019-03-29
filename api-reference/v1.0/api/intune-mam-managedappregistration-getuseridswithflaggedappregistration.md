---
title: Funktion getUserIdsWithFlaggedAppRegistration
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0fb55917b9172fa5836e44a864c1ba41e9e06371
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961224"
---
# <a name="getuseridswithflaggedappregistration-function"></a><span data-ttu-id="6fa7a-103">Funktion getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="6fa7a-103">getUserIdsWithFlaggedAppRegistration function</span></span>

> <span data-ttu-id="6fa7a-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6fa7a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fa7a-105">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="6fa7a-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fa7a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6fa7a-106">Prerequisites</span></span>
<span data-ttu-id="6fa7a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fa7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fa7a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6fa7a-109">Permission type</span></span>|<span data-ttu-id="6fa7a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6fa7a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fa7a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6fa7a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6fa7a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6fa7a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6fa7a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6fa7a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fa7a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6fa7a-114">Not supported.</span></span>|
|<span data-ttu-id="6fa7a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6fa7a-115">Application</span></span>|<span data-ttu-id="6fa7a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6fa7a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fa7a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6fa7a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

## <a name="request-headers"></a><span data-ttu-id="6fa7a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6fa7a-118">Request headers</span></span>
|<span data-ttu-id="6fa7a-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6fa7a-119">Header</span></span>|<span data-ttu-id="6fa7a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="6fa7a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fa7a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fa7a-121">Authorization</span></span>|<span data-ttu-id="6fa7a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6fa7a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fa7a-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6fa7a-123">Accept</span></span>|<span data-ttu-id="6fa7a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6fa7a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fa7a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6fa7a-125">Request body</span></span>
<span data-ttu-id="6fa7a-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6fa7a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fa7a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="6fa7a-127">Response</span></span>
<span data-ttu-id="6fa7a-128">Wenn die Funktion erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Zeichenfolge-Sammlung im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6fa7a-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fa7a-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6fa7a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fa7a-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6fa7a-130">Request</span></span>
<span data-ttu-id="6fa7a-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6fa7a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

### <a name="response"></a><span data-ttu-id="6fa7a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="6fa7a-132">Response</span></span>
<span data-ttu-id="6fa7a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6fa7a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": [
    "Get User Ids With Flagged App Registration value"
  ]
}
```



