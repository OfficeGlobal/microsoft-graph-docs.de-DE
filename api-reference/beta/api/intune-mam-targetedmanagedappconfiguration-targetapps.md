---
title: targetApps-Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7121e8901e9c9c94196b1d7441c29b7ecc9fd6fb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945342"
---
# <a name="targetapps-action"></a><span data-ttu-id="5af29-103">targetApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="5af29-103">targetApps action</span></span>

> <span data-ttu-id="5af29-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5af29-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5af29-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5af29-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5af29-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5af29-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5af29-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="5af29-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5af29-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5af29-108">Prerequisites</span></span>
<span data-ttu-id="5af29-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5af29-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5af29-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5af29-111">Permission type</span></span>|<span data-ttu-id="5af29-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5af29-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5af29-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5af29-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5af29-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5af29-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5af29-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5af29-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5af29-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5af29-116">Not supported.</span></span>|
|<span data-ttu-id="5af29-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5af29-117">Application</span></span>|<span data-ttu-id="5af29-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5af29-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5af29-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5af29-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="5af29-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5af29-120">Request headers</span></span>
|<span data-ttu-id="5af29-121">Header</span><span class="sxs-lookup"><span data-stu-id="5af29-121">Header</span></span>|<span data-ttu-id="5af29-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5af29-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5af29-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5af29-123">Authorization</span></span>|<span data-ttu-id="5af29-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5af29-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5af29-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5af29-125">Accept</span></span>|<span data-ttu-id="5af29-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5af29-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5af29-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5af29-127">Request body</span></span>
<span data-ttu-id="5af29-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="5af29-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5af29-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="5af29-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5af29-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5af29-130">Property</span></span>|<span data-ttu-id="5af29-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5af29-131">Type</span></span>|<span data-ttu-id="5af29-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5af29-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5af29-133">Apps</span><span class="sxs-lookup"><span data-stu-id="5af29-133">apps</span></span>|<span data-ttu-id="5af29-134">Sammlung von Objekten des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5af29-134">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="5af29-135">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="5af29-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5af29-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="5af29-136">Response</span></span>
<span data-ttu-id="5af29-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="5af29-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5af29-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5af29-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="5af29-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5af29-139">Request</span></span>
<span data-ttu-id="5af29-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5af29-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps

Content-type: application/json
Content-length: 286

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="5af29-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="5af29-141">Response</span></span>
<span data-ttu-id="5af29-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5af29-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





