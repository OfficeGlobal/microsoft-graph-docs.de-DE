---
title: Erstellen von „androidForWorkAppConfigurationSchema“
description: Diese Methode erstellt ein neues Objekt des Typs androidForWorkAppConfigurationSchema.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dfbd2d8a1c6cefbde7ea8f14e640aa4ef5a0a5fb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148531"
---
# <a name="create-androidforworkappconfigurationschema"></a><span data-ttu-id="1f07b-103">Erstellen von „androidForWorkAppConfigurationSchema“</span><span class="sxs-lookup"><span data-stu-id="1f07b-103">Create androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="1f07b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1f07b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f07b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1f07b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f07b-106">Diese Methode erstellt ein neues Objekt des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="1f07b-106">Create a new [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f07b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1f07b-107">Prerequisites</span></span>
<span data-ttu-id="1f07b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1f07b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1f07b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1f07b-110">Permission type</span></span>|<span data-ttu-id="1f07b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1f07b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f07b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1f07b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f07b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f07b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1f07b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1f07b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f07b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f07b-115">Not supported.</span></span>|
|<span data-ttu-id="1f07b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1f07b-116">Application</span></span>|<span data-ttu-id="1f07b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f07b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f07b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f07b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="1f07b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1f07b-119">Request headers</span></span>
|<span data-ttu-id="1f07b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1f07b-120">Header</span></span>|<span data-ttu-id="1f07b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1f07b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f07b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f07b-122">Authorization</span></span>|<span data-ttu-id="1f07b-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1f07b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f07b-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1f07b-124">Accept</span></span>|<span data-ttu-id="1f07b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1f07b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f07b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1f07b-126">Request body</span></span>
<span data-ttu-id="1f07b-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „androidForWorkAppConfigurationSchema“ an.</span><span class="sxs-lookup"><span data-stu-id="1f07b-127">In the request body, supply a JSON representation for the androidForWorkAppConfigurationSchema object.</span></span>

<span data-ttu-id="1f07b-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „androidForWorkAppConfigurationSchema“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="1f07b-128">The following table shows the properties that are required when you create the androidForWorkAppConfigurationSchema.</span></span>

|<span data-ttu-id="1f07b-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1f07b-129">Property</span></span>|<span data-ttu-id="1f07b-130">Typ</span><span class="sxs-lookup"><span data-stu-id="1f07b-130">Type</span></span>|<span data-ttu-id="1f07b-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f07b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f07b-132">id</span><span class="sxs-lookup"><span data-stu-id="1f07b-132">id</span></span>|<span data-ttu-id="1f07b-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1f07b-133">String</span></span>|<span data-ttu-id="1f07b-134">Schlüssel der Entität (Name des Android-Pakets der Anwendung), der das Schema entspricht</span><span class="sxs-lookup"><span data-stu-id="1f07b-134">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="1f07b-135">exampleJson</span><span class="sxs-lookup"><span data-stu-id="1f07b-135">exampleJson</span></span>|<span data-ttu-id="1f07b-136">Binär</span><span class="sxs-lookup"><span data-stu-id="1f07b-136">Binary</span></span>|<span data-ttu-id="1f07b-137">UTF8-codiertes Bytearray mit der diesem Schema entsprechenden JSON-Beispielzeichenfolge, das veranschaulicht, wie die Konfiguration für diese App festgelegt werden soll</span><span class="sxs-lookup"><span data-stu-id="1f07b-137">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="1f07b-138">schemaItems</span><span class="sxs-lookup"><span data-stu-id="1f07b-138">schemaItems</span></span>|<span data-ttu-id="1f07b-139">Collection von Objekten des Typs [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="1f07b-139">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="1f07b-140">Collection von Elementen, die jeweils eine benannte Konfigurationsoption im Schema darstellen</span><span class="sxs-lookup"><span data-stu-id="1f07b-140">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="1f07b-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f07b-141">Response</span></span>
<span data-ttu-id="1f07b-142">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1f07b-142">If successful, this method returns a `201 Created` response code and a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f07b-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1f07b-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f07b-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f07b-144">Request</span></span>
<span data-ttu-id="1f07b-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1f07b-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas
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

### <a name="response"></a><span data-ttu-id="1f07b-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f07b-146">Response</span></span>
<span data-ttu-id="1f07b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f07b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




