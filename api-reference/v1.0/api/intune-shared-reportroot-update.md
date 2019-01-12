---
title: Aktualisieren von „reportRoot“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs reportRoot.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a902d341761cf56ced39a8309479ca27611ec5ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934555"
---
# <a name="update-reportroot"></a><span data-ttu-id="47edd-103">Aktualisieren von „reportRoot“</span><span class="sxs-lookup"><span data-stu-id="47edd-103">Update reportRoot</span></span>

> <span data-ttu-id="47edd-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="47edd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47edd-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="47edd-105">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="47edd-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="47edd-106">Prerequisites</span></span>
<span data-ttu-id="47edd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47edd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47edd-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="47edd-109">Permission type</span></span>|<span data-ttu-id="47edd-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="47edd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47edd-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="47edd-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="47edd-112">&nbsp;&nbsp; Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="47edd-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="47edd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47edd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="47edd-114">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="47edd-114">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="47edd-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47edd-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="47edd-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="47edd-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47edd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47edd-117">Not supported.</span></span>|
|<span data-ttu-id="47edd-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="47edd-118">Application</span></span>|<span data-ttu-id="47edd-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47edd-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47edd-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="47edd-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="47edd-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="47edd-121">Request headers</span></span>
|<span data-ttu-id="47edd-122">Header</span><span class="sxs-lookup"><span data-stu-id="47edd-122">Header</span></span>|<span data-ttu-id="47edd-123">Wert</span><span class="sxs-lookup"><span data-stu-id="47edd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47edd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="47edd-124">Authorization</span></span>|<span data-ttu-id="47edd-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="47edd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47edd-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="47edd-126">Accept</span></span>|<span data-ttu-id="47edd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="47edd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47edd-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="47edd-128">Request body</span></span>
<span data-ttu-id="47edd-129">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [reportRoot](../resources/intune-shared-reportroot.md) an.</span><span class="sxs-lookup"><span data-stu-id="47edd-129">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="47edd-130">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [reportRoot](../resources/intune-shared-reportroot.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="47edd-130">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="47edd-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="47edd-131">Property</span></span>|<span data-ttu-id="47edd-132">Typ</span><span class="sxs-lookup"><span data-stu-id="47edd-132">Type</span></span>|<span data-ttu-id="47edd-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="47edd-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47edd-134">id</span><span class="sxs-lookup"><span data-stu-id="47edd-134">id</span></span>|<span data-ttu-id="47edd-135">String</span><span class="sxs-lookup"><span data-stu-id="47edd-135">String</span></span>|<span data-ttu-id="47edd-136">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="47edd-136">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="47edd-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="47edd-137">Response</span></span>
<span data-ttu-id="47edd-138">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [reportRoot](../resources/intune-shared-reportroot.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="47edd-138">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47edd-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="47edd-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="47edd-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="47edd-140">Request</span></span>
<span data-ttu-id="47edd-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="47edd-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="47edd-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="47edd-142">Response</span></span>
<span data-ttu-id="47edd-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="47edd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```








