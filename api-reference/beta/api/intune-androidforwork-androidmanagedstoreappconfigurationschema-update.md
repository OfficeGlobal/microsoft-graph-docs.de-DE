---
title: AndroidManagedStoreAppConfigurationSchema aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidManagedStoreAppConfigurationSchema-Objekts.
ms.openlocfilehash: e762a909db958b62d1128ff1dae178181124990c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059283"
---
# <a name="update-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="73bb5-103">AndroidManagedStoreAppConfigurationSchema aktualisieren</span><span class="sxs-lookup"><span data-stu-id="73bb5-103">Update androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="73bb5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="73bb5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73bb5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="73bb5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73bb5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="73bb5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73bb5-107">Aktualisieren Sie die Eigenschaften eines [AndroidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="73bb5-107">Update the properties of a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="73bb5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="73bb5-108">Prerequisites</span></span>
<span data-ttu-id="73bb5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73bb5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73bb5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="73bb5-111">Permission type</span></span>|<span data-ttu-id="73bb5-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="73bb5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73bb5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="73bb5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="73bb5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73bb5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="73bb5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="73bb5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73bb5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73bb5-116">Not supported.</span></span>|
|<span data-ttu-id="73bb5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="73bb5-117">Application</span></span>|<span data-ttu-id="73bb5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73bb5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73bb5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="73bb5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="73bb5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="73bb5-120">Request headers</span></span>
|<span data-ttu-id="73bb5-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="73bb5-121">Header</span></span>|<span data-ttu-id="73bb5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="73bb5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73bb5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="73bb5-123">Authorization</span></span>|<span data-ttu-id="73bb5-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="73bb5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73bb5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="73bb5-125">Accept</span></span>|<span data-ttu-id="73bb5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="73bb5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73bb5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="73bb5-127">Request body</span></span>
<span data-ttu-id="73bb5-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="73bb5-128">In the request body, supply a JSON representation for the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

<span data-ttu-id="73bb5-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="73bb5-129">The following table shows the properties that are required when you create the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span></span>

|<span data-ttu-id="73bb5-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="73bb5-130">Property</span></span>|<span data-ttu-id="73bb5-131">Typ</span><span class="sxs-lookup"><span data-stu-id="73bb5-131">Type</span></span>|<span data-ttu-id="73bb5-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73bb5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73bb5-133">id</span><span class="sxs-lookup"><span data-stu-id="73bb5-133">id</span></span>|<span data-ttu-id="73bb5-134">String</span><span class="sxs-lookup"><span data-stu-id="73bb5-134">String</span></span>|<span data-ttu-id="73bb5-135">Schlüssel der Entität (Name des Android-Pakets der Anwendung), der das Schema entspricht</span><span class="sxs-lookup"><span data-stu-id="73bb5-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="73bb5-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="73bb5-136">exampleJson</span></span>|<span data-ttu-id="73bb5-137">Binär</span><span class="sxs-lookup"><span data-stu-id="73bb5-137">Binary</span></span>|<span data-ttu-id="73bb5-138">UTF8-codiertes Bytearray mit der diesem Schema entsprechenden JSON-Beispielzeichenfolge, das veranschaulicht, wie die Konfiguration für diese App festgelegt werden soll</span><span class="sxs-lookup"><span data-stu-id="73bb5-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="73bb5-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="73bb5-139">schemaItems</span></span>|<span data-ttu-id="73bb5-140">[AndroidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="73bb5-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="73bb5-141">Collection von Elementen, die jeweils eine benannte Konfigurationsoption im Schema darstellen</span><span class="sxs-lookup"><span data-stu-id="73bb5-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="73bb5-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="73bb5-142">Response</span></span>
<span data-ttu-id="73bb5-143">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="73bb5-143">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73bb5-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="73bb5-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="73bb5-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="73bb5-145">Request</span></span>
<span data-ttu-id="73bb5-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="73bb5-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
Content-type: application/json
Content-length: 725

{
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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

### <a name="response"></a><span data-ttu-id="73bb5-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="73bb5-147">Response</span></span>
<span data-ttu-id="73bb5-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73bb5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 854

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
  "id": "db86c34a-c34a-db86-4ac3-86db4ac386db",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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





