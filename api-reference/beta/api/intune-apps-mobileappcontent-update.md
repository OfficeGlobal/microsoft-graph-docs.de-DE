---
title: Aktualisieren von „mobileAppContent“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs mobileAppContent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f38e95e3001665010d96f5be0008a82672243b80
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957003"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="03952-103">Aktualisieren von „mobileAppContent“</span><span class="sxs-lookup"><span data-stu-id="03952-103">Update mobileAppContent</span></span>

> <span data-ttu-id="03952-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="03952-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03952-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="03952-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03952-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="03952-106">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03952-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="03952-107">Prerequisites</span></span>
<span data-ttu-id="03952-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03952-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03952-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="03952-110">Permission type</span></span>|<span data-ttu-id="03952-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="03952-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03952-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="03952-112">Delegated (work or school account)</span></span>|<span data-ttu-id="03952-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03952-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="03952-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="03952-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03952-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="03952-115">Not supported.</span></span>|
|<span data-ttu-id="03952-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="03952-116">Application</span></span>|<span data-ttu-id="03952-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="03952-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03952-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="03952-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="03952-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="03952-119">Request headers</span></span>
|<span data-ttu-id="03952-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="03952-120">Header</span></span>|<span data-ttu-id="03952-121">Wert</span><span class="sxs-lookup"><span data-stu-id="03952-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03952-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="03952-122">Authorization</span></span>|<span data-ttu-id="03952-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="03952-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03952-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="03952-124">Accept</span></span>|<span data-ttu-id="03952-125">application/json</span><span class="sxs-lookup"><span data-stu-id="03952-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03952-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="03952-126">Request body</span></span>
<span data-ttu-id="03952-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md) an.</span><span class="sxs-lookup"><span data-stu-id="03952-127">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="03952-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="03952-128">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="03952-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="03952-129">Property</span></span>|<span data-ttu-id="03952-130">Typ</span><span class="sxs-lookup"><span data-stu-id="03952-130">Type</span></span>|<span data-ttu-id="03952-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="03952-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03952-132">id</span><span class="sxs-lookup"><span data-stu-id="03952-132">id</span></span>|<span data-ttu-id="03952-133">String</span><span class="sxs-lookup"><span data-stu-id="03952-133">String</span></span>|<span data-ttu-id="03952-134">Die Version der App-Inhalte</span><span class="sxs-lookup"><span data-stu-id="03952-134">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="03952-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="03952-135">Response</span></span>
<span data-ttu-id="03952-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="03952-136">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03952-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="03952-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="03952-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="03952-138">Request</span></span>
<span data-ttu-id="03952-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="03952-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="03952-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="03952-140">Response</span></span>
<span data-ttu-id="03952-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="03952-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```




