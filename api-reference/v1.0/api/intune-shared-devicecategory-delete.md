---
title: deviceCategory löschen
description: Löscht ein deviceCategory-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 35dffc1c280caeb10007dbf11d390ac7487d4a61
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30249970"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="7f081-103">deviceCategory löschen</span><span class="sxs-lookup"><span data-stu-id="7f081-103">Delete deviceCategory</span></span>

> <span data-ttu-id="7f081-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7f081-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f081-105">Löscht ein [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="7f081-105">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f081-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7f081-106">Prerequisites</span></span>
<span data-ttu-id="7f081-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f081-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f081-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7f081-109">Permission type</span></span>|<span data-ttu-id="7f081-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7f081-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f081-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7f081-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7f081-112">&nbsp; &nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="7f081-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7f081-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f081-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7f081-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7f081-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f081-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f081-115">Not supported.</span></span>|
|<span data-ttu-id="7f081-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7f081-116">Application</span></span>|<span data-ttu-id="7f081-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f081-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f081-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f081-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="7f081-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7f081-119">Request headers</span></span>
|<span data-ttu-id="7f081-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7f081-120">Header</span></span>|<span data-ttu-id="7f081-121">Wert</span><span class="sxs-lookup"><span data-stu-id="7f081-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f081-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f081-122">Authorization</span></span>|<span data-ttu-id="7f081-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7f081-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f081-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7f081-124">Accept</span></span>|<span data-ttu-id="7f081-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7f081-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f081-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7f081-126">Request body</span></span>
<span data-ttu-id="7f081-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7f081-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f081-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f081-128">Response</span></span>
<span data-ttu-id="7f081-129">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7f081-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7f081-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7f081-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f081-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f081-131">Request</span></span>
<span data-ttu-id="7f081-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7f081-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="7f081-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f081-133">Response</span></span>
<span data-ttu-id="7f081-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7f081-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



