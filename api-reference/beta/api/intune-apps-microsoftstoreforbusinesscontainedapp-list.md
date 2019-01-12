---
title: Liste microsoftStoreForBusinessContainedApps
description: Listeneigenschaften und Beziehungen der MicrosoftStoreForBusinessContainedApp-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7f3dda5817460a6245302f729d7475cb514c2152
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984073"
---
# <a name="list-microsoftstoreforbusinesscontainedapps"></a><span data-ttu-id="31d0d-103">Liste microsoftStoreForBusinessContainedApps</span><span class="sxs-lookup"><span data-stu-id="31d0d-103">List microsoftStoreForBusinessContainedApps</span></span>

> <span data-ttu-id="31d0d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="31d0d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31d0d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="31d0d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31d0d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="31d0d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31d0d-107">Listeneigenschaften und Beziehungen der [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="31d0d-107">List properties and relationships of the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="31d0d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="31d0d-108">Prerequisites</span></span>
<span data-ttu-id="31d0d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31d0d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31d0d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="31d0d-111">Permission type</span></span>|<span data-ttu-id="31d0d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="31d0d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31d0d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="31d0d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31d0d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="31d0d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="31d0d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="31d0d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31d0d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31d0d-116">Not supported.</span></span>|
|<span data-ttu-id="31d0d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="31d0d-117">Application</span></span>|<span data-ttu-id="31d0d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31d0d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31d0d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="31d0d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="31d0d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="31d0d-120">Request headers</span></span>
|<span data-ttu-id="31d0d-121">Header</span><span class="sxs-lookup"><span data-stu-id="31d0d-121">Header</span></span>|<span data-ttu-id="31d0d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="31d0d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31d0d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="31d0d-123">Authorization</span></span>|<span data-ttu-id="31d0d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="31d0d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31d0d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="31d0d-125">Accept</span></span>|<span data-ttu-id="31d0d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31d0d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31d0d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="31d0d-127">Request body</span></span>
<span data-ttu-id="31d0d-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="31d0d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31d0d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="31d0d-129">Response</span></span>
<span data-ttu-id="31d0d-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="31d0d-130">If successful, this method returns a `200 OK` response code and a collection of [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31d0d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="31d0d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="31d0d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="31d0d-132">Request</span></span>
<span data-ttu-id="31d0d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="31d0d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
```

### <a name="response"></a><span data-ttu-id="31d0d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="31d0d-134">Response</span></span>
<span data-ttu-id="31d0d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="31d0d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





