---
title: Aktualisieren von „reportRoot“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs reportRoot.
author: tfitzmac
ms.openlocfilehash: 4f3d0e297a9b7d122e9b21afd7555c1af307d2d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349532"
---
# <a name="update-reportroot"></a><span data-ttu-id="9cbc9-103">Aktualisieren von „reportRoot“</span><span class="sxs-lookup"><span data-stu-id="9cbc9-103">Update reportRoot</span></span>

> <span data-ttu-id="9cbc9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9cbc9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9cbc9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9cbc9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9cbc9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9cbc9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9cbc9-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="9cbc9-107">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9cbc9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9cbc9-108">Prerequisites</span></span>
<span data-ttu-id="9cbc9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cbc9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cbc9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9cbc9-111">Permission type</span></span>|<span data-ttu-id="9cbc9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9cbc9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cbc9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9cbc9-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9cbc9-114">&nbsp;&nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="9cbc9-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="9cbc9-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cbc9-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="9cbc9-116">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="9cbc9-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="9cbc9-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cbc9-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9cbc9-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9cbc9-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cbc9-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9cbc9-119">Not supported.</span></span>|
|<span data-ttu-id="9cbc9-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9cbc9-120">Application</span></span>|<span data-ttu-id="9cbc9-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9cbc9-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cbc9-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9cbc9-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="9cbc9-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9cbc9-123">Request headers</span></span>
|<span data-ttu-id="9cbc9-124">Header</span><span class="sxs-lookup"><span data-stu-id="9cbc9-124">Header</span></span>|<span data-ttu-id="9cbc9-125">Wert</span><span class="sxs-lookup"><span data-stu-id="9cbc9-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cbc9-126">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9cbc9-126">Authorization</span></span>|<span data-ttu-id="9cbc9-127">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9cbc9-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cbc9-128">Accept</span><span class="sxs-lookup"><span data-stu-id="9cbc9-128">Accept</span></span>|<span data-ttu-id="9cbc9-129">application/json</span><span class="sxs-lookup"><span data-stu-id="9cbc9-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cbc9-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9cbc9-130">Request body</span></span>
<span data-ttu-id="9cbc9-131">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [reportRoot](../resources/intune-shared-reportroot.md) an.</span><span class="sxs-lookup"><span data-stu-id="9cbc9-131">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="9cbc9-132">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [reportRoot](../resources/intune-shared-reportroot.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="9cbc9-132">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="9cbc9-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9cbc9-133">Property</span></span>|<span data-ttu-id="9cbc9-134">Typ</span><span class="sxs-lookup"><span data-stu-id="9cbc9-134">Type</span></span>|<span data-ttu-id="9cbc9-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9cbc9-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cbc9-136">id</span><span class="sxs-lookup"><span data-stu-id="9cbc9-136">id</span></span>|<span data-ttu-id="9cbc9-137">String</span><span class="sxs-lookup"><span data-stu-id="9cbc9-137">String</span></span>|<span data-ttu-id="9cbc9-138">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="9cbc9-138">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="9cbc9-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="9cbc9-139">Response</span></span>
<span data-ttu-id="9cbc9-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [reportRoot](../resources/intune-shared-reportroot.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9cbc9-140">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cbc9-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9cbc9-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="9cbc9-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9cbc9-142">Request</span></span>
<span data-ttu-id="9cbc9-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9cbc9-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="9cbc9-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="9cbc9-144">Response</span></span>
<span data-ttu-id="9cbc9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9cbc9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```



