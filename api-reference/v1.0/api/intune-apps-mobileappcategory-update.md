---
title: Aktualisieren von „mobileAppCategory“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs mobileAppCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e20f15e17df63ec706880922fedb6b1c80e646a4
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252546"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="2407b-103">Aktualisieren von „mobileAppCategory“</span><span class="sxs-lookup"><span data-stu-id="2407b-103">Update mobileAppCategory</span></span>

> <span data-ttu-id="2407b-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2407b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2407b-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="2407b-105">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2407b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2407b-106">Prerequisites</span></span>
<span data-ttu-id="2407b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2407b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2407b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2407b-109">Permission type</span></span>|<span data-ttu-id="2407b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2407b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2407b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2407b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2407b-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2407b-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2407b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2407b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2407b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2407b-114">Not supported.</span></span>|
|<span data-ttu-id="2407b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2407b-115">Application</span></span>|<span data-ttu-id="2407b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2407b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2407b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2407b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="2407b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2407b-118">Request headers</span></span>
|<span data-ttu-id="2407b-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2407b-119">Header</span></span>|<span data-ttu-id="2407b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2407b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2407b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2407b-121">Authorization</span></span>|<span data-ttu-id="2407b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2407b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2407b-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2407b-123">Accept</span></span>|<span data-ttu-id="2407b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2407b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2407b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2407b-125">Request body</span></span>
<span data-ttu-id="2407b-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekt des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) an.</span><span class="sxs-lookup"><span data-stu-id="2407b-126">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="2407b-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="2407b-127">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="2407b-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2407b-128">Property</span></span>|<span data-ttu-id="2407b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="2407b-129">Type</span></span>|<span data-ttu-id="2407b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2407b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2407b-131">id</span><span class="sxs-lookup"><span data-stu-id="2407b-131">id</span></span>|<span data-ttu-id="2407b-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2407b-132">String</span></span>|<span data-ttu-id="2407b-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2407b-133">The key of the entity.</span></span>|
|<span data-ttu-id="2407b-134">displayName</span><span class="sxs-lookup"><span data-stu-id="2407b-134">displayName</span></span>|<span data-ttu-id="2407b-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2407b-135">String</span></span>|<span data-ttu-id="2407b-136">Name der App-Kategorie</span><span class="sxs-lookup"><span data-stu-id="2407b-136">The name of the app category.</span></span>|
|<span data-ttu-id="2407b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2407b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2407b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2407b-138">DateTimeOffset</span></span>|<span data-ttu-id="2407b-139">Datum und Uhrzeit der letzten Änderung des Objekts des Typs „mobileAppCategory“</span><span class="sxs-lookup"><span data-stu-id="2407b-139">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="2407b-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="2407b-140">Response</span></span>
<span data-ttu-id="2407b-141">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2407b-141">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2407b-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2407b-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="2407b-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2407b-143">Request</span></span>
<span data-ttu-id="2407b-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2407b-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="2407b-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="2407b-145">Response</span></span>
<span data-ttu-id="2407b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2407b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```



