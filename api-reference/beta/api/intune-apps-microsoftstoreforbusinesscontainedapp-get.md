---
title: Abrufen von microsoftStoreForBusinessContainedApp
description: Lesen Sie Eigenschaften und Beziehungen des MicrosoftStoreForBusinessContainedApp-Objekts.
ms.openlocfilehash: 2ff2b4b4398d4fdf70b9569f2ee13a49da895528
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059964"
---
# <a name="get-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="b4c72-103">Abrufen von microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="b4c72-103">Get microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="b4c72-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b4c72-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4c72-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b4c72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4c72-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b4c72-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4c72-107">Lesen Sie Eigenschaften und Beziehungen des [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b4c72-107">Read properties and relationships of the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4c72-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b4c72-108">Prerequisites</span></span>
<span data-ttu-id="b4c72-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4c72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4c72-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b4c72-111">Permission type</span></span>|<span data-ttu-id="b4c72-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b4c72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4c72-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b4c72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4c72-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4c72-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b4c72-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b4c72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4c72-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4c72-116">Not supported.</span></span>|
|<span data-ttu-id="b4c72-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4c72-117">Application</span></span>|<span data-ttu-id="b4c72-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4c72-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4c72-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4c72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b4c72-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b4c72-120">Optional query parameters</span></span>
<span data-ttu-id="b4c72-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b4c72-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b4c72-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b4c72-122">Request headers</span></span>
|<span data-ttu-id="b4c72-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b4c72-123">Header</span></span>|<span data-ttu-id="b4c72-124">Wert</span><span class="sxs-lookup"><span data-stu-id="b4c72-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4c72-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4c72-125">Authorization</span></span>|<span data-ttu-id="b4c72-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b4c72-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4c72-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b4c72-127">Accept</span></span>|<span data-ttu-id="b4c72-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b4c72-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4c72-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b4c72-129">Request body</span></span>
<span data-ttu-id="b4c72-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b4c72-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4c72-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4c72-131">Response</span></span>
<span data-ttu-id="b4c72-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b4c72-132">If successful, this method returns a `200 OK` response code and [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4c72-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b4c72-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4c72-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4c72-134">Request</span></span>
<span data-ttu-id="b4c72-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b4c72-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
```

### <a name="response"></a><span data-ttu-id="b4c72-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4c72-136">Response</span></span>
<span data-ttu-id="b4c72-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4c72-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 201

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
    "id": "bf1d79df-79df-bf1d-df79-1dbfdf791dbf",
    "appUserModelId": "App User Model Id value"
  }
}
```





