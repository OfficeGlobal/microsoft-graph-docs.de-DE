---
title: Auflisten von „userInstallStateSummary“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs userInstallStateSummary auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a6ffe715dec0ba761f9c5636a7c184c64cf248b6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967069"
---
# <a name="list-userinstallstatesummaries"></a><span data-ttu-id="7a794-103">Auflisten von „userInstallStateSummary“</span><span class="sxs-lookup"><span data-stu-id="7a794-103">List userInstallStateSummaries</span></span>

> <span data-ttu-id="7a794-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7a794-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a794-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) auf.</span><span class="sxs-lookup"><span data-stu-id="7a794-105">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a794-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7a794-106">Prerequisites</span></span>
<span data-ttu-id="7a794-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a794-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a794-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7a794-109">Permission type</span></span>|<span data-ttu-id="7a794-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7a794-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a794-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7a794-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7a794-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a794-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7a794-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7a794-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a794-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a794-114">Not supported.</span></span>|
|<span data-ttu-id="7a794-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7a794-115">Application</span></span>|<span data-ttu-id="7a794-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a794-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a794-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a794-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="7a794-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7a794-118">Request headers</span></span>
|<span data-ttu-id="7a794-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7a794-119">Header</span></span>|<span data-ttu-id="7a794-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7a794-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a794-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a794-121">Authorization</span></span>|<span data-ttu-id="7a794-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7a794-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a794-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7a794-123">Accept</span></span>|<span data-ttu-id="7a794-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7a794-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a794-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7a794-125">Request body</span></span>
<span data-ttu-id="7a794-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7a794-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a794-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a794-127">Response</span></span>
<span data-ttu-id="7a794-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7a794-128">If successful, this method returns a `200 OK` response code and a collection of [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a794-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7a794-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a794-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a794-130">Request</span></span>
<span data-ttu-id="7a794-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7a794-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="7a794-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a794-132">Response</span></span>
<span data-ttu-id="7a794-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a794-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userInstallStateSummary",
      "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
      "userName": "User Name value",
      "installedDeviceCount": 4,
      "failedDeviceCount": 1,
      "notInstalledDeviceCount": 7
    }
  ]
}
```



