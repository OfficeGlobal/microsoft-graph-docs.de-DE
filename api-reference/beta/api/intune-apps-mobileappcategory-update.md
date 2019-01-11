---
title: Aktualisieren von „mobileAppCategory“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs mobileAppCategory.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bb21e4e3b564f50538f7399f8715c7f55a56b58b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869776"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="e2c06-103">Aktualisieren von „mobileAppCategory“</span><span class="sxs-lookup"><span data-stu-id="e2c06-103">Update mobileAppCategory</span></span>

> <span data-ttu-id="e2c06-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e2c06-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2c06-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e2c06-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2c06-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e2c06-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2c06-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="e2c06-107">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e2c06-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e2c06-108">Prerequisites</span></span>
<span data-ttu-id="e2c06-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2c06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2c06-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e2c06-111">Permission type</span></span>|<span data-ttu-id="e2c06-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e2c06-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2c06-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e2c06-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2c06-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2c06-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e2c06-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e2c06-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2c06-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e2c06-116">Not supported.</span></span>|
|<span data-ttu-id="e2c06-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e2c06-117">Application</span></span>|<span data-ttu-id="e2c06-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e2c06-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2c06-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2c06-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="e2c06-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e2c06-120">Request headers</span></span>
|<span data-ttu-id="e2c06-121">Header</span><span class="sxs-lookup"><span data-stu-id="e2c06-121">Header</span></span>|<span data-ttu-id="e2c06-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e2c06-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2c06-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2c06-123">Authorization</span></span>|<span data-ttu-id="e2c06-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e2c06-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2c06-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e2c06-125">Accept</span></span>|<span data-ttu-id="e2c06-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2c06-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2c06-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e2c06-127">Request body</span></span>
<span data-ttu-id="e2c06-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekt des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) an.</span><span class="sxs-lookup"><span data-stu-id="e2c06-128">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="e2c06-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="e2c06-129">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="e2c06-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e2c06-130">Property</span></span>|<span data-ttu-id="e2c06-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e2c06-131">Type</span></span>|<span data-ttu-id="e2c06-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2c06-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2c06-133">id</span><span class="sxs-lookup"><span data-stu-id="e2c06-133">id</span></span>|<span data-ttu-id="e2c06-134">String</span><span class="sxs-lookup"><span data-stu-id="e2c06-134">String</span></span>|<span data-ttu-id="e2c06-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e2c06-135">The key of the entity.</span></span>|
|<span data-ttu-id="e2c06-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e2c06-136">displayName</span></span>|<span data-ttu-id="e2c06-137">String</span><span class="sxs-lookup"><span data-stu-id="e2c06-137">String</span></span>|<span data-ttu-id="e2c06-138">Name der App-Kategorie</span><span class="sxs-lookup"><span data-stu-id="e2c06-138">The name of the app category.</span></span>|
|<span data-ttu-id="e2c06-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2c06-139">lastModifiedDateTime</span></span>|<span data-ttu-id="e2c06-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2c06-140">DateTimeOffset</span></span>|<span data-ttu-id="e2c06-141">Datum und Uhrzeit der letzten Änderung des Objekts des Typs „mobileAppCategory“</span><span class="sxs-lookup"><span data-stu-id="e2c06-141">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="e2c06-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2c06-142">Response</span></span>
<span data-ttu-id="e2c06-143">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e2c06-143">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2c06-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e2c06-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="e2c06-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2c06-145">Request</span></span>
<span data-ttu-id="e2c06-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e2c06-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 107

{
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="e2c06-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2c06-147">Response</span></span>
<span data-ttu-id="e2c06-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e2c06-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





