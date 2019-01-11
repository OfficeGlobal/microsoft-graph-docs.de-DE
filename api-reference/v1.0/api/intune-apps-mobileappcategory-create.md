---
title: Erstellen von „mobileAppCategory“
description: Diese Methode erstellt ein neues Objekt des Typs mobileAppCategory.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c09b557da645767e090bfecca7974c0af41b17f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870798"
---
# <a name="create-mobileappcategory"></a><span data-ttu-id="d5a75-103">Erstellen von „mobileAppCategory“</span><span class="sxs-lookup"><span data-stu-id="d5a75-103">Create mobileAppCategory</span></span>

> <span data-ttu-id="d5a75-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d5a75-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5a75-105">Diese Methode erstellt ein neues Objekt des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="d5a75-105">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d5a75-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d5a75-106">Prerequisites</span></span>
<span data-ttu-id="d5a75-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5a75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5a75-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d5a75-109">Permission type</span></span>|<span data-ttu-id="d5a75-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d5a75-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5a75-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d5a75-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d5a75-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5a75-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d5a75-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d5a75-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5a75-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d5a75-114">Not supported.</span></span>|
|<span data-ttu-id="d5a75-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d5a75-115">Application</span></span>|<span data-ttu-id="d5a75-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d5a75-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5a75-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5a75-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppCategories
POST /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="d5a75-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d5a75-118">Request headers</span></span>
|<span data-ttu-id="d5a75-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d5a75-119">Header</span></span>|<span data-ttu-id="d5a75-120">Wert</span><span class="sxs-lookup"><span data-stu-id="d5a75-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5a75-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5a75-121">Authorization</span></span>|<span data-ttu-id="d5a75-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d5a75-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5a75-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d5a75-123">Accept</span></span>|<span data-ttu-id="d5a75-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d5a75-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5a75-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d5a75-125">Request body</span></span>
<span data-ttu-id="d5a75-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mobileAppCategory“ an.</span><span class="sxs-lookup"><span data-stu-id="d5a75-126">In the request body, supply a JSON representation for the mobileAppCategory object.</span></span>

<span data-ttu-id="d5a75-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mobileAppCategory“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="d5a75-127">The following table shows the properties that are required when you create the mobileAppCategory.</span></span>

|<span data-ttu-id="d5a75-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d5a75-128">Property</span></span>|<span data-ttu-id="d5a75-129">Typ</span><span class="sxs-lookup"><span data-stu-id="d5a75-129">Type</span></span>|<span data-ttu-id="d5a75-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d5a75-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5a75-131">id</span><span class="sxs-lookup"><span data-stu-id="d5a75-131">id</span></span>|<span data-ttu-id="d5a75-132">String</span><span class="sxs-lookup"><span data-stu-id="d5a75-132">String</span></span>|<span data-ttu-id="d5a75-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d5a75-133">The key of the entity.</span></span>|
|<span data-ttu-id="d5a75-134">displayName</span><span class="sxs-lookup"><span data-stu-id="d5a75-134">displayName</span></span>|<span data-ttu-id="d5a75-135">String</span><span class="sxs-lookup"><span data-stu-id="d5a75-135">String</span></span>|<span data-ttu-id="d5a75-136">Name der App-Kategorie</span><span class="sxs-lookup"><span data-stu-id="d5a75-136">The name of the app category.</span></span>|
|<span data-ttu-id="d5a75-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5a75-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d5a75-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5a75-138">DateTimeOffset</span></span>|<span data-ttu-id="d5a75-139">Datum und Uhrzeit der letzten Änderung des Objekts des Typs „mobileAppCategory“</span><span class="sxs-lookup"><span data-stu-id="d5a75-139">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="d5a75-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5a75-140">Response</span></span>
<span data-ttu-id="d5a75-141">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d5a75-141">If successful, this method returns a `201 Created` response code and a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5a75-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d5a75-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="d5a75-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5a75-143">Request</span></span>
<span data-ttu-id="d5a75-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d5a75-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="d5a75-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5a75-145">Response</span></span>
<span data-ttu-id="d5a75-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d5a75-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



