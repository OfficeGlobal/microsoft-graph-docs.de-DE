---
title: windowsInformationProtectionNetworkLearningSummary aktualisieren
description: Aktualisieren der Eigenschaften eines windowsInformationProtectionNetworkLearningSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 74df8f54ddec226372df1a4a49b7746f95b2c023
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876916"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="9b9cf-103">windowsInformationProtectionNetworkLearningSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9b9cf-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="9b9cf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9b9cf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b9cf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9b9cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b9cf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9b9cf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b9cf-107">Aktualisieren der Eigenschaften eines [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9b9cf-107">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b9cf-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9b9cf-108">Prerequisites</span></span>
<span data-ttu-id="9b9cf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b9cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b9cf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9b9cf-111">Permission type</span></span>|<span data-ttu-id="9b9cf-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9b9cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b9cf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9b9cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b9cf-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b9cf-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9b9cf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9b9cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b9cf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9b9cf-116">Not supported.</span></span>|
|<span data-ttu-id="9b9cf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9b9cf-117">Application</span></span>|<span data-ttu-id="9b9cf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9b9cf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b9cf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b9cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="9b9cf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9b9cf-120">Request headers</span></span>
|<span data-ttu-id="9b9cf-121">Header</span><span class="sxs-lookup"><span data-stu-id="9b9cf-121">Header</span></span>|<span data-ttu-id="9b9cf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9b9cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b9cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b9cf-123">Authorization</span></span>|<span data-ttu-id="9b9cf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9b9cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b9cf-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9b9cf-125">Accept</span></span>|<span data-ttu-id="9b9cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b9cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b9cf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9b9cf-127">Request body</span></span>
<span data-ttu-id="9b9cf-128">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="9b9cf-128">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="9b9cf-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="9b9cf-129">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="9b9cf-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9b9cf-130">Property</span></span>|<span data-ttu-id="9b9cf-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9b9cf-131">Type</span></span>|<span data-ttu-id="9b9cf-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9b9cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b9cf-133">id</span><span class="sxs-lookup"><span data-stu-id="9b9cf-133">id</span></span>|<span data-ttu-id="9b9cf-134">String</span><span class="sxs-lookup"><span data-stu-id="9b9cf-134">String</span></span>|<span data-ttu-id="9b9cf-135">Eindeutiger Bezeichner für die WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="9b9cf-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="9b9cf-136">url</span><span class="sxs-lookup"><span data-stu-id="9b9cf-136">url</span></span>|<span data-ttu-id="9b9cf-137">String</span><span class="sxs-lookup"><span data-stu-id="9b9cf-137">String</span></span>|<span data-ttu-id="9b9cf-138">Website-URL</span><span class="sxs-lookup"><span data-stu-id="9b9cf-138">Website url</span></span>|
|<span data-ttu-id="9b9cf-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="9b9cf-139">deviceCount</span></span>|<span data-ttu-id="9b9cf-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9b9cf-140">Int32</span></span>|<span data-ttu-id="9b9cf-141">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="9b9cf-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="9b9cf-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b9cf-142">Response</span></span>
<span data-ttu-id="9b9cf-143">Wenn erfolgreich, gibt diese Methode den `200 OK`-Antwortcode und das aktualisierte [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9b9cf-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b9cf-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9b9cf-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="9b9cf-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b9cf-145">Request</span></span>
<span data-ttu-id="9b9cf-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9b9cf-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 48

{
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="9b9cf-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b9cf-147">Response</span></span>
<span data-ttu-id="9b9cf-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9b9cf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





