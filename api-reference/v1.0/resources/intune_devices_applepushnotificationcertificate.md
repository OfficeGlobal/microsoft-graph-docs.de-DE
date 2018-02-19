# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="085e0-101">applePushNotificationCertificate-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="085e0-101">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="085e0-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="085e0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="085e0-103">Apple Push Notification-Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="085e0-103">Apple push notification certificate.</span></span>
## <a name="methods"></a><span data-ttu-id="085e0-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="085e0-104">Methods</span></span>
|<span data-ttu-id="085e0-105">Methode</span><span class="sxs-lookup"><span data-stu-id="085e0-105">Method</span></span>|<span data-ttu-id="085e0-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="085e0-106">Return Type</span></span>|<span data-ttu-id="085e0-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="085e0-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="085e0-108">applePushNotificationCertificate abrufen</span><span class="sxs-lookup"><span data-stu-id="085e0-108">Get applePushNotificationCertificate</span></span>](../api/intune_devices_applepushnotificationcertificate_get.md)|[<span data-ttu-id="085e0-109">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="085e0-109">applePushNotificationCertificate</span></span>](../resources/intune_devices_applepushnotificationcertificate.md)|<span data-ttu-id="085e0-110">Lesen von Eigenschaften und Beziehungen des [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="085e0-110">Read properties and relationships of [plannerPlanDetails](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="085e0-111">applePushNotificationCertificate aktualisieren</span><span class="sxs-lookup"><span data-stu-id="085e0-111">Update applePushNotificationCertificate</span></span>](../api/intune_devices_applepushnotificationcertificate_update.md)|[<span data-ttu-id="085e0-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="085e0-112">applePushNotificationCertificate</span></span>](../resources/intune_devices_applepushnotificationcertificate.md)|<span data-ttu-id="085e0-113">Aktualisieren der Eigenschaften eines [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="085e0-113">Update the properties of a [calendar](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="085e0-114">downloadApplePushNotificationCertificateSigningRequest-Funktion</span><span class="sxs-lookup"><span data-stu-id="085e0-114">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune_devices_applepushnotificationcertificate_downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="085e0-115">String</span><span class="sxs-lookup"><span data-stu-id="085e0-115">String</span></span>|<span data-ttu-id="085e0-116">Signieranforderung für Apple Push Notification-Zertifikat herunterladen</span><span class="sxs-lookup"><span data-stu-id="085e0-116">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="085e0-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="085e0-117">Properties</span></span>
|<span data-ttu-id="085e0-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="085e0-118">Property</span></span>|<span data-ttu-id="085e0-119">Typ</span><span class="sxs-lookup"><span data-stu-id="085e0-119">Type</span></span>|<span data-ttu-id="085e0-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="085e0-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="085e0-121">id</span><span class="sxs-lookup"><span data-stu-id="085e0-121">id</span></span>|<span data-ttu-id="085e0-122">String</span><span class="sxs-lookup"><span data-stu-id="085e0-122">String</span></span>|<span data-ttu-id="085e0-123">Eindeutiger Bezeichner für das Zertifikat</span><span class="sxs-lookup"><span data-stu-id="085e0-123">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="085e0-124">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="085e0-124">appleIdentifier</span></span>|<span data-ttu-id="085e0-125">String</span><span class="sxs-lookup"><span data-stu-id="085e0-125">String</span></span>|<span data-ttu-id="085e0-126">Apple-ID des Kontos, mit dem das MDM-Push-Zertifikat erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="085e0-126">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="085e0-127">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="085e0-127">topicIdentifier</span></span>|<span data-ttu-id="085e0-128">String</span><span class="sxs-lookup"><span data-stu-id="085e0-128">String</span></span>|<span data-ttu-id="085e0-129">Thema-ID</span><span class="sxs-lookup"><span data-stu-id="085e0-129">Topic Id.</span></span>|
|<span data-ttu-id="085e0-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="085e0-130">lastModifiedDateTime</span></span>|<span data-ttu-id="085e0-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="085e0-131">DateTimeOffset</span></span>|<span data-ttu-id="085e0-132">Datum und Uhrzeit der letzten Änderung des Apple Push Notification-Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="085e0-132">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="085e0-133">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="085e0-133">expirationDateTime</span></span>|<span data-ttu-id="085e0-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="085e0-134">DateTimeOffset</span></span>|<span data-ttu-id="085e0-135">Ablaufdatum und -Uhrzeit für das Apple Push Notification-Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="085e0-135">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="085e0-136">certificate</span><span class="sxs-lookup"><span data-stu-id="085e0-136">ACS, certificate</span></span>|<span data-ttu-id="085e0-137">String</span><span class="sxs-lookup"><span data-stu-id="085e0-137">String</span></span>|<span data-ttu-id="085e0-138">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="085e0-138">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="085e0-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="085e0-139">Relationships</span></span>
<span data-ttu-id="085e0-140">Keine</span><span class="sxs-lookup"><span data-stu-id="085e0-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="085e0-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="085e0-141">JSON Representation</span></span>
<span data-ttu-id="085e0-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="085e0-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificate": "String"
}
```



