---
title: Erstellen von „mobileAppCategory“
description: Diese Methode erstellt ein neues Objekt des Typs mobileAppCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3abe0c2df1695f5e1f27a414265bfc357d832b1a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963849"
---
# <a name="create-mobileappcategory"></a><span data-ttu-id="6dfae-103">Erstellen von „mobileAppCategory“</span><span class="sxs-lookup"><span data-stu-id="6dfae-103">Create mobileAppCategory</span></span>

> <span data-ttu-id="6dfae-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6dfae-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dfae-105">Diese Methode erstellt ein neues Objekt des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="6dfae-105">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6dfae-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6dfae-106">Prerequisites</span></span>
<span data-ttu-id="6dfae-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dfae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dfae-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6dfae-109">Permission type</span></span>|<span data-ttu-id="6dfae-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6dfae-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dfae-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6dfae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6dfae-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dfae-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6dfae-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6dfae-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dfae-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6dfae-114">Not supported.</span></span>|
|<span data-ttu-id="6dfae-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6dfae-115">Application</span></span>|<span data-ttu-id="6dfae-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6dfae-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dfae-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6dfae-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppCategories
POST /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="6dfae-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6dfae-118">Request headers</span></span>
|<span data-ttu-id="6dfae-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6dfae-119">Header</span></span>|<span data-ttu-id="6dfae-120">Wert</span><span class="sxs-lookup"><span data-stu-id="6dfae-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dfae-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dfae-121">Authorization</span></span>|<span data-ttu-id="6dfae-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6dfae-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dfae-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6dfae-123">Accept</span></span>|<span data-ttu-id="6dfae-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6dfae-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dfae-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6dfae-125">Request body</span></span>
<span data-ttu-id="6dfae-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mobileAppCategory“ an.</span><span class="sxs-lookup"><span data-stu-id="6dfae-126">In the request body, supply a JSON representation for the mobileAppCategory object.</span></span>

<span data-ttu-id="6dfae-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mobileAppCategory“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="6dfae-127">The following table shows the properties that are required when you create the mobileAppCategory.</span></span>

|<span data-ttu-id="6dfae-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6dfae-128">Property</span></span>|<span data-ttu-id="6dfae-129">Typ</span><span class="sxs-lookup"><span data-stu-id="6dfae-129">Type</span></span>|<span data-ttu-id="6dfae-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6dfae-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dfae-131">id</span><span class="sxs-lookup"><span data-stu-id="6dfae-131">id</span></span>|<span data-ttu-id="6dfae-132">String</span><span class="sxs-lookup"><span data-stu-id="6dfae-132">String</span></span>|<span data-ttu-id="6dfae-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6dfae-133">The key of the entity.</span></span>|
|<span data-ttu-id="6dfae-134">displayName</span><span class="sxs-lookup"><span data-stu-id="6dfae-134">displayName</span></span>|<span data-ttu-id="6dfae-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6dfae-135">String</span></span>|<span data-ttu-id="6dfae-136">Name der App-Kategorie</span><span class="sxs-lookup"><span data-stu-id="6dfae-136">The name of the app category.</span></span>|
|<span data-ttu-id="6dfae-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6dfae-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6dfae-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6dfae-138">DateTimeOffset</span></span>|<span data-ttu-id="6dfae-139">Datum und Uhrzeit der letzten Änderung des Objekts des Typs „mobileAppCategory“</span><span class="sxs-lookup"><span data-stu-id="6dfae-139">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="6dfae-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="6dfae-140">Response</span></span>
<span data-ttu-id="6dfae-141">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6dfae-141">If successful, this method returns a `201 Created` response code and a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dfae-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6dfae-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="6dfae-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6dfae-143">Request</span></span>
<span data-ttu-id="6dfae-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6dfae-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="6dfae-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="6dfae-145">Response</span></span>
<span data-ttu-id="6dfae-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6dfae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```



