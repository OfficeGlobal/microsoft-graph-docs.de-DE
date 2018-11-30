---
title: windowsInformationProtectionNetworkLearningSummary aktualisieren
description: Aktualisieren der Eigenschaften eines windowsInformationProtectionNetworkLearningSummary-Objekts.
ms.openlocfilehash: ade11aa7dfdbe9f189923ad470d411e19a50fb51
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062881"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="a2afd-103">windowsInformationProtectionNetworkLearningSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a2afd-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="a2afd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a2afd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2afd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a2afd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2afd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a2afd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2afd-107">Aktualisieren der Eigenschaften eines [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a2afd-107">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2afd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a2afd-108">Prerequisites</span></span>
<span data-ttu-id="a2afd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2afd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2afd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a2afd-111">Permission type</span></span>|<span data-ttu-id="a2afd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a2afd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2afd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a2afd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2afd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2afd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a2afd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a2afd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2afd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2afd-116">Not supported.</span></span>|
|<span data-ttu-id="a2afd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a2afd-117">Application</span></span>|<span data-ttu-id="a2afd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2afd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2afd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2afd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="a2afd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a2afd-120">Request headers</span></span>
|<span data-ttu-id="a2afd-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a2afd-121">Header</span></span>|<span data-ttu-id="a2afd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a2afd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2afd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2afd-123">Authorization</span></span>|<span data-ttu-id="a2afd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a2afd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2afd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a2afd-125">Accept</span></span>|<span data-ttu-id="a2afd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2afd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2afd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a2afd-127">Request body</span></span>
<span data-ttu-id="a2afd-128">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekt ein.</span><span class="sxs-lookup"><span data-stu-id="a2afd-128">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="a2afd-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a2afd-129">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="a2afd-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a2afd-130">Property</span></span>|<span data-ttu-id="a2afd-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a2afd-131">Type</span></span>|<span data-ttu-id="a2afd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2afd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2afd-133">id</span><span class="sxs-lookup"><span data-stu-id="a2afd-133">id</span></span>|<span data-ttu-id="a2afd-134">String</span><span class="sxs-lookup"><span data-stu-id="a2afd-134">String</span></span>|<span data-ttu-id="a2afd-135">Eindeutiger Bezeichner für die WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="a2afd-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="a2afd-136">url</span><span class="sxs-lookup"><span data-stu-id="a2afd-136">url</span></span>|<span data-ttu-id="a2afd-137">String</span><span class="sxs-lookup"><span data-stu-id="a2afd-137">String</span></span>|<span data-ttu-id="a2afd-138">Website-URL</span><span class="sxs-lookup"><span data-stu-id="a2afd-138">Website url</span></span>|
|<span data-ttu-id="a2afd-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="a2afd-139">deviceCount</span></span>|<span data-ttu-id="a2afd-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a2afd-140">Int32</span></span>|<span data-ttu-id="a2afd-141">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="a2afd-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="a2afd-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2afd-142">Response</span></span>
<span data-ttu-id="a2afd-143">Wenn erfolgreich, gibt diese Methode den `200 OK`-Antwortcode und das aktualisierte [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a2afd-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2afd-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a2afd-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2afd-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2afd-145">Request</span></span>
<span data-ttu-id="a2afd-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a2afd-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 48

{
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="a2afd-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2afd-147">Response</span></span>
<span data-ttu-id="a2afd-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a2afd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





