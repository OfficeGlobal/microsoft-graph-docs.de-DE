---
title: CartToClassAssociation aktualisieren
description: Aktualisieren der Eigenschaften eines cartToClassAssociation-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 09e83b523145f79d610b1299d61fafc5d0a03b02
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964479"
---
# <a name="update-carttoclassassociation"></a><span data-ttu-id="306d0-103">CartToClassAssociation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="306d0-103">Update cartToClassAssociation</span></span>

> <span data-ttu-id="306d0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="306d0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="306d0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="306d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="306d0-106">Aktualisieren der Eigenschaften eines [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="306d0-106">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="306d0-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="306d0-107">Prerequisites</span></span>
<span data-ttu-id="306d0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="306d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="306d0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="306d0-110">Permission type</span></span>|<span data-ttu-id="306d0-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="306d0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="306d0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="306d0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="306d0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="306d0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="306d0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="306d0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="306d0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="306d0-115">Not supported.</span></span>|
|<span data-ttu-id="306d0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="306d0-116">Application</span></span>|<span data-ttu-id="306d0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="306d0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="306d0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="306d0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## <a name="request-headers"></a><span data-ttu-id="306d0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="306d0-119">Request headers</span></span>
|<span data-ttu-id="306d0-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="306d0-120">Header</span></span>|<span data-ttu-id="306d0-121">Wert</span><span class="sxs-lookup"><span data-stu-id="306d0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="306d0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="306d0-122">Authorization</span></span>|<span data-ttu-id="306d0-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="306d0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="306d0-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="306d0-124">Accept</span></span>|<span data-ttu-id="306d0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="306d0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="306d0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="306d0-126">Request body</span></span>
<span data-ttu-id="306d0-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="306d0-127">In the request body, supply a JSON representation for the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

<span data-ttu-id="306d0-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="306d0-128">The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>

|<span data-ttu-id="306d0-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="306d0-129">Property</span></span>|<span data-ttu-id="306d0-130">Typ</span><span class="sxs-lookup"><span data-stu-id="306d0-130">Type</span></span>|<span data-ttu-id="306d0-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="306d0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="306d0-132">id</span><span class="sxs-lookup"><span data-stu-id="306d0-132">id</span></span>|<span data-ttu-id="306d0-133">String</span><span class="sxs-lookup"><span data-stu-id="306d0-133">String</span></span>|<span data-ttu-id="306d0-134">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="306d0-134">Key of the entity.</span></span>|
|<span data-ttu-id="306d0-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="306d0-135">createdDateTime</span></span>|<span data-ttu-id="306d0-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="306d0-136">DateTimeOffset</span></span>|<span data-ttu-id="306d0-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="306d0-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="306d0-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="306d0-138">lastModifiedDateTime</span></span>|<span data-ttu-id="306d0-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="306d0-139">DateTimeOffset</span></span>|<span data-ttu-id="306d0-140">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="306d0-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="306d0-141">Version</span><span class="sxs-lookup"><span data-stu-id="306d0-141">version</span></span>|<span data-ttu-id="306d0-142">Int32</span><span class="sxs-lookup"><span data-stu-id="306d0-142">Int32</span></span>|<span data-ttu-id="306d0-143">Version von CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="306d0-143">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="306d0-144">displayName</span><span class="sxs-lookup"><span data-stu-id="306d0-144">displayName</span></span>|<span data-ttu-id="306d0-145">String</span><span class="sxs-lookup"><span data-stu-id="306d0-145">String</span></span>|<span data-ttu-id="306d0-146">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="306d0-146">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="306d0-147">description</span><span class="sxs-lookup"><span data-stu-id="306d0-147">description</span></span>|<span data-ttu-id="306d0-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="306d0-148">String</span></span>|<span data-ttu-id="306d0-149">Der Administrator hat die Beschreibung des CartToClassAssociation bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="306d0-149">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="306d0-150">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="306d0-150">deviceCartIds</span></span>|<span data-ttu-id="306d0-151">String collection</span><span class="sxs-lookup"><span data-stu-id="306d0-151">String collection</span></span>|<span data-ttu-id="306d0-152">Bezeichner von Gerätewagen, die Klassen zugeordnet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="306d0-152">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="306d0-153">classroomIds</span><span class="sxs-lookup"><span data-stu-id="306d0-153">classroomIds</span></span>|<span data-ttu-id="306d0-154">String collection</span><span class="sxs-lookup"><span data-stu-id="306d0-154">String collection</span></span>|<span data-ttu-id="306d0-155">Bezeichner der Unterrichtsräume, die mit Geräte Körben verknüpft werden sollen.</span><span class="sxs-lookup"><span data-stu-id="306d0-155">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="306d0-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="306d0-156">Response</span></span>
<span data-ttu-id="306d0-157">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="306d0-157">If successful, this method returns a `200 OK` response code and an updated [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="306d0-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="306d0-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="306d0-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="306d0-159">Request</span></span>
<span data-ttu-id="306d0-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="306d0-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
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

### <a name="response"></a><span data-ttu-id="306d0-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="306d0-161">Response</span></span>
<span data-ttu-id="306d0-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="306d0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




