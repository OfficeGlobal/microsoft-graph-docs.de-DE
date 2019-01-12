---
title: Aktualisieren von „androidForWorkAppConfigurationSchema“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs androidForWorkAppConfigurationSchema.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 09393062a4d23622c10bf87f3fec420fc51c6650
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946518"
---
# <a name="update-androidforworkappconfigurationschema"></a><span data-ttu-id="210d3-103">Aktualisieren von „androidForWorkAppConfigurationSchema“</span><span class="sxs-lookup"><span data-stu-id="210d3-103">Update androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="210d3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="210d3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="210d3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="210d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="210d3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="210d3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="210d3-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="210d3-107">Update the properties of a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="210d3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="210d3-108">Prerequisites</span></span>
<span data-ttu-id="210d3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="210d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="210d3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="210d3-111">Permission type</span></span>|<span data-ttu-id="210d3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="210d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="210d3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="210d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="210d3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="210d3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="210d3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="210d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="210d3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="210d3-116">Not supported.</span></span>|
|<span data-ttu-id="210d3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="210d3-117">Application</span></span>|<span data-ttu-id="210d3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="210d3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="210d3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="210d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="210d3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="210d3-120">Request headers</span></span>
|<span data-ttu-id="210d3-121">Header</span><span class="sxs-lookup"><span data-stu-id="210d3-121">Header</span></span>|<span data-ttu-id="210d3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="210d3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="210d3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="210d3-123">Authorization</span></span>|<span data-ttu-id="210d3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="210d3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="210d3-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="210d3-125">Accept</span></span>|<span data-ttu-id="210d3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="210d3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="210d3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="210d3-127">Request body</span></span>
<span data-ttu-id="210d3-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) an.</span><span class="sxs-lookup"><span data-stu-id="210d3-128">In the request body, supply a JSON representation for the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

<span data-ttu-id="210d3-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="210d3-129">The following table shows the properties that are required when you create the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span></span>

|<span data-ttu-id="210d3-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="210d3-130">Property</span></span>|<span data-ttu-id="210d3-131">Typ</span><span class="sxs-lookup"><span data-stu-id="210d3-131">Type</span></span>|<span data-ttu-id="210d3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="210d3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="210d3-133">id</span><span class="sxs-lookup"><span data-stu-id="210d3-133">id</span></span>|<span data-ttu-id="210d3-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="210d3-134">String</span></span>|<span data-ttu-id="210d3-135">Schlüssel der Entität (Name des Android-Pakets der Anwendung), der das Schema entspricht</span><span class="sxs-lookup"><span data-stu-id="210d3-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="210d3-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="210d3-136">exampleJson</span></span>|<span data-ttu-id="210d3-137">Binär</span><span class="sxs-lookup"><span data-stu-id="210d3-137">Binary</span></span>|<span data-ttu-id="210d3-138">UTF8-codiertes Bytearray mit der diesem Schema entsprechenden JSON-Beispielzeichenfolge, das veranschaulicht, wie die Konfiguration für diese App festgelegt werden soll</span><span class="sxs-lookup"><span data-stu-id="210d3-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="210d3-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="210d3-139">schemaItems</span></span>|<span data-ttu-id="210d3-140">Collection von Objekten des Typs [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="210d3-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="210d3-141">Collection von Elementen, die jeweils eine benannte Konfigurationsoption im Schema darstellen</span><span class="sxs-lookup"><span data-stu-id="210d3-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="210d3-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="210d3-142">Response</span></span>
<span data-ttu-id="210d3-143">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="210d3-143">If successful, this method returns a `200 OK` response code and an updated [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="210d3-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="210d3-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="210d3-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="210d3-145">Request</span></span>
<span data-ttu-id="210d3-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="210d3-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
Content-type: application/json
Content-length: 720

{
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "integer",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="210d3-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="210d3-147">Response</span></span>
<span data-ttu-id="210d3-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="210d3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 844

{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "id": "c1230dc6-0dc6-c123-c60d-23c1c60d23c1",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "integer",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```





