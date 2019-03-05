---
title: windowsInformationProtectionNetworkLearningSummary erstellen
description: Erstellen eines neuen windowsInformationProtectionNetworkLearningSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dc9ffe06e2438510a5301caa09dca2f20c27c293
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257799"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="6c2b4-103">windowsInformationProtectionNetworkLearningSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="6c2b4-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="6c2b4-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6c2b4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c2b4-105">Erstellen eines neuen [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6c2b4-105">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c2b4-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6c2b4-106">Prerequisites</span></span>
<span data-ttu-id="6c2b4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6c2b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6c2b4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6c2b4-109">Permission type</span></span>|<span data-ttu-id="6c2b4-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6c2b4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c2b4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6c2b4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6c2b4-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c2b4-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6c2b4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6c2b4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c2b4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6c2b4-114">Not supported.</span></span>|
|<span data-ttu-id="6c2b4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6c2b4-115">Application</span></span>|<span data-ttu-id="6c2b4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6c2b4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c2b4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c2b4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="6c2b4-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6c2b4-118">Request headers</span></span>
|<span data-ttu-id="6c2b4-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6c2b4-119">Header</span></span>|<span data-ttu-id="6c2b4-120">Wert</span><span class="sxs-lookup"><span data-stu-id="6c2b4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c2b4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c2b4-121">Authorization</span></span>|<span data-ttu-id="6c2b4-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6c2b4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c2b4-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6c2b4-123">Accept</span></span>|<span data-ttu-id="6c2b4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6c2b4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c2b4-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6c2b4-125">Request body</span></span>
<span data-ttu-id="6c2b4-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsInformationProtectionNetworkLearningSummary-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="6c2b4-126">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="6c2b4-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionNetworkLearningSummary erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="6c2b4-127">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="6c2b4-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6c2b4-128">Property</span></span>|<span data-ttu-id="6c2b4-129">Typ</span><span class="sxs-lookup"><span data-stu-id="6c2b4-129">Type</span></span>|<span data-ttu-id="6c2b4-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6c2b4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c2b4-131">id</span><span class="sxs-lookup"><span data-stu-id="6c2b4-131">id</span></span>|<span data-ttu-id="6c2b4-132">String</span><span class="sxs-lookup"><span data-stu-id="6c2b4-132">String</span></span>|<span data-ttu-id="6c2b4-133">Eindeutiger Bezeichner für die WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="6c2b4-133">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="6c2b4-134">url</span><span class="sxs-lookup"><span data-stu-id="6c2b4-134">url</span></span>|<span data-ttu-id="6c2b4-135">String</span><span class="sxs-lookup"><span data-stu-id="6c2b4-135">String</span></span>|<span data-ttu-id="6c2b4-136">Website-URL</span><span class="sxs-lookup"><span data-stu-id="6c2b4-136">Website url</span></span>|
|<span data-ttu-id="6c2b4-137">deviceCount</span><span class="sxs-lookup"><span data-stu-id="6c2b4-137">deviceCount</span></span>|<span data-ttu-id="6c2b4-138">Int32</span><span class="sxs-lookup"><span data-stu-id="6c2b4-138">Int32</span></span>|<span data-ttu-id="6c2b4-139">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="6c2b4-139">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="6c2b4-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c2b4-140">Response</span></span>
<span data-ttu-id="6c2b4-141">Wenn erfolgreich, gibt diese Methode den `201 Created`-Antwortcode und das [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6c2b4-141">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c2b4-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6c2b4-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c2b4-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c2b4-143">Request</span></span>
<span data-ttu-id="6c2b4-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6c2b4-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="6c2b4-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c2b4-145">Response</span></span>
<span data-ttu-id="6c2b4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6c2b4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```



