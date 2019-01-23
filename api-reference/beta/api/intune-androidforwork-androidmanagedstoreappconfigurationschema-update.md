---
title: AndroidManagedStoreAppConfigurationSchema aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidManagedStoreAppConfigurationSchema-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 326f56f497f1086ccc6e37d0171261c50dfb9c77
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410133"
---
# <a name="update-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="708f2-103">AndroidManagedStoreAppConfigurationSchema aktualisieren</span><span class="sxs-lookup"><span data-stu-id="708f2-103">Update androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="708f2-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="708f2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="708f2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="708f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="708f2-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="708f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="708f2-107">Aktualisieren Sie die Eigenschaften eines [AndroidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="708f2-107">Update the properties of a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="708f2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="708f2-108">Prerequisites</span></span>
<span data-ttu-id="708f2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="708f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="708f2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="708f2-111">Permission type</span></span>|<span data-ttu-id="708f2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="708f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="708f2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="708f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="708f2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="708f2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="708f2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="708f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="708f2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="708f2-116">Not supported.</span></span>|
|<span data-ttu-id="708f2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="708f2-117">Application</span></span>|<span data-ttu-id="708f2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="708f2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="708f2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="708f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="708f2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="708f2-120">Request headers</span></span>
|<span data-ttu-id="708f2-121">Header</span><span class="sxs-lookup"><span data-stu-id="708f2-121">Header</span></span>|<span data-ttu-id="708f2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="708f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="708f2-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="708f2-123">Authorization</span></span>|<span data-ttu-id="708f2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="708f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="708f2-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="708f2-125">Accept</span></span>|<span data-ttu-id="708f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="708f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="708f2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="708f2-127">Request body</span></span>
<span data-ttu-id="708f2-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="708f2-128">In the request body, supply a JSON representation for the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

<span data-ttu-id="708f2-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="708f2-129">The following table shows the properties that are required when you create the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span></span>

|<span data-ttu-id="708f2-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="708f2-130">Property</span></span>|<span data-ttu-id="708f2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="708f2-131">Type</span></span>|<span data-ttu-id="708f2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="708f2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="708f2-133">id</span><span class="sxs-lookup"><span data-stu-id="708f2-133">id</span></span>|<span data-ttu-id="708f2-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="708f2-134">String</span></span>|<span data-ttu-id="708f2-135">Schlüssel der Entität (Name des Android-Pakets der Anwendung), der das Schema entspricht</span><span class="sxs-lookup"><span data-stu-id="708f2-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="708f2-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="708f2-136">exampleJson</span></span>|<span data-ttu-id="708f2-137">Binär</span><span class="sxs-lookup"><span data-stu-id="708f2-137">Binary</span></span>|<span data-ttu-id="708f2-138">UTF8-codiertes Bytearray mit der diesem Schema entsprechenden JSON-Beispielzeichenfolge, das veranschaulicht, wie die Konfiguration für diese App festgelegt werden soll</span><span class="sxs-lookup"><span data-stu-id="708f2-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="708f2-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="708f2-139">schemaItems</span></span>|<span data-ttu-id="708f2-140">[AndroidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="708f2-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="708f2-141">Collection von Elementen, die jeweils eine benannte Konfigurationsoption im Schema darstellen</span><span class="sxs-lookup"><span data-stu-id="708f2-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="708f2-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="708f2-142">Response</span></span>
<span data-ttu-id="708f2-143">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="708f2-143">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="708f2-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="708f2-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="708f2-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="708f2-145">Request</span></span>
<span data-ttu-id="708f2-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="708f2-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
Content-type: application/json
Content-length: 805

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
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

### <a name="response"></a><span data-ttu-id="708f2-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="708f2-147">Response</span></span>
<span data-ttu-id="708f2-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="708f2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




