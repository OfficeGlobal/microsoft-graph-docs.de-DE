---
title: windowsInformationProtectionNetworkLearningSummary aktualisieren
description: Aktualisieren der Eigenschaften eines windowsInformationProtectionNetworkLearningSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3d1268d077c9bfc32e5d85b85b103bc7a3e71f78
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947106"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="51fb8-103">windowsInformationProtectionNetworkLearningSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="51fb8-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="51fb8-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="51fb8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51fb8-105">Aktualisieren der Eigenschaften eines [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="51fb8-105">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51fb8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="51fb8-106">Prerequisites</span></span>
<span data-ttu-id="51fb8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51fb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51fb8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="51fb8-109">Permission type</span></span>|<span data-ttu-id="51fb8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="51fb8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51fb8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="51fb8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51fb8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51fb8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="51fb8-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="51fb8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51fb8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51fb8-114">Not supported.</span></span>|
|<span data-ttu-id="51fb8-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="51fb8-115">Application</span></span>|<span data-ttu-id="51fb8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51fb8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51fb8-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="51fb8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="51fb8-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="51fb8-118">Request headers</span></span>
|<span data-ttu-id="51fb8-119">Header</span><span class="sxs-lookup"><span data-stu-id="51fb8-119">Header</span></span>|<span data-ttu-id="51fb8-120">Wert</span><span class="sxs-lookup"><span data-stu-id="51fb8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51fb8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="51fb8-121">Authorization</span></span>|<span data-ttu-id="51fb8-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="51fb8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51fb8-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="51fb8-123">Accept</span></span>|<span data-ttu-id="51fb8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="51fb8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51fb8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="51fb8-125">Request body</span></span>
<span data-ttu-id="51fb8-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="51fb8-126">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="51fb8-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="51fb8-127">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="51fb8-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="51fb8-128">Property</span></span>|<span data-ttu-id="51fb8-129">Typ</span><span class="sxs-lookup"><span data-stu-id="51fb8-129">Type</span></span>|<span data-ttu-id="51fb8-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51fb8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51fb8-131">id</span><span class="sxs-lookup"><span data-stu-id="51fb8-131">id</span></span>|<span data-ttu-id="51fb8-132">String</span><span class="sxs-lookup"><span data-stu-id="51fb8-132">String</span></span>|<span data-ttu-id="51fb8-133">Eindeutiger Bezeichner für die WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="51fb8-133">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="51fb8-134">url</span><span class="sxs-lookup"><span data-stu-id="51fb8-134">url</span></span>|<span data-ttu-id="51fb8-135">String</span><span class="sxs-lookup"><span data-stu-id="51fb8-135">String</span></span>|<span data-ttu-id="51fb8-136">Website-URL</span><span class="sxs-lookup"><span data-stu-id="51fb8-136">Website url</span></span>|
|<span data-ttu-id="51fb8-137">deviceCount</span><span class="sxs-lookup"><span data-stu-id="51fb8-137">deviceCount</span></span>|<span data-ttu-id="51fb8-138">Int32</span><span class="sxs-lookup"><span data-stu-id="51fb8-138">Int32</span></span>|<span data-ttu-id="51fb8-139">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="51fb8-139">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="51fb8-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="51fb8-140">Response</span></span>
<span data-ttu-id="51fb8-141">Wenn erfolgreich, gibt diese Methode den `200 OK`-Antwortcode und das aktualisierte [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="51fb8-141">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51fb8-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="51fb8-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="51fb8-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="51fb8-143">Request</span></span>
<span data-ttu-id="51fb8-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="51fb8-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="51fb8-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="51fb8-145">Response</span></span>
<span data-ttu-id="51fb8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="51fb8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```



