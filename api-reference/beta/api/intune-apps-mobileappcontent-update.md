---
title: Aktualisieren von „mobileAppContent“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs mobileAppContent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b792deab5c10e8770666a707976afa330d03a4f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149371"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="34ad1-103">Aktualisieren von „mobileAppContent“</span><span class="sxs-lookup"><span data-stu-id="34ad1-103">Update mobileAppContent</span></span>

> <span data-ttu-id="34ad1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34ad1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34ad1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="34ad1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34ad1-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="34ad1-106">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34ad1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="34ad1-107">Prerequisites</span></span>
<span data-ttu-id="34ad1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="34ad1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="34ad1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="34ad1-110">Permission type</span></span>|<span data-ttu-id="34ad1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="34ad1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34ad1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="34ad1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34ad1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34ad1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="34ad1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="34ad1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34ad1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="34ad1-115">Not supported.</span></span>|
|<span data-ttu-id="34ad1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="34ad1-116">Application</span></span>|<span data-ttu-id="34ad1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="34ad1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34ad1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="34ad1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="34ad1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="34ad1-119">Request headers</span></span>
|<span data-ttu-id="34ad1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="34ad1-120">Header</span></span>|<span data-ttu-id="34ad1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="34ad1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34ad1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="34ad1-122">Authorization</span></span>|<span data-ttu-id="34ad1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="34ad1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34ad1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="34ad1-124">Accept</span></span>|<span data-ttu-id="34ad1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34ad1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34ad1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="34ad1-126">Request body</span></span>
<span data-ttu-id="34ad1-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md) an.</span><span class="sxs-lookup"><span data-stu-id="34ad1-127">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="34ad1-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="34ad1-128">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="34ad1-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="34ad1-129">Property</span></span>|<span data-ttu-id="34ad1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="34ad1-130">Type</span></span>|<span data-ttu-id="34ad1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34ad1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34ad1-132">id</span><span class="sxs-lookup"><span data-stu-id="34ad1-132">id</span></span>|<span data-ttu-id="34ad1-133">String</span><span class="sxs-lookup"><span data-stu-id="34ad1-133">String</span></span>|<span data-ttu-id="34ad1-134">Die Version der App-Inhalte</span><span class="sxs-lookup"><span data-stu-id="34ad1-134">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="34ad1-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="34ad1-135">Response</span></span>
<span data-ttu-id="34ad1-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="34ad1-136">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34ad1-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="34ad1-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="34ad1-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="34ad1-138">Request</span></span>
<span data-ttu-id="34ad1-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="34ad1-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="34ad1-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="34ad1-140">Response</span></span>
<span data-ttu-id="34ad1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="34ad1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```




