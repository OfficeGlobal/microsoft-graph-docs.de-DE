---
title: AndroidManagedStoreAppConfigurationSchema erstellen
description: Erstellen eines neuen androidManagedStoreAppConfigurationSchema-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 10def3b377d7de59fd16f491e8054129b73c9189
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979550"
---
# <a name="create-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="c7055-103">AndroidManagedStoreAppConfigurationSchema erstellen</span><span class="sxs-lookup"><span data-stu-id="c7055-103">Create androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="c7055-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c7055-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7055-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c7055-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7055-106">Erstellen eines neuen [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c7055-106">Create a new [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7055-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c7055-107">Prerequisites</span></span>
<span data-ttu-id="c7055-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7055-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7055-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c7055-110">Permission type</span></span>|<span data-ttu-id="c7055-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c7055-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7055-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c7055-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c7055-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7055-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c7055-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c7055-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7055-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7055-115">Not supported.</span></span>|
|<span data-ttu-id="c7055-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c7055-116">Application</span></span>|<span data-ttu-id="c7055-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7055-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7055-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7055-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="c7055-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c7055-119">Request headers</span></span>
|<span data-ttu-id="c7055-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c7055-120">Header</span></span>|<span data-ttu-id="c7055-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c7055-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7055-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7055-122">Authorization</span></span>|<span data-ttu-id="c7055-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c7055-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7055-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c7055-124">Accept</span></span>|<span data-ttu-id="c7055-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c7055-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7055-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c7055-126">Request body</span></span>
<span data-ttu-id="c7055-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das androidManagedStoreAppConfigurationSchema-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c7055-127">In the request body, supply a JSON representation for the androidManagedStoreAppConfigurationSchema object.</span></span>

<span data-ttu-id="c7055-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidManagedStoreAppConfigurationSchema erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c7055-128">The following table shows the properties that are required when you create the androidManagedStoreAppConfigurationSchema.</span></span>

|<span data-ttu-id="c7055-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c7055-129">Property</span></span>|<span data-ttu-id="c7055-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c7055-130">Type</span></span>|<span data-ttu-id="c7055-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7055-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7055-132">id</span><span class="sxs-lookup"><span data-stu-id="c7055-132">id</span></span>|<span data-ttu-id="c7055-133">String</span><span class="sxs-lookup"><span data-stu-id="c7055-133">String</span></span>|<span data-ttu-id="c7055-134">Schlüssel der Entität (Name des Android-Pakets der Anwendung), der das Schema entspricht</span><span class="sxs-lookup"><span data-stu-id="c7055-134">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="c7055-135">exampleJson</span><span class="sxs-lookup"><span data-stu-id="c7055-135">exampleJson</span></span>|<span data-ttu-id="c7055-136">Binär</span><span class="sxs-lookup"><span data-stu-id="c7055-136">Binary</span></span>|<span data-ttu-id="c7055-137">UTF8-codiertes Bytearray mit der diesem Schema entsprechenden JSON-Beispielzeichenfolge, das veranschaulicht, wie die Konfiguration für diese App festgelegt werden soll</span><span class="sxs-lookup"><span data-stu-id="c7055-137">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="c7055-138">schemaItems</span><span class="sxs-lookup"><span data-stu-id="c7055-138">schemaItems</span></span>|<span data-ttu-id="c7055-139">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="c7055-139">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="c7055-140">Collection von Elementen, die jeweils eine benannte Konfigurationsoption im Schema darstellen</span><span class="sxs-lookup"><span data-stu-id="c7055-140">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="c7055-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7055-141">Response</span></span>
<span data-ttu-id="c7055-142">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c7055-142">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7055-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c7055-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7055-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7055-144">Request</span></span>
<span data-ttu-id="c7055-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c7055-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas
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

### <a name="response"></a><span data-ttu-id="c7055-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7055-146">Response</span></span>
<span data-ttu-id="c7055-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c7055-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




