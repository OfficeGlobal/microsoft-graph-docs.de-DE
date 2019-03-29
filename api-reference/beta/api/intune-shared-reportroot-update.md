---
title: Aktualisieren von „reportRoot“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs reportRoot.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3127ca7804883c5e29fe91cf5e21bb15240a1314
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972809"
---
# <a name="update-reportroot"></a><span data-ttu-id="1d16c-103">Aktualisieren von „reportRoot“</span><span class="sxs-lookup"><span data-stu-id="1d16c-103">Update reportRoot</span></span>

> <span data-ttu-id="1d16c-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="1d16c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1d16c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1d16c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d16c-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1d16c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d16c-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="1d16c-107">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1d16c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1d16c-108">Prerequisites</span></span>
<span data-ttu-id="1d16c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d16c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d16c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1d16c-111">Permission type</span></span>|<span data-ttu-id="1d16c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1d16c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d16c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1d16c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1d16c-114">&nbsp; &nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="1d16c-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="1d16c-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d16c-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="1d16c-116">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="1d16c-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="1d16c-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d16c-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1d16c-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1d16c-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d16c-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1d16c-119">Not supported.</span></span>|
|<span data-ttu-id="1d16c-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1d16c-120">Application</span></span>|<span data-ttu-id="1d16c-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1d16c-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d16c-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d16c-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="1d16c-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1d16c-123">Request headers</span></span>
|<span data-ttu-id="1d16c-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1d16c-124">Header</span></span>|<span data-ttu-id="1d16c-125">Wert</span><span class="sxs-lookup"><span data-stu-id="1d16c-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d16c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d16c-126">Authorization</span></span>|<span data-ttu-id="1d16c-127">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1d16c-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d16c-128">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1d16c-128">Accept</span></span>|<span data-ttu-id="1d16c-129">application/json</span><span class="sxs-lookup"><span data-stu-id="1d16c-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d16c-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1d16c-130">Request body</span></span>
<span data-ttu-id="1d16c-131">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [reportRoot](../resources/intune-shared-reportroot.md) an.</span><span class="sxs-lookup"><span data-stu-id="1d16c-131">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="1d16c-132">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [reportRoot](../resources/intune-shared-reportroot.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="1d16c-132">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="1d16c-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1d16c-133">Property</span></span>|<span data-ttu-id="1d16c-134">Typ</span><span class="sxs-lookup"><span data-stu-id="1d16c-134">Type</span></span>|<span data-ttu-id="1d16c-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d16c-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d16c-136">id</span><span class="sxs-lookup"><span data-stu-id="1d16c-136">id</span></span>|<span data-ttu-id="1d16c-137">String</span><span class="sxs-lookup"><span data-stu-id="1d16c-137">String</span></span>|<span data-ttu-id="1d16c-138">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="1d16c-138">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="1d16c-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d16c-139">Response</span></span>
<span data-ttu-id="1d16c-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [reportRoot](../resources/intune-shared-reportroot.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1d16c-140">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d16c-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1d16c-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="1d16c-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d16c-142">Request</span></span>
<span data-ttu-id="1d16c-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1d16c-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="1d16c-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d16c-144">Response</span></span>
<span data-ttu-id="1d16c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1d16c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```



