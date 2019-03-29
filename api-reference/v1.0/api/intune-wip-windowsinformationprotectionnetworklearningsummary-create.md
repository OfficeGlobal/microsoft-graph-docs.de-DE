---
title: windowsInformationProtectionNetworkLearningSummary erstellen
description: Erstellen eines neuen windowsInformationProtectionNetworkLearningSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02a38617e2c47bd023ee4044126d0f4cf5308a8a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959950"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="3989d-103">windowsInformationProtectionNetworkLearningSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="3989d-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="3989d-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3989d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3989d-105">Erstellen eines neuen [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3989d-105">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3989d-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3989d-106">Prerequisites</span></span>
<span data-ttu-id="3989d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3989d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3989d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3989d-109">Permission type</span></span>|<span data-ttu-id="3989d-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3989d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3989d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3989d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3989d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3989d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3989d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3989d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3989d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3989d-114">Not supported.</span></span>|
|<span data-ttu-id="3989d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3989d-115">Application</span></span>|<span data-ttu-id="3989d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3989d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3989d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3989d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="3989d-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3989d-118">Request headers</span></span>
|<span data-ttu-id="3989d-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3989d-119">Header</span></span>|<span data-ttu-id="3989d-120">Wert</span><span class="sxs-lookup"><span data-stu-id="3989d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3989d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3989d-121">Authorization</span></span>|<span data-ttu-id="3989d-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3989d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3989d-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3989d-123">Accept</span></span>|<span data-ttu-id="3989d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3989d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3989d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3989d-125">Request body</span></span>
<span data-ttu-id="3989d-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsInformationProtectionNetworkLearningSummary-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="3989d-126">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="3989d-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionNetworkLearningSummary erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="3989d-127">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="3989d-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3989d-128">Property</span></span>|<span data-ttu-id="3989d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="3989d-129">Type</span></span>|<span data-ttu-id="3989d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3989d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3989d-131">id</span><span class="sxs-lookup"><span data-stu-id="3989d-131">id</span></span>|<span data-ttu-id="3989d-132">String</span><span class="sxs-lookup"><span data-stu-id="3989d-132">String</span></span>|<span data-ttu-id="3989d-133">Eindeutiger Bezeichner für die WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="3989d-133">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="3989d-134">url</span><span class="sxs-lookup"><span data-stu-id="3989d-134">url</span></span>|<span data-ttu-id="3989d-135">String</span><span class="sxs-lookup"><span data-stu-id="3989d-135">String</span></span>|<span data-ttu-id="3989d-136">Website-URL</span><span class="sxs-lookup"><span data-stu-id="3989d-136">Website url</span></span>|
|<span data-ttu-id="3989d-137">deviceCount</span><span class="sxs-lookup"><span data-stu-id="3989d-137">deviceCount</span></span>|<span data-ttu-id="3989d-138">Int32</span><span class="sxs-lookup"><span data-stu-id="3989d-138">Int32</span></span>|<span data-ttu-id="3989d-139">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="3989d-139">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="3989d-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="3989d-140">Response</span></span>
<span data-ttu-id="3989d-141">Wenn erfolgreich, gibt diese Methode den `201 Created`-Antwortcode und das [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3989d-141">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3989d-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3989d-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="3989d-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3989d-143">Request</span></span>
<span data-ttu-id="3989d-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3989d-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3989d-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="3989d-145">Response</span></span>
<span data-ttu-id="3989d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3989d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



