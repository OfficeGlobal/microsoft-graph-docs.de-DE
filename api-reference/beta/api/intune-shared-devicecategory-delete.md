---
title: deviceCategory löschen
description: Löscht ein deviceCategory-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cff7aa7b7c290b37358cef413a0b17e54e91c83c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978829"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="59fb9-103">deviceCategory löschen</span><span class="sxs-lookup"><span data-stu-id="59fb9-103">Delete deviceCategory</span></span>

> <span data-ttu-id="59fb9-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="59fb9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="59fb9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="59fb9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="59fb9-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="59fb9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59fb9-107">Löscht ein [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="59fb9-107">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="59fb9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="59fb9-108">Prerequisites</span></span>
<span data-ttu-id="59fb9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59fb9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59fb9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="59fb9-111">Permission type</span></span>|<span data-ttu-id="59fb9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="59fb9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59fb9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="59fb9-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="59fb9-114">&nbsp; &nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="59fb9-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="59fb9-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59fb9-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="59fb9-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="59fb9-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59fb9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="59fb9-117">Not supported.</span></span>|
|<span data-ttu-id="59fb9-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="59fb9-118">Application</span></span>|<span data-ttu-id="59fb9-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="59fb9-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59fb9-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="59fb9-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="59fb9-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="59fb9-121">Request headers</span></span>
|<span data-ttu-id="59fb9-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="59fb9-122">Header</span></span>|<span data-ttu-id="59fb9-123">Wert</span><span class="sxs-lookup"><span data-stu-id="59fb9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59fb9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="59fb9-124">Authorization</span></span>|<span data-ttu-id="59fb9-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="59fb9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59fb9-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="59fb9-126">Accept</span></span>|<span data-ttu-id="59fb9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="59fb9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59fb9-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="59fb9-128">Request body</span></span>
<span data-ttu-id="59fb9-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="59fb9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59fb9-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="59fb9-130">Response</span></span>
<span data-ttu-id="59fb9-131">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="59fb9-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="59fb9-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="59fb9-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="59fb9-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="59fb9-133">Request</span></span>

<span data-ttu-id="59fb9-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="59fb9-134">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="59fb9-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="59fb9-135">Response</span></span>

<span data-ttu-id="59fb9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="59fb9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



