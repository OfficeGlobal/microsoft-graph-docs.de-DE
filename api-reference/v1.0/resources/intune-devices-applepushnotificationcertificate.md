---
title: applePushNotificationCertificate-Ressourcentyp
description: Apple Push Notification-Zertifikat.
author: tfitzmac
ms.openlocfilehash: b5be59f1a6318e07fff981fd32ec6461cb530798
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305439"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="91919-103">applePushNotificationCertificate-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="91919-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="91919-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="91919-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91919-105">Apple Push Notification-Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="91919-105">Apple push notification certificate.</span></span>
## <a name="methods"></a><span data-ttu-id="91919-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="91919-106">Methods</span></span>
|<span data-ttu-id="91919-107">Methode</span><span class="sxs-lookup"><span data-stu-id="91919-107">Method</span></span>|<span data-ttu-id="91919-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="91919-108">Return Type</span></span>|<span data-ttu-id="91919-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91919-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="91919-110">applePushNotificationCertificate abrufen</span><span class="sxs-lookup"><span data-stu-id="91919-110">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="91919-111">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="91919-111">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="91919-112">Lesen von Eigenschaften und Beziehungen des [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="91919-112">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="91919-113">applePushNotificationCertificate aktualisieren</span><span class="sxs-lookup"><span data-stu-id="91919-113">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="91919-114">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="91919-114">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="91919-115">Aktualisieren der Eigenschaften eines [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="91919-115">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="91919-116">downloadApplePushNotificationCertificateSigningRequest-Funktion</span><span class="sxs-lookup"><span data-stu-id="91919-116">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="91919-117">String</span><span class="sxs-lookup"><span data-stu-id="91919-117">String</span></span>|<span data-ttu-id="91919-118">Signieranforderung für Apple Push Notification-Zertifikat herunterladen</span><span class="sxs-lookup"><span data-stu-id="91919-118">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="91919-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="91919-119">Properties</span></span>
|<span data-ttu-id="91919-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="91919-120">Property</span></span>|<span data-ttu-id="91919-121">Typ</span><span class="sxs-lookup"><span data-stu-id="91919-121">Type</span></span>|<span data-ttu-id="91919-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91919-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91919-123">id</span><span class="sxs-lookup"><span data-stu-id="91919-123">id</span></span>|<span data-ttu-id="91919-124">String</span><span class="sxs-lookup"><span data-stu-id="91919-124">String</span></span>|<span data-ttu-id="91919-125">Eindeutiger Bezeichner für das Zertifikat</span><span class="sxs-lookup"><span data-stu-id="91919-125">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="91919-126">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="91919-126">appleIdentifier</span></span>|<span data-ttu-id="91919-127">String</span><span class="sxs-lookup"><span data-stu-id="91919-127">String</span></span>|<span data-ttu-id="91919-128">Apple-ID des Kontos, mit dem das MDM-Push-Zertifikat erstellt wurde</span><span class="sxs-lookup"><span data-stu-id="91919-128">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="91919-129">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="91919-129">topicIdentifier</span></span>|<span data-ttu-id="91919-130">String</span><span class="sxs-lookup"><span data-stu-id="91919-130">String</span></span>|<span data-ttu-id="91919-131">Thema-ID</span><span class="sxs-lookup"><span data-stu-id="91919-131">Topic Id.</span></span>|
|<span data-ttu-id="91919-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91919-132">lastModifiedDateTime</span></span>|<span data-ttu-id="91919-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91919-133">DateTimeOffset</span></span>|<span data-ttu-id="91919-134">Datum und Uhrzeit der letzten Änderung des Apple Push Notification-Zertifikats</span><span class="sxs-lookup"><span data-stu-id="91919-134">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="91919-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="91919-135">expirationDateTime</span></span>|<span data-ttu-id="91919-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91919-136">DateTimeOffset</span></span>|<span data-ttu-id="91919-137">Datum und Uhrzeit des Ablaufs des Apple Push Notification-Zertifikats</span><span class="sxs-lookup"><span data-stu-id="91919-137">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="91919-138">certificate</span><span class="sxs-lookup"><span data-stu-id="91919-138">certificate</span></span>|<span data-ttu-id="91919-139">String</span><span class="sxs-lookup"><span data-stu-id="91919-139">String</span></span>|<span data-ttu-id="91919-140">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="91919-140">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="91919-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="91919-141">Relationships</span></span>
<span data-ttu-id="91919-142">Keine</span><span class="sxs-lookup"><span data-stu-id="91919-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="91919-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="91919-143">JSON Representation</span></span>
<span data-ttu-id="91919-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="91919-144">Here is a JSON representation of the resource.</span></span>
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



