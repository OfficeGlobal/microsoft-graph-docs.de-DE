---
title: Benachrichtigung Ressourcentyp
description: 'Stellt eine Benachrichtigung, die von einem app-Server veröffentlicht wird, die einen angegebenen Benutzer abzielt. Die Benachrichtigung in Microsoft Graph gespeichert ist und auf anderes Gerät Endpunkte Besitz des Benutzers verteilt ist. '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: af130c9806511b0afbdaedb602790c7c40d3ca2e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509259"
---
# <a name="notification-resource-type"></a><span data-ttu-id="07a7e-104">Benachrichtigung Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="07a7e-104">notification resource type</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07a7e-105">Stellt eine Benachrichtigung, die von einem app-Server veröffentlicht wird, die einen angegebenen Benutzer abzielt.</span><span class="sxs-lookup"><span data-stu-id="07a7e-105">Represents a notification that is published by an app server that targets a specified user.</span></span> <span data-ttu-id="07a7e-106">Die Benachrichtigung in Microsoft Graph gespeichert ist und auf anderes Gerät Endpunkte Besitz des Benutzers verteilt ist.</span><span class="sxs-lookup"><span data-stu-id="07a7e-106">The notification is stored in Microsoft Graph and is distributed to different device endpoints owned by the user.</span></span> 

<span data-ttu-id="07a7e-107">Eine Benachrichtigung kann es sich um eine visuelle Benachrichtigung Nutzlast sein, die vom Betriebssystem, einschließlich Windows, iOS und Android-Plattformen interpretiert werden können.</span><span class="sxs-lookup"><span data-stu-id="07a7e-107">A notification can be a visual notification payload that can be interpreted by the operating system, including Windows, Android, and iOS platforms.</span></span> <span data-ttu-id="07a7e-108">Es kann auch sein, Datennutzlast, die den zugestellt und behandelt wurde von app-Clients, die bestimmen, klicken Sie dann die entsprechende Benutzer erleben auf jedem Gerät – in der Regel eine visuelle Benachrichtigung Benutzeroberfläche, die den Inhalt in der ursprünglichen Datennutzlast entspricht, die generiert wird lokal.</span><span class="sxs-lookup"><span data-stu-id="07a7e-108">It can also be a data payload that's delivered to and handled by app clients, which then determine the corresponding user experience on each device – usually, a visual notification UI that corresponds to the content in the original data payload that's generated locally.</span></span> 

<span data-ttu-id="07a7e-109">Wenn ein Benutzer auf eine visuelle Benachrichtigung fungiert, kann der app-Client mithilfe der clientseitigen Project ROM SDK klicken Sie dann verwenden, um den Status der entsprechende Benachrichtigung, beispielsweise durch eine Benachrichtigung kennzeichnen, wie Sie ausgeblendete feed in Microsoft Graph - aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="07a7e-109">When a user acts on a visual notification, the app client can then use client-side Project Rome SDK to update the state of the corresponding notification feed in Microsoft Graph - for example, by marking a notification as dismissed.</span></span> <span data-ttu-id="07a7e-110">Das Update wird dann an alle Endpunkte andere app-Client verteilt werden, und die Clients die Änderung entsprechend behandelt, beispielsweise durch Schließen die Benachrichtigung, um zu verhindern, dass den Benutzer redundanten Informationen einsehen können.</span><span class="sxs-lookup"><span data-stu-id="07a7e-110">The update will then be distributed to all other app client endpoints, and the clients handle the change accordingly, for example by dismissing the notification to prevent the user from seeing redundant information.</span></span> <span data-ttu-id="07a7e-111">App-Clients können dieselbe Ressource Benachrichtigung zugreifen, zu einem späteren Zeitpunkt, bevor sie abläuft (auch nach es als geschlossen markiert ist), als Benachrichtigungsverlauf, über die [Project-ROM-SDK](https://github.com/Microsoft/project-rome).</span><span class="sxs-lookup"><span data-stu-id="07a7e-111">App clients can access the same notification resource at a later time before it expires (even after it is marked as dismissed), as notification history, via the [Project Rome SDK](https://github.com/Microsoft/project-rome).</span></span> 

## <a name="methods"></a><span data-ttu-id="07a7e-112">Methoden</span><span class="sxs-lookup"><span data-stu-id="07a7e-112">Methods</span></span>
|<span data-ttu-id="07a7e-113">Methode</span><span class="sxs-lookup"><span data-stu-id="07a7e-113">Method</span></span> | <span data-ttu-id="07a7e-114">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="07a7e-114">Return Type</span></span> | <span data-ttu-id="07a7e-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07a7e-115">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="07a7e-116">Benachrichtigung erstellen</span><span class="sxs-lookup"><span data-stu-id="07a7e-116">Create notification</span></span>](../api/projectrome-notification-post.md) | <span data-ttu-id="07a7e-117">Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="07a7e-117">[notification](projectrome-notification.md)</span></span> |<span data-ttu-id="07a7e-118">Erstellen Sie und senden Sie eine Benachrichtigung.</span><span class="sxs-lookup"><span data-stu-id="07a7e-118">Create and send a notification.</span></span> |

## <a name="properties"></a><span data-ttu-id="07a7e-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="07a7e-119">Properties</span></span>
|<span data-ttu-id="07a7e-120">Name</span><span class="sxs-lookup"><span data-stu-id="07a7e-120">Name</span></span> | <span data-ttu-id="07a7e-121">Typ</span><span class="sxs-lookup"><span data-stu-id="07a7e-121">Type</span></span> | <span data-ttu-id="07a7e-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07a7e-122">Description</span></span>|
|:----|:-----|:-----------|
| <span data-ttu-id="07a7e-123">targetHostName</span><span class="sxs-lookup"><span data-stu-id="07a7e-123">targetHostName</span></span> | <span data-ttu-id="07a7e-124">String</span><span class="sxs-lookup"><span data-stu-id="07a7e-124">String</span></span> | <span data-ttu-id="07a7e-125">Stellt den Hostnamen der app auf die der aufrufende Dienst möchte die Benachrichtigung für den angegebenen Benutzer buchen.</span><span class="sxs-lookup"><span data-stu-id="07a7e-125">Represents the host name of the app to which the calling service wants to post the notification, for the given user.</span></span> |
| <span data-ttu-id="07a7e-126">appNotificationId</span><span class="sxs-lookup"><span data-stu-id="07a7e-126">appNotificationId</span></span> | <span data-ttu-id="07a7e-127">String</span><span class="sxs-lookup"><span data-stu-id="07a7e-127">String</span></span> | <span data-ttu-id="07a7e-128">Die eindeutige Id, die von der app-Server eine Benachrichtigung, die verwendet wird, zu identifizieren, und statten Sie eine einzelne Benachrichtigung festgelegt.</span><span class="sxs-lookup"><span data-stu-id="07a7e-128">The unique id set by the app server of a notification that is used to identify and target an individual notification.</span></span> |
| <span data-ttu-id="07a7e-129">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="07a7e-129">expirationDateTime</span></span> | <span data-ttu-id="07a7e-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07a7e-130">DateTimeOffset</span></span> | <span data-ttu-id="07a7e-131">Legt eine Ablaufzeit UTC auf eine Benachrichtigung Benutzer - Zeit wird oben, die Benachrichtigung wird aus der Microsoft Graph Benachrichtigung feed Store vollständig entfernt und ist nicht mehr Teil der Benachrichtigungsverlauf.</span><span class="sxs-lookup"><span data-stu-id="07a7e-131">Sets a UTC expiration time on a user notification - when time is up, the notification is removed from the Microsoft Graph notification feed store completely and is no longer part of notification history.</span></span> <span data-ttu-id="07a7e-132">Max-Wert beträgt 30 Tage.</span><span class="sxs-lookup"><span data-stu-id="07a7e-132">Max value is 30 days.</span></span> |
| <span data-ttu-id="07a7e-133">payload</span><span class="sxs-lookup"><span data-stu-id="07a7e-133">payload</span></span> | <span data-ttu-id="07a7e-134">Edm.ComplexType JSON-Objekt</span><span class="sxs-lookup"><span data-stu-id="07a7e-134">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="07a7e-135">Dies ist der Dateninhalt des Benachrichtigung Rohdaten oder visual-Benutzer, die Identitätsdaten durch den Empfang dieser Benachrichtigung app-Client und übermittelt werden.</span><span class="sxs-lookup"><span data-stu-id="07a7e-135">This is the data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> |
| <span data-ttu-id="07a7e-136">payload.rawContent</span><span class="sxs-lookup"><span data-stu-id="07a7e-136">payload.rawContent</span></span> | <span data-ttu-id="07a7e-137">String</span><span class="sxs-lookup"><span data-stu-id="07a7e-137">String</span></span> | <span data-ttu-id="07a7e-138">Der Inhalt der Benachrichtigung über eine unformatierte User-Benachrichtigung, die an übermittelt und vom Empfang dieser Benachrichtigung app-Client verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="07a7e-138">The notification content of a raw user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> <span data-ttu-id="07a7e-139">Mindestens eine der Payload.RawContent und Payload.VisualContent muss für eine Benachrichtigung POST-Anforderung gültig sein.</span><span class="sxs-lookup"><span data-stu-id="07a7e-139">At least one of Payload.RawContent and Payload.VisualContent needs to be valid for a POST Notification request.</span></span> |
| <span data-ttu-id="07a7e-140">Payload.Visual</span><span class="sxs-lookup"><span data-stu-id="07a7e-140">payload.visual</span></span> | <span data-ttu-id="07a7e-141">Edm.ComplexType JSON-Objekt</span><span class="sxs-lookup"><span data-stu-id="07a7e-141">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="07a7e-142">Der visuelle Inhalt einer Benachrichtigung visuelle Benutzer, die von der Benachrichtigung-Plattform auf jedes mobile Plattform genutzt werden und für die Benutzer gerendert.</span><span class="sxs-lookup"><span data-stu-id="07a7e-142">The visual content of a visual user notification, which will be consumed by the notification platform on each mobile platform and rendered for the users.</span></span> <span data-ttu-id="07a7e-143">Mindestens eine der Inhalte und VisualContent muss für eine Benachrichtigung POST-Anforderung gültig sein.</span><span class="sxs-lookup"><span data-stu-id="07a7e-143">At least one of Content and VisualContent needs to be valid for a POST Notification request.</span></span> |
| <span data-ttu-id="07a7e-144">Payload.Visual.Title</span><span class="sxs-lookup"><span data-stu-id="07a7e-144">payload.visual.title</span></span> | <span data-ttu-id="07a7e-145">String</span><span class="sxs-lookup"><span data-stu-id="07a7e-145">String</span></span> | <span data-ttu-id="07a7e-146">Der Titel einer Benachrichtigung visuelle Benutzer.</span><span class="sxs-lookup"><span data-stu-id="07a7e-146">The title of a visual user notification.</span></span> <span data-ttu-id="07a7e-147">Titel oder Textkörper benötigen.</span><span class="sxs-lookup"><span data-stu-id="07a7e-147">Must have either title or body.</span></span> |
| <span data-ttu-id="07a7e-148">Payload.Visual.Body</span><span class="sxs-lookup"><span data-stu-id="07a7e-148">payload.visual.body</span></span> | <span data-ttu-id="07a7e-149">String</span><span class="sxs-lookup"><span data-stu-id="07a7e-149">String</span></span> | <span data-ttu-id="07a7e-150">Der Text einer Benachrichtigung visuelle Benutzer.</span><span class="sxs-lookup"><span data-stu-id="07a7e-150">The body of a visual user notification.</span></span> <span data-ttu-id="07a7e-151">Titel oder Textkörper benötigen.</span><span class="sxs-lookup"><span data-stu-id="07a7e-151">Must have either title or body.</span></span> |
| <span data-ttu-id="07a7e-152">displayTimeToLive</span><span class="sxs-lookup"><span data-stu-id="07a7e-152">displayTimeToLive</span></span> | <span data-ttu-id="07a7e-153">Int</span><span class="sxs-lookup"><span data-stu-id="07a7e-153">Int</span></span> | <span data-ttu-id="07a7e-154">Legt fest, wie lange (in Sekunden) ist, wird dieser Benachrichtigungsinhalt in jede Plattform Benachrichtigung Viewer bleiben.</span><span class="sxs-lookup"><span data-stu-id="07a7e-154">Sets how long (in seconds) this notification content will stay in each platform’s notification viewer.</span></span> <span data-ttu-id="07a7e-155">Angenommen, wenn die Benachrichtigung an ein Windows-Gerät übermittelt werden, ist der Wert dieser Eigenschaft an ToastNotification.ExpirationTime, übergeben die bestimmt, wie lange die Toast-Benachrichtigung des Benutzers Windows-Aktion Center bleibt.</span><span class="sxs-lookup"><span data-stu-id="07a7e-155">For example, when the notification is delivered to a Windows device, the value of this property is passed on to ToastNotification.ExpirationTime, which determines how long the toast notification will stay in the user’s Windows Action Center.</span></span> |
| <span data-ttu-id="07a7e-156">Priorität</span><span class="sxs-lookup"><span data-stu-id="07a7e-156">priority</span></span> | <span data-ttu-id="07a7e-157">EnumType</span><span class="sxs-lookup"><span data-stu-id="07a7e-157">EnumType</span></span> | <span data-ttu-id="07a7e-158">Gibt die Priorität einer Benachrichtigung unformatierte User.</span><span class="sxs-lookup"><span data-stu-id="07a7e-158">Indicates the priority of a raw user notification.</span></span> <span data-ttu-id="07a7e-159">Visual Benachrichtigungen werden standardmäßig mit hoher Priorität gesendet.</span><span class="sxs-lookup"><span data-stu-id="07a7e-159">Visual notifications are sent with high priority by default.</span></span> <span data-ttu-id="07a7e-160">Gültige Werte sind hohen und niedrigen.</span><span class="sxs-lookup"><span data-stu-id="07a7e-160">Valid values are High and Low.</span></span> |
| <span data-ttu-id="07a7e-161">GroupName</span><span class="sxs-lookup"><span data-stu-id="07a7e-161">groupName</span></span> | <span data-ttu-id="07a7e-162">String</span><span class="sxs-lookup"><span data-stu-id="07a7e-162">String</span></span> | <span data-ttu-id="07a7e-163">Der Name der Gruppe, zu der diese Benachrichtigung gehört.</span><span class="sxs-lookup"><span data-stu-id="07a7e-163">The name of the group that this notification belongs to.</span></span> <span data-ttu-id="07a7e-164">Es wird vom Entwickler zum Gruppieren von Benachrichtigungen festgelegt.</span><span class="sxs-lookup"><span data-stu-id="07a7e-164">It is set by the developer for the purpose of grouping notifications together.</span></span> |
| <span data-ttu-id="07a7e-165">targetPolicy</span><span class="sxs-lookup"><span data-stu-id="07a7e-165">targetPolicy</span></span> | <span data-ttu-id="07a7e-166">Edm.ComplexType JSON-Objekt</span><span class="sxs-lookup"><span data-stu-id="07a7e-166">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="07a7e-167">Richtlinie Zielobjekt behandelt Notification Delivery Richtlinie auf zwei verschiedenen Ebenen - Endpunkttypen (Windows, iOS und Android), die verwendet werden soll, und bestimmten Endpunkten (identifiziert durch Abonnement-Ids), die verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="07a7e-167">Target policy object handles notification delivery policy at two different levels - endpoint types (Windows, iOS and Android) that should be targeted, and specific endpoints (identified by subscription ids) that should be targeted.</span></span> |
| <span data-ttu-id="07a7e-168">targetPolicy.platformTypes</span><span class="sxs-lookup"><span data-stu-id="07a7e-168">targetPolicy.platformTypes</span></span> | <span data-ttu-id="07a7e-169">Edm.ComplexType Auflistung (EnumType)</span><span class="sxs-lookup"><span data-stu-id="07a7e-169">Edm.ComplexType, Collection (EnumType)</span></span> | <span data-ttu-id="07a7e-170">Verwenden Sie zum Filtern der Benachrichtigung Verteilung einer bestimmten Plattform oder Plattformen.</span><span class="sxs-lookup"><span data-stu-id="07a7e-170">Use to filter the notification distribution to a specific platform or platforms.</span></span> <span data-ttu-id="07a7e-171">Standardmäßig werden alle Push Endpunkttypen (iOS, Windows und Android) aktiviert.</span><span class="sxs-lookup"><span data-stu-id="07a7e-171">By default, all push endpoint types (iOS, Windows, and Android) are enabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="07a7e-172">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="07a7e-172">Relationships</span></span>
<span data-ttu-id="07a7e-173">Keine.</span><span class="sxs-lookup"><span data-stu-id="07a7e-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="07a7e-174">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="07a7e-174">JSON representation</span></span>
<span data-ttu-id="07a7e-175">Im folgenden finden eine JSON-Darstellung der Ressource, wenn Sie eine direkte visuelle Benachrichtigung veröffentlichen, die an das Zielbetriebssystem übermittelt werden.</span><span class="sxs-lookup"><span data-stu-id="07a7e-175">The following is a JSON representation of the resource when you publish a direct visual notification that is delivered to the destination operating system.</span></span>

```json
{   
  "targetHostName": "String",
  "appNotificationId": "String",
  "expirationDateTime": "DateTimeOffset",
  "payload":  
  {
    "visualContent": 
    {
      "title": "String",
      "body": "String"
    },
  },
  "displayTimeToLive": "Int",
  "priority": "Enum",
  "groupName": "String",
  "targetPolicy":
  {
    "platformTypes": [ 
      "Enum"
    ]
  }
}
```

<span data-ttu-id="07a7e-176">Im folgenden finden eine JSON-Darstellung der Ressource, wenn Sie eine Benachrichtigung über eine unformatierte Daten veröffentlichen, die an die app-Clients übermittelt werden.</span><span class="sxs-lookup"><span data-stu-id="07a7e-176">The following is a JSON representation of the resource when you publish a raw data notification that is delivered to app clients.</span></span>
```json
{   
  "targetHostName": "String",
  "appNotificationId": "String",
  "expirationDateTime": "DateTimeOffset",
  "payload":  
  {
    "rawContent": "String"
  },
  "displayTimeToLive": "Int",
  "priority": "Enum",
  "groupName": "String",
  "targetPolicy":
  {
    "platformTypes": [ 
      "Enum"
    ]
  }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/projectrome-notification.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
