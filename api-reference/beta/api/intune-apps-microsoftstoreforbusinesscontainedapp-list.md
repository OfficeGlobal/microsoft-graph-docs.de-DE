---
title: MicrosoftStoreForBusinessContainedApps aufListen
description: AufListen von Eigenschaften und Beziehungen der microsoftStoreForBusinessContainedApp-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37817d818ac1714fe9e2478e02c50786cb548a8a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156343"
---
# <a name="list-microsoftstoreforbusinesscontainedapps"></a><span data-ttu-id="9d613-103">MicrosoftStoreForBusinessContainedApps aufListen</span><span class="sxs-lookup"><span data-stu-id="9d613-103">List microsoftStoreForBusinessContainedApps</span></span>

> <span data-ttu-id="9d613-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9d613-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d613-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9d613-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d613-106">AufListen von Eigenschaften und Beziehungen der [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="9d613-106">List properties and relationships of the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d613-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9d613-107">Prerequisites</span></span>
<span data-ttu-id="9d613-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9d613-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9d613-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9d613-110">Permission type</span></span>|<span data-ttu-id="9d613-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9d613-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d613-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9d613-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9d613-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d613-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9d613-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9d613-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d613-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9d613-115">Not supported.</span></span>|
|<span data-ttu-id="9d613-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9d613-116">Application</span></span>|<span data-ttu-id="9d613-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9d613-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d613-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d613-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="9d613-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9d613-119">Request headers</span></span>
|<span data-ttu-id="9d613-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9d613-120">Header</span></span>|<span data-ttu-id="9d613-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9d613-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d613-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d613-122">Authorization</span></span>|<span data-ttu-id="9d613-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9d613-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d613-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9d613-124">Accept</span></span>|<span data-ttu-id="9d613-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9d613-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d613-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9d613-126">Request body</span></span>
<span data-ttu-id="9d613-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9d613-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d613-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d613-128">Response</span></span>
<span data-ttu-id="9d613-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9d613-129">If successful, this method returns a `200 OK` response code and a collection of [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d613-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9d613-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d613-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d613-131">Request</span></span>
<span data-ttu-id="9d613-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9d613-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
```

### <a name="response"></a><span data-ttu-id="9d613-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d613-133">Response</span></span>
<span data-ttu-id="9d613-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9d613-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




