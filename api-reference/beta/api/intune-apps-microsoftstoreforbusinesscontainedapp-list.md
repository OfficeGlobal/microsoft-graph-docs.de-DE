---
title: Liste microsoftStoreForBusinessContainedApps
description: Listeneigenschaften und Beziehungen der MicrosoftStoreForBusinessContainedApp-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3f03addc84b44c2bc796d76122a61f2f943c682f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813734"
---
# <a name="list-microsoftstoreforbusinesscontainedapps"></a><span data-ttu-id="e33a8-103">Liste microsoftStoreForBusinessContainedApps</span><span class="sxs-lookup"><span data-stu-id="e33a8-103">List microsoftStoreForBusinessContainedApps</span></span>

> <span data-ttu-id="e33a8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e33a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e33a8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e33a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e33a8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e33a8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e33a8-107">Listeneigenschaften und Beziehungen der [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="e33a8-107">List properties and relationships of the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e33a8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e33a8-108">Prerequisites</span></span>
<span data-ttu-id="e33a8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e33a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e33a8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e33a8-111">Permission type</span></span>|<span data-ttu-id="e33a8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e33a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e33a8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e33a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e33a8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e33a8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e33a8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e33a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e33a8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e33a8-116">Not supported.</span></span>|
|<span data-ttu-id="e33a8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e33a8-117">Application</span></span>|<span data-ttu-id="e33a8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e33a8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e33a8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e33a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="e33a8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e33a8-120">Request headers</span></span>
|<span data-ttu-id="e33a8-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e33a8-121">Header</span></span>|<span data-ttu-id="e33a8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e33a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e33a8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e33a8-123">Authorization</span></span>|<span data-ttu-id="e33a8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e33a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e33a8-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e33a8-125">Accept</span></span>|<span data-ttu-id="e33a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e33a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e33a8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e33a8-127">Request body</span></span>
<span data-ttu-id="e33a8-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e33a8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e33a8-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e33a8-129">Response</span></span>
<span data-ttu-id="e33a8-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e33a8-130">If successful, this method returns a `200 OK` response code and a collection of [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e33a8-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e33a8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e33a8-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e33a8-132">Request</span></span>
<span data-ttu-id="e33a8-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e33a8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
```

### <a name="response"></a><span data-ttu-id="e33a8-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e33a8-134">Response</span></span>
<span data-ttu-id="e33a8-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e33a8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
      "id": "bf1d79df-79df-bf1d-df79-1dbfdf791dbf",
      "appUserModelId": "App User Model Id value"
    }
  ]
}
```





