---
title: deviceCategory erstellen
description: Erstellen eines neuen deviceCategory-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 76c1d0c8b22484b3a35d0db49c5a4e578e656880
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255171"
---
# <a name="create-devicecategory"></a><span data-ttu-id="ac070-103">deviceCategory erstellen</span><span class="sxs-lookup"><span data-stu-id="ac070-103">Create deviceCategory</span></span>

> <span data-ttu-id="ac070-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ac070-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac070-105">Erstellen eines neuen [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ac070-105">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac070-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ac070-106">Prerequisites</span></span>
<span data-ttu-id="ac070-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac070-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac070-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ac070-109">Permission type</span></span>|<span data-ttu-id="ac070-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ac070-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac070-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ac070-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ac070-112">&nbsp; &nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="ac070-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="ac070-113">DeviceManagementManaged Devices. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="ac070-113">DeviceManagementManaged Devices.ReadWrite.All</span></span>|
|<span data-ttu-id="ac070-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ac070-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac070-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ac070-115">Not supported.</span></span>|
|<span data-ttu-id="ac070-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ac070-116">Application</span></span>|<span data-ttu-id="ac070-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ac070-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac070-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac070-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="ac070-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ac070-119">Request headers</span></span>
|<span data-ttu-id="ac070-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ac070-120">Header</span></span>|<span data-ttu-id="ac070-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ac070-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac070-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac070-122">Authorization</span></span>|<span data-ttu-id="ac070-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ac070-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac070-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ac070-124">Accept</span></span>|<span data-ttu-id="ac070-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ac070-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac070-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ac070-126">Request body</span></span>
<span data-ttu-id="ac070-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekt des Typs deviceCategory an.</span><span class="sxs-lookup"><span data-stu-id="ac070-127">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="ac070-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceCategory erstellen.</span><span class="sxs-lookup"><span data-stu-id="ac070-128">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="ac070-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ac070-129">Property</span></span>|<span data-ttu-id="ac070-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ac070-130">Type</span></span>|<span data-ttu-id="ac070-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac070-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac070-132">id</span><span class="sxs-lookup"><span data-stu-id="ac070-132">id</span></span>|<span data-ttu-id="ac070-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ac070-133">String</span></span>|<span data-ttu-id="ac070-134">Eindeutiger Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="ac070-134">Unique identifier for the device category.</span></span> <span data-ttu-id="ac070-135">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ac070-135">Read-only.</span></span>|
|<span data-ttu-id="ac070-136">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="ac070-136">**Onboarding**</span></span>|
|<span data-ttu-id="ac070-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ac070-137">displayName</span></span>|<span data-ttu-id="ac070-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ac070-138">String</span></span>|<span data-ttu-id="ac070-139">Der Anzeigename für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="ac070-139">Display name for the device category.</span></span>|
|<span data-ttu-id="ac070-140">description</span><span class="sxs-lookup"><span data-stu-id="ac070-140">description</span></span>|<span data-ttu-id="ac070-141">String</span><span class="sxs-lookup"><span data-stu-id="ac070-141">String</span></span>|<span data-ttu-id="ac070-142">Optionale Beschreibung für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="ac070-142">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="ac070-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac070-143">Response</span></span>
<span data-ttu-id="ac070-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ac070-144">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac070-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ac070-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="ac070-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac070-146">Request</span></span>
<span data-ttu-id="ac070-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ac070-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="ac070-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac070-148">Response</span></span>
<span data-ttu-id="ac070-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ac070-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



