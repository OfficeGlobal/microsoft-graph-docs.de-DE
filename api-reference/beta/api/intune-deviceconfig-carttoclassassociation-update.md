---
title: CartToClassAssociation aktualisieren
description: Aktualisieren Sie die Eigenschaften eines CartToClassAssociation-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a8da37fa694c0352ade04c1ae9ce9bca926bc126
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396798"
---
# <a name="update-carttoclassassociation"></a><span data-ttu-id="4afdc-103">CartToClassAssociation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4afdc-103">Update cartToClassAssociation</span></span>

> <span data-ttu-id="4afdc-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="4afdc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4afdc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4afdc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4afdc-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4afdc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4afdc-107">Aktualisieren Sie die Eigenschaften eines [CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4afdc-107">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4afdc-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4afdc-108">Prerequisites</span></span>
<span data-ttu-id="4afdc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4afdc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4afdc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4afdc-111">Permission type</span></span>|<span data-ttu-id="4afdc-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4afdc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4afdc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4afdc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4afdc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4afdc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4afdc-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4afdc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4afdc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4afdc-116">Not supported.</span></span>|
|<span data-ttu-id="4afdc-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4afdc-117">Application</span></span>|<span data-ttu-id="4afdc-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4afdc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4afdc-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4afdc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## <a name="request-headers"></a><span data-ttu-id="4afdc-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4afdc-120">Request headers</span></span>
|<span data-ttu-id="4afdc-121">Header</span><span class="sxs-lookup"><span data-stu-id="4afdc-121">Header</span></span>|<span data-ttu-id="4afdc-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4afdc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4afdc-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4afdc-123">Authorization</span></span>|<span data-ttu-id="4afdc-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4afdc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4afdc-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4afdc-125">Accept</span></span>|<span data-ttu-id="4afdc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4afdc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4afdc-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4afdc-127">Request body</span></span>
<span data-ttu-id="4afdc-128">Geben Sie im Textkörper Anforderung für das Objekt [CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="4afdc-128">In the request body, supply a JSON representation for the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

<span data-ttu-id="4afdc-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="4afdc-129">The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>

|<span data-ttu-id="4afdc-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4afdc-130">Property</span></span>|<span data-ttu-id="4afdc-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4afdc-131">Type</span></span>|<span data-ttu-id="4afdc-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4afdc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4afdc-133">id</span><span class="sxs-lookup"><span data-stu-id="4afdc-133">id</span></span>|<span data-ttu-id="4afdc-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4afdc-134">String</span></span>|<span data-ttu-id="4afdc-135">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="4afdc-135">Key of the entity.</span></span>|
|<span data-ttu-id="4afdc-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4afdc-136">createdDateTime</span></span>|<span data-ttu-id="4afdc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4afdc-137">DateTimeOffset</span></span>|<span data-ttu-id="4afdc-138">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4afdc-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="4afdc-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4afdc-139">lastModifiedDateTime</span></span>|<span data-ttu-id="4afdc-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4afdc-140">DateTimeOffset</span></span>|<span data-ttu-id="4afdc-141">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4afdc-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="4afdc-142">Version</span><span class="sxs-lookup"><span data-stu-id="4afdc-142">version</span></span>|<span data-ttu-id="4afdc-143">Int32</span><span class="sxs-lookup"><span data-stu-id="4afdc-143">Int32</span></span>|<span data-ttu-id="4afdc-144">Version der CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="4afdc-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="4afdc-145">displayName</span><span class="sxs-lookup"><span data-stu-id="4afdc-145">displayName</span></span>|<span data-ttu-id="4afdc-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4afdc-146">String</span></span>|<span data-ttu-id="4afdc-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4afdc-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="4afdc-148">description</span><span class="sxs-lookup"><span data-stu-id="4afdc-148">description</span></span>|<span data-ttu-id="4afdc-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4afdc-149">String</span></span>|<span data-ttu-id="4afdc-150">Admin bereitgestellte Beschreibung für die CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="4afdc-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="4afdc-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="4afdc-151">deviceCartIds</span></span>|<span data-ttu-id="4afdc-152">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="4afdc-152">String collection</span></span>|<span data-ttu-id="4afdc-153">Bezeichner des Geräts Toilettengebäude Klassen zugeordnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="4afdc-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="4afdc-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="4afdc-154">classroomIds</span></span>|<span data-ttu-id="4afdc-155">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="4afdc-155">String collection</span></span>|<span data-ttu-id="4afdc-156">Die IDs der Schulungsräume Gerät Toilettengebäude zugeordnet werden soll.</span><span class="sxs-lookup"><span data-stu-id="4afdc-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="4afdc-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="4afdc-157">Response</span></span>
<span data-ttu-id="4afdc-158">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4afdc-158">If successful, this method returns a `200 OK` response code and an updated [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4afdc-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4afdc-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="4afdc-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4afdc-160">Request</span></span>
<span data-ttu-id="4afdc-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4afdc-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4afdc-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="4afdc-162">Response</span></span>
<span data-ttu-id="4afdc-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4afdc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




