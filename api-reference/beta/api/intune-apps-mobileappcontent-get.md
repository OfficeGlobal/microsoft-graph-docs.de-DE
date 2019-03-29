---
title: mobileAppContent abrufen
description: Lesen von Eigenschaften und Beziehungen des mobileAppContent-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d68e049e43f69f1009c27bde0983a8d84bdb60f7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980901"
---
# <a name="get-mobileappcontent"></a><span data-ttu-id="a573a-103">mobileAppContent abrufen</span><span class="sxs-lookup"><span data-stu-id="a573a-103">Get mobileAppContent</span></span>

> <span data-ttu-id="a573a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a573a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a573a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a573a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a573a-106">Lesen von Eigenschaften und Beziehungen des [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a573a-106">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a573a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a573a-107">Prerequisites</span></span>
<span data-ttu-id="a573a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a573a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a573a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a573a-110">Permission type</span></span>|<span data-ttu-id="a573a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a573a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a573a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a573a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a573a-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a573a-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a573a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a573a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a573a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a573a-115">Not supported.</span></span>|
|<span data-ttu-id="a573a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a573a-116">Application</span></span>|<span data-ttu-id="a573a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a573a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a573a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a573a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a573a-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a573a-119">Optional query parameters</span></span>
<span data-ttu-id="a573a-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a573a-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a573a-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a573a-121">Request headers</span></span>
|<span data-ttu-id="a573a-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a573a-122">Header</span></span>|<span data-ttu-id="a573a-123">Wert</span><span class="sxs-lookup"><span data-stu-id="a573a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a573a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a573a-124">Authorization</span></span>|<span data-ttu-id="a573a-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a573a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a573a-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a573a-126">Accept</span></span>|<span data-ttu-id="a573a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a573a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a573a-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a573a-128">Request body</span></span>
<span data-ttu-id="a573a-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a573a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a573a-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a573a-130">Response</span></span>
<span data-ttu-id="a573a-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a573a-131">If successful, this method returns a `200 OK` response code and [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a573a-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a573a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a573a-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a573a-133">Request</span></span>
<span data-ttu-id="a573a-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a573a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
```

### <a name="response"></a><span data-ttu-id="a573a-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="a573a-135">Response</span></span>
<span data-ttu-id="a573a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a573a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




