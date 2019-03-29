---
title: Auflisten von „mobileAppContent“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs mobileAppContent auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7d8f864b17f2d89e40108fb29c29733996d8636b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962442"
---
# <a name="list-mobileappcontents"></a><span data-ttu-id="fcca6-103">Auflisten von „mobileAppContent“</span><span class="sxs-lookup"><span data-stu-id="fcca6-103">List mobileAppContents</span></span>

> <span data-ttu-id="fcca6-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fcca6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcca6-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md) auf.</span><span class="sxs-lookup"><span data-stu-id="fcca6-105">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fcca6-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fcca6-106">Prerequisites</span></span>
<span data-ttu-id="fcca6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcca6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcca6-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fcca6-109">Permission type</span></span>|<span data-ttu-id="fcca6-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fcca6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcca6-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fcca6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fcca6-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcca6-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fcca6-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fcca6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcca6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fcca6-114">Not supported.</span></span>|
|<span data-ttu-id="fcca6-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fcca6-115">Application</span></span>|<span data-ttu-id="fcca6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fcca6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcca6-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fcca6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="fcca6-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fcca6-118">Request headers</span></span>
|<span data-ttu-id="fcca6-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fcca6-119">Header</span></span>|<span data-ttu-id="fcca6-120">Wert</span><span class="sxs-lookup"><span data-stu-id="fcca6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcca6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcca6-121">Authorization</span></span>|<span data-ttu-id="fcca6-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fcca6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcca6-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fcca6-123">Accept</span></span>|<span data-ttu-id="fcca6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fcca6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcca6-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fcca6-125">Request body</span></span>
<span data-ttu-id="fcca6-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fcca6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcca6-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="fcca6-127">Response</span></span>
<span data-ttu-id="fcca6-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fcca6-128">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcca6-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fcca6-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="fcca6-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fcca6-130">Request</span></span>
<span data-ttu-id="fcca6-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fcca6-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
```

### <a name="response"></a><span data-ttu-id="fcca6-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="fcca6-132">Response</span></span>
<span data-ttu-id="fcca6-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fcca6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 148

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppContent",
      "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
    }
  ]
}
```



