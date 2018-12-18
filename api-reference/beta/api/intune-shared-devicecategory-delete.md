---
title: deviceCategory löschen
description: Löscht ein deviceCategory-Objekt.
author: tfitzmac
ms.openlocfilehash: ea8f8860f79cc0c14e985c64a1457b114d30b6b4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321294"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="fdf76-103">deviceCategory löschen</span><span class="sxs-lookup"><span data-stu-id="fdf76-103">Delete deviceCategory</span></span>

> <span data-ttu-id="fdf76-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fdf76-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fdf76-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fdf76-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fdf76-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fdf76-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fdf76-107">Löscht ein [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="fdf76-107">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fdf76-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fdf76-108">Prerequisites</span></span>
<span data-ttu-id="fdf76-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdf76-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdf76-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fdf76-111">Permission type</span></span>|<span data-ttu-id="fdf76-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fdf76-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdf76-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fdf76-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fdf76-114">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="fdf76-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="fdf76-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdf76-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fdf76-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fdf76-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdf76-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fdf76-117">Not supported.</span></span>|
|<span data-ttu-id="fdf76-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fdf76-118">Application</span></span>|<span data-ttu-id="fdf76-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fdf76-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdf76-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fdf76-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="fdf76-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fdf76-121">Request headers</span></span>
|<span data-ttu-id="fdf76-122">Header</span><span class="sxs-lookup"><span data-stu-id="fdf76-122">Header</span></span>|<span data-ttu-id="fdf76-123">Wert</span><span class="sxs-lookup"><span data-stu-id="fdf76-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdf76-124">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fdf76-124">Authorization</span></span>|<span data-ttu-id="fdf76-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fdf76-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdf76-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fdf76-126">Accept</span></span>|<span data-ttu-id="fdf76-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fdf76-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdf76-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fdf76-128">Request body</span></span>
<span data-ttu-id="fdf76-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fdf76-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdf76-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="fdf76-130">Response</span></span>
<span data-ttu-id="fdf76-131">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fdf76-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fdf76-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fdf76-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdf76-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fdf76-133">Request</span></span>

<span data-ttu-id="fdf76-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fdf76-134">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="fdf76-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="fdf76-135">Response</span></span>

<span data-ttu-id="fdf76-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fdf76-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



