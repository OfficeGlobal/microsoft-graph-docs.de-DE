---
title: Erstellen von cartToClassAssociation
description: Erstellen eines neuen CartToClassAssociation-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6e3582f3f38258db75236b6cc877a64471da4b85
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822708"
---
# <a name="create-carttoclassassociation"></a><span data-ttu-id="70bd5-103">Erstellen von cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="70bd5-103">Create cartToClassAssociation</span></span>

> <span data-ttu-id="70bd5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="70bd5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70bd5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="70bd5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70bd5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="70bd5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70bd5-107">Erstellen eines neuen [CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="70bd5-107">Create a new [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="70bd5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="70bd5-108">Prerequisites</span></span>
<span data-ttu-id="70bd5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70bd5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70bd5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="70bd5-111">Permission type</span></span>|<span data-ttu-id="70bd5-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="70bd5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70bd5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="70bd5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70bd5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70bd5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="70bd5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="70bd5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70bd5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70bd5-116">Not supported.</span></span>|
|<span data-ttu-id="70bd5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="70bd5-117">Application</span></span>|<span data-ttu-id="70bd5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70bd5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70bd5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="70bd5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cartToClassAssociations
```

## <a name="request-headers"></a><span data-ttu-id="70bd5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="70bd5-120">Request headers</span></span>
|<span data-ttu-id="70bd5-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="70bd5-121">Header</span></span>|<span data-ttu-id="70bd5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="70bd5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70bd5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="70bd5-123">Authorization</span></span>|<span data-ttu-id="70bd5-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="70bd5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70bd5-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="70bd5-125">Accept</span></span>|<span data-ttu-id="70bd5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70bd5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70bd5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="70bd5-127">Request body</span></span>
<span data-ttu-id="70bd5-128">Geben Sie im Textkörper Anforderung für das Objekt CartToClassAssociation eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="70bd5-128">In the request body, supply a JSON representation for the cartToClassAssociation object.</span></span>

<span data-ttu-id="70bd5-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die CartToClassAssociation erstellen.</span><span class="sxs-lookup"><span data-stu-id="70bd5-129">The following table shows the properties that are required when you create the cartToClassAssociation.</span></span>

|<span data-ttu-id="70bd5-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="70bd5-130">Property</span></span>|<span data-ttu-id="70bd5-131">Typ</span><span class="sxs-lookup"><span data-stu-id="70bd5-131">Type</span></span>|<span data-ttu-id="70bd5-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70bd5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70bd5-133">id</span><span class="sxs-lookup"><span data-stu-id="70bd5-133">id</span></span>|<span data-ttu-id="70bd5-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70bd5-134">String</span></span>|<span data-ttu-id="70bd5-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="70bd5-135">Key of the entity.</span></span>|
|<span data-ttu-id="70bd5-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70bd5-136">createdDateTime</span></span>|<span data-ttu-id="70bd5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70bd5-137">DateTimeOffset</span></span>|<span data-ttu-id="70bd5-138">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="70bd5-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="70bd5-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70bd5-139">lastModifiedDateTime</span></span>|<span data-ttu-id="70bd5-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70bd5-140">DateTimeOffset</span></span>|<span data-ttu-id="70bd5-141">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="70bd5-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="70bd5-142">Version</span><span class="sxs-lookup"><span data-stu-id="70bd5-142">version</span></span>|<span data-ttu-id="70bd5-143">Int32</span><span class="sxs-lookup"><span data-stu-id="70bd5-143">Int32</span></span>|<span data-ttu-id="70bd5-144">Version der CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="70bd5-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="70bd5-145">displayName</span><span class="sxs-lookup"><span data-stu-id="70bd5-145">displayName</span></span>|<span data-ttu-id="70bd5-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70bd5-146">String</span></span>|<span data-ttu-id="70bd5-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="70bd5-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="70bd5-148">description</span><span class="sxs-lookup"><span data-stu-id="70bd5-148">description</span></span>|<span data-ttu-id="70bd5-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70bd5-149">String</span></span>|<span data-ttu-id="70bd5-150">Admin bereitgestellte Beschreibung für die CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="70bd5-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="70bd5-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="70bd5-151">deviceCartIds</span></span>|<span data-ttu-id="70bd5-152">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="70bd5-152">String collection</span></span>|<span data-ttu-id="70bd5-153">Bezeichner des Geräts Toilettengebäude Klassen zugeordnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="70bd5-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="70bd5-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="70bd5-154">classroomIds</span></span>|<span data-ttu-id="70bd5-155">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="70bd5-155">String collection</span></span>|<span data-ttu-id="70bd5-156">Die IDs der Schulungsräume Gerät Toilettengebäude zugeordnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="70bd5-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="70bd5-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="70bd5-157">Response</span></span>
<span data-ttu-id="70bd5-158">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="70bd5-158">If successful, this method returns a `201 Created` response code and a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70bd5-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="70bd5-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="70bd5-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="70bd5-160">Request</span></span>
<span data-ttu-id="70bd5-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="70bd5-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
Content-type: application/json
Content-length: 335

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="70bd5-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="70bd5-162">Response</span></span>
<span data-ttu-id="70bd5-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70bd5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "9bdc58dd-58dd-9bdc-dd58-dc9bdd58dc9b",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```





