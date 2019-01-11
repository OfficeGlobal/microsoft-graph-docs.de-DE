---
title: deviceCategory erstellen
description: Erstellen eines neuen deviceCategory-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 61a114e86b50e5992c7614d14ae4734bfc879657
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861628"
---
# <a name="create-devicecategory"></a><span data-ttu-id="71d08-103">deviceCategory erstellen</span><span class="sxs-lookup"><span data-stu-id="71d08-103">Create deviceCategory</span></span>

> <span data-ttu-id="71d08-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="71d08-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71d08-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="71d08-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71d08-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="71d08-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71d08-107">Erstellen eines neuen [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="71d08-107">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71d08-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="71d08-108">Prerequisites</span></span>

<span data-ttu-id="71d08-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71d08-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71d08-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71d08-111">Permission type</span></span>|<span data-ttu-id="71d08-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71d08-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71d08-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71d08-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="71d08-114">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="71d08-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="71d08-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71d08-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="71d08-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71d08-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71d08-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71d08-117">Not supported.</span></span>|
|<span data-ttu-id="71d08-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71d08-118">Application</span></span>|<span data-ttu-id="71d08-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71d08-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71d08-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71d08-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="71d08-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71d08-121">Request headers</span></span>

|<span data-ttu-id="71d08-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="71d08-122">Header</span></span>|<span data-ttu-id="71d08-123">Wert</span><span class="sxs-lookup"><span data-stu-id="71d08-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71d08-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="71d08-124">Authorization</span></span>|<span data-ttu-id="71d08-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="71d08-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71d08-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="71d08-126">Accept</span></span>|<span data-ttu-id="71d08-127">application/json</span><span class="sxs-lookup"><span data-stu-id="71d08-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71d08-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71d08-128">Request body</span></span>

<span data-ttu-id="71d08-129">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekt des Typs deviceCategory an.</span><span class="sxs-lookup"><span data-stu-id="71d08-129">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="71d08-130">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceCategory erstellen.</span><span class="sxs-lookup"><span data-stu-id="71d08-130">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="71d08-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71d08-131">Property</span></span>|<span data-ttu-id="71d08-132">Typ</span><span class="sxs-lookup"><span data-stu-id="71d08-132">Type</span></span>|<span data-ttu-id="71d08-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71d08-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71d08-134">id</span><span class="sxs-lookup"><span data-stu-id="71d08-134">id</span></span>|<span data-ttu-id="71d08-135">String</span><span class="sxs-lookup"><span data-stu-id="71d08-135">String</span></span>|<span data-ttu-id="71d08-136">Eindeutiger Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="71d08-136">Unique identifier for the device category.</span></span> <span data-ttu-id="71d08-137">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="71d08-137">Read-only.</span></span>|
|<span data-ttu-id="71d08-138">**Obboarding**</span><span class="sxs-lookup"><span data-stu-id="71d08-138">**Obboarding**</span></span>|
|<span data-ttu-id="71d08-139">description</span><span class="sxs-lookup"><span data-stu-id="71d08-139">description</span></span>|<span data-ttu-id="71d08-140">String</span><span class="sxs-lookup"><span data-stu-id="71d08-140">String</span></span>|<span data-ttu-id="71d08-141">Optionale Beschreibung für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="71d08-141">Optional description for the device category.</span></span>|
|<span data-ttu-id="71d08-142">displayName</span><span class="sxs-lookup"><span data-stu-id="71d08-142">displayName</span></span>|<span data-ttu-id="71d08-143">String</span><span class="sxs-lookup"><span data-stu-id="71d08-143">String</span></span>|<span data-ttu-id="71d08-144">Der Anzeigename für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="71d08-144">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="71d08-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="71d08-145">Response</span></span>

<span data-ttu-id="71d08-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71d08-146">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71d08-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71d08-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="71d08-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71d08-148">Request</span></span>

<span data-ttu-id="71d08-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71d08-149">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="71d08-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="71d08-150">Response</span></span>

<span data-ttu-id="71d08-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71d08-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



