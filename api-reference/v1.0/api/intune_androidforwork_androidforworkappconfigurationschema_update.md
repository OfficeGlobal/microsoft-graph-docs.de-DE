# <a name="update-androidforworkappconfigurationschema"></a><span data-ttu-id="a5aa6-101">Aktualisieren von „androidForWorkAppConfigurationSchema“</span><span class="sxs-lookup"><span data-stu-id="a5aa6-101">Update androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="a5aa6-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a5aa6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5aa6-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="a5aa6-103">Update the properties of a [calendar](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a5aa6-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a5aa6-104">Prerequisites</span></span>
<span data-ttu-id="a5aa6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a5aa6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a5aa6-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a5aa6-107">Permission type</span></span>|<span data-ttu-id="a5aa6-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a5aa6-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5aa6-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a5aa6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a5aa6-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5aa6-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a5aa6-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a5aa6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5aa6-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a5aa6-112">Not supported.</span></span>|
|<span data-ttu-id="a5aa6-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a5aa6-113">Application</span></span>|<span data-ttu-id="a5aa6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a5aa6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5aa6-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5aa6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="a5aa6-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a5aa6-116">Request headers</span></span>
|<span data-ttu-id="a5aa6-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a5aa6-117">Header</span></span>|<span data-ttu-id="a5aa6-118">Wert</span><span class="sxs-lookup"><span data-stu-id="a5aa6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5aa6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5aa6-119">Authorization</span></span>|<span data-ttu-id="a5aa6-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a5aa6-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a5aa6-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a5aa6-121">Accept</span></span>|<span data-ttu-id="a5aa6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a5aa6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5aa6-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a5aa6-123">Request body</span></span>
<span data-ttu-id="a5aa6-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) an.</span><span class="sxs-lookup"><span data-stu-id="a5aa6-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object.</span></span>

<span data-ttu-id="a5aa6-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="a5aa6-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="a5aa6-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a5aa6-126">Property</span></span>|<span data-ttu-id="a5aa6-127">Typ</span><span class="sxs-lookup"><span data-stu-id="a5aa6-127">Type</span></span>|<span data-ttu-id="a5aa6-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5aa6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5aa6-129">id</span><span class="sxs-lookup"><span data-stu-id="a5aa6-129">id</span></span>|<span data-ttu-id="a5aa6-130">String</span><span class="sxs-lookup"><span data-stu-id="a5aa6-130">String</span></span>|<span data-ttu-id="a5aa6-131">Schlüssel der Entität (Name des Android-Pakets der Anwendung), der das Schema entspricht</span><span class="sxs-lookup"><span data-stu-id="a5aa6-131">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="a5aa6-132">exampleJson</span><span class="sxs-lookup"><span data-stu-id="a5aa6-132">exampleJson</span></span>|<span data-ttu-id="a5aa6-133">Binary</span><span class="sxs-lookup"><span data-stu-id="a5aa6-133">Binary</span></span>|<span data-ttu-id="a5aa6-134">UTF8-codiertes Bytearray mit der diesem Schema entsprechenden JSON-Beispielzeichenfolge, das veranschaulicht, wie die Konfiguration für diese App festgelegt werden soll</span><span class="sxs-lookup"><span data-stu-id="a5aa6-134">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="a5aa6-135">schemaItems</span><span class="sxs-lookup"><span data-stu-id="a5aa6-135">schemaItems</span></span>|<span data-ttu-id="a5aa6-136">Collection von Objekten des Typs [androidForWorkAppConfigurationSchemaItem](../resources/intune_androidforwork_androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="a5aa6-136">[androidForWorkAppConfigurationSchemaItem](../resources/intune_androidforwork_androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="a5aa6-137">Collection von Elementen, die jeweils eine benannte Konfigurationsoption im Schema darstellen</span><span class="sxs-lookup"><span data-stu-id="a5aa6-137">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="a5aa6-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5aa6-138">Response</span></span>
<span data-ttu-id="a5aa6-139">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a5aa6-139">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5aa6-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a5aa6-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="a5aa6-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5aa6-141">Request</span></span>
<span data-ttu-id="a5aa6-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a5aa6-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
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

### <a name="response"></a><span data-ttu-id="a5aa6-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5aa6-143">Response</span></span>
<span data-ttu-id="a5aa6-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a5aa6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



