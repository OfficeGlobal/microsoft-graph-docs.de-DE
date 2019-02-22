---
title: Aktualisieren von „reportRoot“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs reportRoot.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2bdb7aeb33fe932d5e6081930a805193e7177758
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156126"
---
# <a name="update-reportroot"></a><span data-ttu-id="edc39-103">Aktualisieren von „reportRoot“</span><span class="sxs-lookup"><span data-stu-id="edc39-103">Update reportRoot</span></span>

> <span data-ttu-id="edc39-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="edc39-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="edc39-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="edc39-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="edc39-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="edc39-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edc39-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="edc39-107">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="edc39-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="edc39-108">Prerequisites</span></span>
<span data-ttu-id="edc39-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edc39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="edc39-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="edc39-111">Permission type</span></span>|<span data-ttu-id="edc39-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="edc39-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edc39-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="edc39-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="edc39-114">&nbsp; &nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="edc39-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="edc39-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edc39-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="edc39-116">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="edc39-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="edc39-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edc39-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="edc39-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="edc39-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edc39-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="edc39-119">Not supported.</span></span>|
|<span data-ttu-id="edc39-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="edc39-120">Application</span></span>|<span data-ttu-id="edc39-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="edc39-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="edc39-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="edc39-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="edc39-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="edc39-123">Request headers</span></span>
|<span data-ttu-id="edc39-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="edc39-124">Header</span></span>|<span data-ttu-id="edc39-125">Wert</span><span class="sxs-lookup"><span data-stu-id="edc39-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edc39-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="edc39-126">Authorization</span></span>|<span data-ttu-id="edc39-127">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="edc39-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edc39-128">Annehmen</span><span class="sxs-lookup"><span data-stu-id="edc39-128">Accept</span></span>|<span data-ttu-id="edc39-129">application/json</span><span class="sxs-lookup"><span data-stu-id="edc39-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edc39-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="edc39-130">Request body</span></span>
<span data-ttu-id="edc39-131">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [reportRoot](../resources/intune-shared-reportroot.md) an.</span><span class="sxs-lookup"><span data-stu-id="edc39-131">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="edc39-132">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [reportRoot](../resources/intune-shared-reportroot.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="edc39-132">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="edc39-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="edc39-133">Property</span></span>|<span data-ttu-id="edc39-134">Typ</span><span class="sxs-lookup"><span data-stu-id="edc39-134">Type</span></span>|<span data-ttu-id="edc39-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="edc39-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edc39-136">id</span><span class="sxs-lookup"><span data-stu-id="edc39-136">id</span></span>|<span data-ttu-id="edc39-137">String</span><span class="sxs-lookup"><span data-stu-id="edc39-137">String</span></span>|<span data-ttu-id="edc39-138">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="edc39-138">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="edc39-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="edc39-139">Response</span></span>
<span data-ttu-id="edc39-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [reportRoot](../resources/intune-shared-reportroot.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="edc39-140">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edc39-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="edc39-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="edc39-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="edc39-142">Request</span></span>
<span data-ttu-id="edc39-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="edc39-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="edc39-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="edc39-144">Response</span></span>
<span data-ttu-id="edc39-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="edc39-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```



