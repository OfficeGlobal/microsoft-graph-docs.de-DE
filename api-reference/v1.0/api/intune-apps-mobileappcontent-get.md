---
title: mobileAppContent abrufen
description: Lesen von Eigenschaften und Beziehungen des mobileAppContent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3dc086b796b0d4a72a11543231582ca62926dfd
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251223"
---
# <a name="get-mobileappcontent"></a><span data-ttu-id="acd78-103">mobileAppContent abrufen</span><span class="sxs-lookup"><span data-stu-id="acd78-103">Get mobileAppContent</span></span>

> <span data-ttu-id="acd78-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="acd78-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acd78-105">Lesen von Eigenschaften und Beziehungen des [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="acd78-105">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="acd78-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="acd78-106">Prerequisites</span></span>
<span data-ttu-id="acd78-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="acd78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="acd78-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="acd78-109">Permission type</span></span>|<span data-ttu-id="acd78-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="acd78-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acd78-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="acd78-111">Delegated (work or school account)</span></span>|<span data-ttu-id="acd78-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="acd78-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="acd78-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="acd78-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acd78-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="acd78-114">Not supported.</span></span>|
|<span data-ttu-id="acd78-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="acd78-115">Application</span></span>|<span data-ttu-id="acd78-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="acd78-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acd78-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="acd78-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="acd78-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="acd78-118">Optional query parameters</span></span>
<span data-ttu-id="acd78-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="acd78-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="acd78-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="acd78-120">Request headers</span></span>
|<span data-ttu-id="acd78-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="acd78-121">Header</span></span>|<span data-ttu-id="acd78-122">Wert</span><span class="sxs-lookup"><span data-stu-id="acd78-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acd78-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="acd78-123">Authorization</span></span>|<span data-ttu-id="acd78-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="acd78-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acd78-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="acd78-125">Accept</span></span>|<span data-ttu-id="acd78-126">application/json</span><span class="sxs-lookup"><span data-stu-id="acd78-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acd78-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="acd78-127">Request body</span></span>
<span data-ttu-id="acd78-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="acd78-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acd78-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="acd78-129">Response</span></span>
<span data-ttu-id="acd78-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="acd78-130">If successful, this method returns a `200 OK` response code and [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acd78-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="acd78-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="acd78-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="acd78-132">Request</span></span>
<span data-ttu-id="acd78-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="acd78-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
```

### <a name="response"></a><span data-ttu-id="acd78-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="acd78-134">Response</span></span>
<span data-ttu-id="acd78-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="acd78-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppContent",
    "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
  }
}
```



