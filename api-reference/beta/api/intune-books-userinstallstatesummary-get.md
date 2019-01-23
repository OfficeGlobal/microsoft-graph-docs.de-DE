---
title: Abrufen von „userInstallStateSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs userInstallStateSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 91ee89e3d23f81fb3def1291f070bc31c5e85c8f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413878"
---
# <a name="get-userinstallstatesummary"></a><span data-ttu-id="d3b56-103">Abrufen von „userInstallStateSummary“</span><span class="sxs-lookup"><span data-stu-id="d3b56-103">Get userInstallStateSummary</span></span>

> <span data-ttu-id="d3b56-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="d3b56-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d3b56-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d3b56-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3b56-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d3b56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3b56-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d3b56-107">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3b56-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d3b56-108">Prerequisites</span></span>
<span data-ttu-id="d3b56-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d3b56-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d3b56-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d3b56-111">Permission type</span></span>|<span data-ttu-id="d3b56-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d3b56-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3b56-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d3b56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3b56-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3b56-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d3b56-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d3b56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3b56-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3b56-116">Not supported.</span></span>|
|<span data-ttu-id="d3b56-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d3b56-117">Application</span></span>|<span data-ttu-id="d3b56-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3b56-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3b56-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3b56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d3b56-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d3b56-120">Optional query parameters</span></span>
<span data-ttu-id="d3b56-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d3b56-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3b56-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d3b56-122">Request headers</span></span>
|<span data-ttu-id="d3b56-123">Header</span><span class="sxs-lookup"><span data-stu-id="d3b56-123">Header</span></span>|<span data-ttu-id="d3b56-124">Wert</span><span class="sxs-lookup"><span data-stu-id="d3b56-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3b56-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d3b56-125">Authorization</span></span>|<span data-ttu-id="d3b56-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d3b56-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3b56-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d3b56-127">Accept</span></span>|<span data-ttu-id="d3b56-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d3b56-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3b56-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d3b56-129">Request body</span></span>
<span data-ttu-id="d3b56-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d3b56-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3b56-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3b56-131">Response</span></span>
<span data-ttu-id="d3b56-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d3b56-132">If successful, this method returns a `200 OK` response code and [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3b56-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d3b56-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3b56-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3b56-134">Request</span></span>
<span data-ttu-id="d3b56-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d3b56-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="d3b56-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3b56-136">Response</span></span>
<span data-ttu-id="d3b56-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d3b56-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "value": {
    "@odata.type": "#microsoft.graph.userInstallStateSummary",
    "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
    "userName": "User Name value",
    "installedDeviceCount": 4,
    "failedDeviceCount": 1,
    "notInstalledDeviceCount": 7
  }
}
```




