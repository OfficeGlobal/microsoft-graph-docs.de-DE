---
title: Funktion getUserIdsWithFlaggedAppRegistration
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 65848b44c0b4228d1df4c5e7ea0e0024e16598eb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139326"
---
# <a name="getuseridswithflaggedappregistration-function"></a><span data-ttu-id="f9b68-103">Funktion getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="f9b68-103">getUserIdsWithFlaggedAppRegistration function</span></span>

> <span data-ttu-id="f9b68-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f9b68-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9b68-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f9b68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9b68-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f9b68-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9b68-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f9b68-107">Prerequisites</span></span>
<span data-ttu-id="f9b68-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f9b68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f9b68-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f9b68-110">Permission type</span></span>|<span data-ttu-id="f9b68-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f9b68-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9b68-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f9b68-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9b68-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9b68-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f9b68-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f9b68-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9b68-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9b68-115">Not supported.</span></span>|
|<span data-ttu-id="f9b68-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f9b68-116">Application</span></span>|<span data-ttu-id="f9b68-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9b68-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9b68-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9b68-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

## <a name="request-headers"></a><span data-ttu-id="f9b68-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f9b68-119">Request headers</span></span>
|<span data-ttu-id="f9b68-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f9b68-120">Header</span></span>|<span data-ttu-id="f9b68-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f9b68-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9b68-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9b68-122">Authorization</span></span>|<span data-ttu-id="f9b68-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f9b68-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9b68-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f9b68-124">Accept</span></span>|<span data-ttu-id="f9b68-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9b68-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9b68-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f9b68-126">Request body</span></span>
<span data-ttu-id="f9b68-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f9b68-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9b68-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9b68-128">Response</span></span>
<span data-ttu-id="f9b68-129">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f9b68-129">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9b68-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f9b68-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9b68-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9b68-131">Request</span></span>
<span data-ttu-id="f9b68-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f9b68-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

### <a name="response"></a><span data-ttu-id="f9b68-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9b68-133">Response</span></span>
<span data-ttu-id="f9b68-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f9b68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




