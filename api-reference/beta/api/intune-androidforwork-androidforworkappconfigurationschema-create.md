---
title: Erstellen von „androidForWorkAppConfigurationSchema“
description: Diese Methode erstellt ein neues Objekt des Typs androidForWorkAppConfigurationSchema.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dce0e8355ef722a3201585b79352a7458ec0ef9f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394852"
---
# <a name="create-androidforworkappconfigurationschema"></a><span data-ttu-id="16048-103">Erstellen von „androidForWorkAppConfigurationSchema“</span><span class="sxs-lookup"><span data-stu-id="16048-103">Create androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="16048-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="16048-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="16048-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="16048-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16048-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="16048-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16048-107">Diese Methode erstellt ein neues Objekt des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="16048-107">Create a new [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16048-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="16048-108">Prerequisites</span></span>
<span data-ttu-id="16048-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="16048-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="16048-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="16048-111">Permission type</span></span>|<span data-ttu-id="16048-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="16048-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16048-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="16048-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16048-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16048-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16048-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="16048-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16048-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16048-116">Not supported.</span></span>|
|<span data-ttu-id="16048-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="16048-117">Application</span></span>|<span data-ttu-id="16048-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16048-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16048-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="16048-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="16048-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="16048-120">Request headers</span></span>
|<span data-ttu-id="16048-121">Header</span><span class="sxs-lookup"><span data-stu-id="16048-121">Header</span></span>|<span data-ttu-id="16048-122">Wert</span><span class="sxs-lookup"><span data-stu-id="16048-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16048-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="16048-123">Authorization</span></span>|<span data-ttu-id="16048-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="16048-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16048-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="16048-125">Accept</span></span>|<span data-ttu-id="16048-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16048-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16048-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="16048-127">Request body</span></span>
<span data-ttu-id="16048-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „androidForWorkAppConfigurationSchema“ an.</span><span class="sxs-lookup"><span data-stu-id="16048-128">In the request body, supply a JSON representation for the androidForWorkAppConfigurationSchema object.</span></span>

<span data-ttu-id="16048-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „androidForWorkAppConfigurationSchema“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="16048-129">The following table shows the properties that are required when you create the androidForWorkAppConfigurationSchema.</span></span>

|<span data-ttu-id="16048-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="16048-130">Property</span></span>|<span data-ttu-id="16048-131">Typ</span><span class="sxs-lookup"><span data-stu-id="16048-131">Type</span></span>|<span data-ttu-id="16048-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16048-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16048-133">id</span><span class="sxs-lookup"><span data-stu-id="16048-133">id</span></span>|<span data-ttu-id="16048-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="16048-134">String</span></span>|<span data-ttu-id="16048-135">Schlüssel der Entität (Name des Android-Pakets der Anwendung), der das Schema entspricht</span><span class="sxs-lookup"><span data-stu-id="16048-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="16048-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="16048-136">exampleJson</span></span>|<span data-ttu-id="16048-137">Binär</span><span class="sxs-lookup"><span data-stu-id="16048-137">Binary</span></span>|<span data-ttu-id="16048-138">UTF8-codiertes Bytearray mit der diesem Schema entsprechenden JSON-Beispielzeichenfolge, das veranschaulicht, wie die Konfiguration für diese App festgelegt werden soll</span><span class="sxs-lookup"><span data-stu-id="16048-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="16048-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="16048-139">schemaItems</span></span>|<span data-ttu-id="16048-140">Collection von Objekten des Typs [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="16048-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="16048-141">Collection von Elementen, die jeweils eine benannte Konfigurationsoption im Schema darstellen</span><span class="sxs-lookup"><span data-stu-id="16048-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="16048-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="16048-142">Response</span></span>
<span data-ttu-id="16048-143">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="16048-143">If successful, this method returns a `201 Created` response code and a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16048-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="16048-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="16048-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="16048-145">Request</span></span>
<span data-ttu-id="16048-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="16048-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="16048-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="16048-147">Response</span></span>
<span data-ttu-id="16048-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="16048-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




