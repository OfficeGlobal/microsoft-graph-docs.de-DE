---
title: Aktualisieren von „androidForWorkAppConfigurationSchema“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs androidForWorkAppConfigurationSchema.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9c3b2a2c55eb7cd8505e12462a88d98433e4f9f3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409363"
---
# <a name="update-androidforworkappconfigurationschema"></a><span data-ttu-id="c8da7-103">Aktualisieren von „androidForWorkAppConfigurationSchema“</span><span class="sxs-lookup"><span data-stu-id="c8da7-103">Update androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="c8da7-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c8da7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c8da7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c8da7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8da7-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c8da7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8da7-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="c8da7-107">Update the properties of a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8da7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c8da7-108">Prerequisites</span></span>
<span data-ttu-id="c8da7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c8da7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c8da7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c8da7-111">Permission type</span></span>|<span data-ttu-id="c8da7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c8da7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8da7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c8da7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8da7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8da7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c8da7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c8da7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8da7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8da7-116">Not supported.</span></span>|
|<span data-ttu-id="c8da7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c8da7-117">Application</span></span>|<span data-ttu-id="c8da7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8da7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8da7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8da7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="c8da7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c8da7-120">Request headers</span></span>
|<span data-ttu-id="c8da7-121">Header</span><span class="sxs-lookup"><span data-stu-id="c8da7-121">Header</span></span>|<span data-ttu-id="c8da7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c8da7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8da7-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c8da7-123">Authorization</span></span>|<span data-ttu-id="c8da7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c8da7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8da7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c8da7-125">Accept</span></span>|<span data-ttu-id="c8da7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8da7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8da7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c8da7-127">Request body</span></span>
<span data-ttu-id="c8da7-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) an.</span><span class="sxs-lookup"><span data-stu-id="c8da7-128">In the request body, supply a JSON representation for the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

<span data-ttu-id="c8da7-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="c8da7-129">The following table shows the properties that are required when you create the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span></span>

|<span data-ttu-id="c8da7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c8da7-130">Property</span></span>|<span data-ttu-id="c8da7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c8da7-131">Type</span></span>|<span data-ttu-id="c8da7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8da7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8da7-133">id</span><span class="sxs-lookup"><span data-stu-id="c8da7-133">id</span></span>|<span data-ttu-id="c8da7-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8da7-134">String</span></span>|<span data-ttu-id="c8da7-135">Schlüssel der Entität (Name des Android-Pakets der Anwendung), der das Schema entspricht</span><span class="sxs-lookup"><span data-stu-id="c8da7-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="c8da7-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="c8da7-136">exampleJson</span></span>|<span data-ttu-id="c8da7-137">Binär</span><span class="sxs-lookup"><span data-stu-id="c8da7-137">Binary</span></span>|<span data-ttu-id="c8da7-138">UTF8-codiertes Bytearray mit der diesem Schema entsprechenden JSON-Beispielzeichenfolge, das veranschaulicht, wie die Konfiguration für diese App festgelegt werden soll</span><span class="sxs-lookup"><span data-stu-id="c8da7-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="c8da7-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="c8da7-139">schemaItems</span></span>|<span data-ttu-id="c8da7-140">Collection von Objekten des Typs [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="c8da7-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="c8da7-141">Collection von Elementen, die jeweils eine benannte Konfigurationsoption im Schema darstellen</span><span class="sxs-lookup"><span data-stu-id="c8da7-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="c8da7-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8da7-142">Response</span></span>
<span data-ttu-id="c8da7-143">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c8da7-143">If successful, this method returns a `200 OK` response code and an updated [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8da7-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c8da7-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8da7-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8da7-145">Request</span></span>
<span data-ttu-id="c8da7-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c8da7-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
Content-type: application/json
Content-length: 795

{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
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

### <a name="response"></a><span data-ttu-id="c8da7-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8da7-147">Response</span></span>
<span data-ttu-id="c8da7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8da7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




