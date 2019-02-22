---
title: CartToClassAssociation erstellen
description: Erstellen eines neuen cartToClassAssociation-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4fe03f073fec54db6f9136ed104033e1deaf857
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150085"
---
# <a name="create-carttoclassassociation"></a><span data-ttu-id="c4ca1-103">CartToClassAssociation erstellen</span><span class="sxs-lookup"><span data-stu-id="c4ca1-103">Create cartToClassAssociation</span></span>

> <span data-ttu-id="c4ca1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c4ca1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4ca1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c4ca1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4ca1-106">Erstellen eines neuen [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c4ca1-106">Create a new [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4ca1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c4ca1-107">Prerequisites</span></span>
<span data-ttu-id="c4ca1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c4ca1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c4ca1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c4ca1-110">Permission type</span></span>|<span data-ttu-id="c4ca1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c4ca1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4ca1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c4ca1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c4ca1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4ca1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c4ca1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c4ca1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4ca1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c4ca1-115">Not supported.</span></span>|
|<span data-ttu-id="c4ca1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c4ca1-116">Application</span></span>|<span data-ttu-id="c4ca1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c4ca1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4ca1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c4ca1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cartToClassAssociations
```

## <a name="request-headers"></a><span data-ttu-id="c4ca1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c4ca1-119">Request headers</span></span>
|<span data-ttu-id="c4ca1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c4ca1-120">Header</span></span>|<span data-ttu-id="c4ca1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c4ca1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4ca1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4ca1-122">Authorization</span></span>|<span data-ttu-id="c4ca1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c4ca1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4ca1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c4ca1-124">Accept</span></span>|<span data-ttu-id="c4ca1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c4ca1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4ca1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c4ca1-126">Request body</span></span>
<span data-ttu-id="c4ca1-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das cartToClassAssociation-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c4ca1-127">In the request body, supply a JSON representation for the cartToClassAssociation object.</span></span>

<span data-ttu-id="c4ca1-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der cartToClassAssociation erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c4ca1-128">The following table shows the properties that are required when you create the cartToClassAssociation.</span></span>

|<span data-ttu-id="c4ca1-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c4ca1-129">Property</span></span>|<span data-ttu-id="c4ca1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c4ca1-130">Type</span></span>|<span data-ttu-id="c4ca1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4ca1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4ca1-132">id</span><span class="sxs-lookup"><span data-stu-id="c4ca1-132">id</span></span>|<span data-ttu-id="c4ca1-133">string</span><span class="sxs-lookup"><span data-stu-id="c4ca1-133">String</span></span>|<span data-ttu-id="c4ca1-134">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="c4ca1-134">Key of the entity.</span></span>|
|<span data-ttu-id="c4ca1-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4ca1-135">createdDateTime</span></span>|<span data-ttu-id="c4ca1-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4ca1-136">DateTimeOffset</span></span>|<span data-ttu-id="c4ca1-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c4ca1-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="c4ca1-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4ca1-138">lastModifiedDateTime</span></span>|<span data-ttu-id="c4ca1-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4ca1-139">DateTimeOffset</span></span>|<span data-ttu-id="c4ca1-140">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c4ca1-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c4ca1-141">Version</span><span class="sxs-lookup"><span data-stu-id="c4ca1-141">version</span></span>|<span data-ttu-id="c4ca1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="c4ca1-142">Int32</span></span>|<span data-ttu-id="c4ca1-143">Version von CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="c4ca1-143">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="c4ca1-144">displayName</span><span class="sxs-lookup"><span data-stu-id="c4ca1-144">displayName</span></span>|<span data-ttu-id="c4ca1-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4ca1-145">String</span></span>|<span data-ttu-id="c4ca1-146">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c4ca1-146">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="c4ca1-147">description</span><span class="sxs-lookup"><span data-stu-id="c4ca1-147">description</span></span>|<span data-ttu-id="c4ca1-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4ca1-148">String</span></span>|<span data-ttu-id="c4ca1-149">Der Administrator hat die Beschreibung des CartToClassAssociation bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="c4ca1-149">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="c4ca1-150">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="c4ca1-150">deviceCartIds</span></span>|<span data-ttu-id="c4ca1-151">String collection</span><span class="sxs-lookup"><span data-stu-id="c4ca1-151">String collection</span></span>|<span data-ttu-id="c4ca1-152">Bezeichner von Gerätewagen, die Klassen zugeordnet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c4ca1-152">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="c4ca1-153">classroomIds</span><span class="sxs-lookup"><span data-stu-id="c4ca1-153">classroomIds</span></span>|<span data-ttu-id="c4ca1-154">String collection</span><span class="sxs-lookup"><span data-stu-id="c4ca1-154">String collection</span></span>|<span data-ttu-id="c4ca1-155">Bezeichner der Unterrichtsräume, die mit Geräte Körben verknüpft werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c4ca1-155">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="c4ca1-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="c4ca1-156">Response</span></span>
<span data-ttu-id="c4ca1-157">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c4ca1-157">If successful, this method returns a `201 Created` response code and a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4ca1-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c4ca1-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4ca1-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c4ca1-159">Request</span></span>
<span data-ttu-id="c4ca1-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c4ca1-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
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

### <a name="response"></a><span data-ttu-id="c4ca1-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="c4ca1-161">Response</span></span>
<span data-ttu-id="c4ca1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c4ca1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




