---
title: Aktualisieren von „androidForWorkAppConfigurationSchema“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs androidForWorkAppConfigurationSchema.
author: tfitzmac
ms.openlocfilehash: ba4050ce741e1fdcfd3158e7f9e9d9e47f422882
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333901"
---
# <a name="update-androidforworkappconfigurationschema"></a><span data-ttu-id="b885b-103">Aktualisieren von „androidForWorkAppConfigurationSchema“</span><span class="sxs-lookup"><span data-stu-id="b885b-103">Update androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="b885b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b885b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b885b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b885b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b885b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b885b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b885b-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="b885b-107">Update the properties of a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b885b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b885b-108">Prerequisites</span></span>
<span data-ttu-id="b885b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b885b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b885b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b885b-111">Permission type</span></span>|<span data-ttu-id="b885b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b885b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b885b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b885b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b885b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b885b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b885b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b885b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b885b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b885b-116">Not supported.</span></span>|
|<span data-ttu-id="b885b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b885b-117">Application</span></span>|<span data-ttu-id="b885b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b885b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b885b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b885b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="b885b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b885b-120">Request headers</span></span>
|<span data-ttu-id="b885b-121">Header</span><span class="sxs-lookup"><span data-stu-id="b885b-121">Header</span></span>|<span data-ttu-id="b885b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b885b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b885b-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b885b-123">Authorization</span></span>|<span data-ttu-id="b885b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b885b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b885b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b885b-125">Accept</span></span>|<span data-ttu-id="b885b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b885b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b885b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b885b-127">Request body</span></span>
<span data-ttu-id="b885b-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) an.</span><span class="sxs-lookup"><span data-stu-id="b885b-128">In the request body, supply a JSON representation for the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

<span data-ttu-id="b885b-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="b885b-129">The following table shows the properties that are required when you create the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span></span>

|<span data-ttu-id="b885b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b885b-130">Property</span></span>|<span data-ttu-id="b885b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b885b-131">Type</span></span>|<span data-ttu-id="b885b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b885b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b885b-133">id</span><span class="sxs-lookup"><span data-stu-id="b885b-133">id</span></span>|<span data-ttu-id="b885b-134">String</span><span class="sxs-lookup"><span data-stu-id="b885b-134">String</span></span>|<span data-ttu-id="b885b-135">Schlüssel der Entität (Name des Android-Pakets der Anwendung), der das Schema entspricht</span><span class="sxs-lookup"><span data-stu-id="b885b-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="b885b-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="b885b-136">exampleJson</span></span>|<span data-ttu-id="b885b-137">Binär</span><span class="sxs-lookup"><span data-stu-id="b885b-137">Binary</span></span>|<span data-ttu-id="b885b-138">UTF8-codiertes Bytearray mit der diesem Schema entsprechenden JSON-Beispielzeichenfolge, das veranschaulicht, wie die Konfiguration für diese App festgelegt werden soll</span><span class="sxs-lookup"><span data-stu-id="b885b-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="b885b-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="b885b-139">schemaItems</span></span>|<span data-ttu-id="b885b-140">Collection von Objekten des Typs [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="b885b-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="b885b-141">Collection von Elementen, die jeweils eine benannte Konfigurationsoption im Schema darstellen</span><span class="sxs-lookup"><span data-stu-id="b885b-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="b885b-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="b885b-142">Response</span></span>
<span data-ttu-id="b885b-143">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b885b-143">If successful, this method returns a `200 OK` response code and an updated [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b885b-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b885b-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="b885b-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b885b-145">Request</span></span>
<span data-ttu-id="b885b-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b885b-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b885b-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="b885b-147">Response</span></span>
<span data-ttu-id="b885b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b885b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





