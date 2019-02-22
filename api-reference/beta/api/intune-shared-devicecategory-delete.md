---
title: deviceCategory löschen
description: Löscht ein deviceCategory-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3f02bcad5c43ef787ad53ea59bb88853074db452
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161754"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="f8f38-103">deviceCategory löschen</span><span class="sxs-lookup"><span data-stu-id="f8f38-103">Delete deviceCategory</span></span>

> <span data-ttu-id="f8f38-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="f8f38-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f8f38-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f8f38-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8f38-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f8f38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8f38-107">Löscht ein [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="f8f38-107">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8f38-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f8f38-108">Prerequisites</span></span>
<span data-ttu-id="f8f38-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8f38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="f8f38-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f8f38-111">Permission type</span></span>|<span data-ttu-id="f8f38-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f8f38-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8f38-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f8f38-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f8f38-114">&nbsp; &nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="f8f38-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="f8f38-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8f38-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f8f38-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f8f38-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8f38-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8f38-117">Not supported.</span></span>|
|<span data-ttu-id="f8f38-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f8f38-118">Application</span></span>|<span data-ttu-id="f8f38-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8f38-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8f38-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8f38-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="f8f38-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f8f38-121">Request headers</span></span>
|<span data-ttu-id="f8f38-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f8f38-122">Header</span></span>|<span data-ttu-id="f8f38-123">Wert</span><span class="sxs-lookup"><span data-stu-id="f8f38-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8f38-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8f38-124">Authorization</span></span>|<span data-ttu-id="f8f38-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f8f38-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8f38-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f8f38-126">Accept</span></span>|<span data-ttu-id="f8f38-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f8f38-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8f38-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f8f38-128">Request body</span></span>
<span data-ttu-id="f8f38-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f8f38-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8f38-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8f38-130">Response</span></span>
<span data-ttu-id="f8f38-131">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f8f38-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f8f38-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f8f38-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8f38-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8f38-133">Request</span></span>

<span data-ttu-id="f8f38-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f8f38-134">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="f8f38-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8f38-135">Response</span></span>

<span data-ttu-id="f8f38-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f8f38-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



