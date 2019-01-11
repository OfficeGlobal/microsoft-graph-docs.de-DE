---
title: Erstellen von „mobileAppCategory“
description: Diese Methode erstellt ein neues Objekt des Typs mobileAppCategory.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a84d141a15a55d95d5429511a8db208f24ed984c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887283"
---
# <a name="create-mobileappcategory"></a><span data-ttu-id="8d65a-103">Erstellen von „mobileAppCategory“</span><span class="sxs-lookup"><span data-stu-id="8d65a-103">Create mobileAppCategory</span></span>

> <span data-ttu-id="8d65a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8d65a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d65a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8d65a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d65a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8d65a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d65a-107">Diese Methode erstellt ein neues Objekt des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="8d65a-107">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8d65a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8d65a-108">Prerequisites</span></span>
<span data-ttu-id="8d65a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d65a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d65a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8d65a-111">Permission type</span></span>|<span data-ttu-id="8d65a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8d65a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d65a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8d65a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d65a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d65a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8d65a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8d65a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d65a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d65a-116">Not supported.</span></span>|
|<span data-ttu-id="8d65a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8d65a-117">Application</span></span>|<span data-ttu-id="8d65a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d65a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d65a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d65a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppCategories
POST /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="8d65a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8d65a-120">Request headers</span></span>
|<span data-ttu-id="8d65a-121">Header</span><span class="sxs-lookup"><span data-stu-id="8d65a-121">Header</span></span>|<span data-ttu-id="8d65a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8d65a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d65a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d65a-123">Authorization</span></span>|<span data-ttu-id="8d65a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8d65a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d65a-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8d65a-125">Accept</span></span>|<span data-ttu-id="8d65a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d65a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d65a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8d65a-127">Request body</span></span>
<span data-ttu-id="8d65a-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mobileAppCategory“ an.</span><span class="sxs-lookup"><span data-stu-id="8d65a-128">In the request body, supply a JSON representation for the mobileAppCategory object.</span></span>

<span data-ttu-id="8d65a-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mobileAppCategory“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="8d65a-129">The following table shows the properties that are required when you create the mobileAppCategory.</span></span>

|<span data-ttu-id="8d65a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8d65a-130">Property</span></span>|<span data-ttu-id="8d65a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8d65a-131">Type</span></span>|<span data-ttu-id="8d65a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d65a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d65a-133">id</span><span class="sxs-lookup"><span data-stu-id="8d65a-133">id</span></span>|<span data-ttu-id="8d65a-134">String</span><span class="sxs-lookup"><span data-stu-id="8d65a-134">String</span></span>|<span data-ttu-id="8d65a-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8d65a-135">The key of the entity.</span></span>|
|<span data-ttu-id="8d65a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8d65a-136">displayName</span></span>|<span data-ttu-id="8d65a-137">String</span><span class="sxs-lookup"><span data-stu-id="8d65a-137">String</span></span>|<span data-ttu-id="8d65a-138">Name der App-Kategorie</span><span class="sxs-lookup"><span data-stu-id="8d65a-138">The name of the app category.</span></span>|
|<span data-ttu-id="8d65a-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d65a-139">lastModifiedDateTime</span></span>|<span data-ttu-id="8d65a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d65a-140">DateTimeOffset</span></span>|<span data-ttu-id="8d65a-141">Datum und Uhrzeit der letzten Änderung des Objekts des Typs „mobileAppCategory“</span><span class="sxs-lookup"><span data-stu-id="8d65a-141">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="8d65a-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d65a-142">Response</span></span>
<span data-ttu-id="8d65a-143">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8d65a-143">If successful, this method returns a `201 Created` response code and a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d65a-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8d65a-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="8d65a-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d65a-145">Request</span></span>
<span data-ttu-id="8d65a-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8d65a-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories
Content-type: application/json
Content-length: 163

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="8d65a-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d65a-147">Response</span></span>
<span data-ttu-id="8d65a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d65a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





