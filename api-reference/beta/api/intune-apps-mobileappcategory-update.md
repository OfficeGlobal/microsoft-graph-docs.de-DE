---
title: Aktualisieren von „mobileAppCategory“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs mobileAppCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 868450fa8e6a0105fefd8eb60dfc6c8a64dda87c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171283"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="4421a-103">Aktualisieren von „mobileAppCategory“</span><span class="sxs-lookup"><span data-stu-id="4421a-103">Update mobileAppCategory</span></span>

> <span data-ttu-id="4421a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4421a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4421a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4421a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4421a-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="4421a-106">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4421a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4421a-107">Prerequisites</span></span>
<span data-ttu-id="4421a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4421a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4421a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4421a-110">Permission type</span></span>|<span data-ttu-id="4421a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4421a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4421a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4421a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4421a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4421a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4421a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4421a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4421a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4421a-115">Not supported.</span></span>|
|<span data-ttu-id="4421a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4421a-116">Application</span></span>|<span data-ttu-id="4421a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4421a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4421a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4421a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="4421a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4421a-119">Request headers</span></span>
|<span data-ttu-id="4421a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4421a-120">Header</span></span>|<span data-ttu-id="4421a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4421a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4421a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4421a-122">Authorization</span></span>|<span data-ttu-id="4421a-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4421a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4421a-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4421a-124">Accept</span></span>|<span data-ttu-id="4421a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4421a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4421a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4421a-126">Request body</span></span>
<span data-ttu-id="4421a-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekt des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) an.</span><span class="sxs-lookup"><span data-stu-id="4421a-127">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="4421a-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="4421a-128">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="4421a-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4421a-129">Property</span></span>|<span data-ttu-id="4421a-130">Typ</span><span class="sxs-lookup"><span data-stu-id="4421a-130">Type</span></span>|<span data-ttu-id="4421a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4421a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4421a-132">id</span><span class="sxs-lookup"><span data-stu-id="4421a-132">id</span></span>|<span data-ttu-id="4421a-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4421a-133">String</span></span>|<span data-ttu-id="4421a-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4421a-134">The key of the entity.</span></span>|
|<span data-ttu-id="4421a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4421a-135">displayName</span></span>|<span data-ttu-id="4421a-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4421a-136">String</span></span>|<span data-ttu-id="4421a-137">Name der App-Kategorie</span><span class="sxs-lookup"><span data-stu-id="4421a-137">The name of the app category.</span></span>|
|<span data-ttu-id="4421a-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4421a-138">lastModifiedDateTime</span></span>|<span data-ttu-id="4421a-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4421a-139">DateTimeOffset</span></span>|<span data-ttu-id="4421a-140">Datum und Uhrzeit der letzten Änderung des Objekts des Typs „mobileAppCategory“</span><span class="sxs-lookup"><span data-stu-id="4421a-140">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="4421a-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="4421a-141">Response</span></span>
<span data-ttu-id="4421a-142">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4421a-142">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4421a-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4421a-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="4421a-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4421a-144">Request</span></span>
<span data-ttu-id="4421a-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4421a-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="4421a-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="4421a-146">Response</span></span>
<span data-ttu-id="4421a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4421a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




