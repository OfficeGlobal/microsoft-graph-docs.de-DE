---
title: Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen
description: 'Sie werden durch ein Beispiel geführt, um die Verwendung *offener Erweiterungen* zu veranschaulichen. '
author: dkershaw10
ms.openlocfilehash: 37df1bd03e68b00be41496ee9f66a076d8758149
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337170"
---
# <a name="add-custom-data-to-users-using-open-extensions"></a><span data-ttu-id="5e13d-103">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="5e13d-103">Add custom data to users using open extensions</span></span>
<span data-ttu-id="5e13d-104">Sie werden durch ein Beispiel geführt, um die Verwendung *offener Erweiterungen* zu veranschaulichen.</span><span class="sxs-lookup"><span data-stu-id="5e13d-104">We're going to walk you through an example to demonstrate how to use *open extensions*.</span></span> 

<span data-ttu-id="5e13d-p101">Angenommen, Sie erstellen eine Anwendung, die auf vielen verschiedenen Clientplattformen, z. B. Desktop und Mobil, verfügbar ist.  Sie möchten zulassen, dass Benutzer ihre eigene Benutzeroberfläche konfigurieren, damit diese konsistent ist, unabhängig davon, mit welchem Gerät sie sich bei der App anmelden. Dies ist eine allgemeine Anforderung für die meisten Apps.</span><span class="sxs-lookup"><span data-stu-id="5e13d-p101">Imagine you're building an application that is available on lots of different client platforms, such as desktop and mobile.  You want to let users configure their UI experience so it’s consistent no matter which device they use to sign in to your app. This is a common requirement for most apps.</span></span> 

<span data-ttu-id="5e13d-108">In diesem Szenario erlernen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="5e13d-108">For this scenario, we're going to show you how to:</span></span>

1. <span data-ttu-id="5e13d-109">Hinzufügen einer offenen Erweiterung, die einige Roamingprofilinformationen über den Benutzer darstellt.</span><span class="sxs-lookup"><span data-stu-id="5e13d-109">Add an open extension representing some roaming profile information about the user.</span></span>
2. <span data-ttu-id="5e13d-110">Abfragen des Benutzers und Zurückgeben des Roamingprofils.</span><span class="sxs-lookup"><span data-stu-id="5e13d-110">Query the user and return the roaming profile.</span></span>
3. <span data-ttu-id="5e13d-111">Ändern der Roamingprofilinformationen des Benutzers (der Wert der offenen Erweiterung).</span><span class="sxs-lookup"><span data-stu-id="5e13d-111">Change the user's roaming profile information (the open extension value).</span></span>
4. <span data-ttu-id="5e13d-112">Löschen der Roamingprofilinformationen des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="5e13d-112">Delete the user's roaming profile information.</span></span>

><span data-ttu-id="5e13d-p102">**Hinweis:** In diesem Thema wird gezeigt, wie offenen Erweiterungen in einer *user*-Ressource hinzugefügt, gelesen, aktualisiert und gelöscht werden.  Diese Methoden werden auch für die Ressourcentypen *administrativeUnit*, *contact*, *device*, *event*, *group*, *group event*, *group post* und *organizaton* unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5e13d-p102">**Note:** This topic shows you how to add, read, update and delete open extensions on a *user* resource.  These methods are also supported for the *administrativeUnit*, *contact*, *device*, *event*, *group*, *group event*, *group post* and *organizaton* resource types.</span></span>  
<span data-ttu-id="5e13d-p103">Aktualisieren Sie einfach die Beispielanforderungen unter Verwendung dieser Ressourcentypen. Die in den Beispielen dargestellten Antworten sind aus Platzgründen möglicherweise abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="5e13d-p103">Simply update the example requests below using any of those resource types. The responses shown in the examples below may be truncated for brevity.</span></span> 

## <a name="1-add-roaming-profile-information"></a><span data-ttu-id="5e13d-117">1. Hinzufügen von Roamingprofilinformationen</span><span class="sxs-lookup"><span data-stu-id="5e13d-117">1. Add roaming profile information</span></span>
<span data-ttu-id="5e13d-p104">Der Benutzer meldet sich bei der App an und konfiguriert das Aussehen und Verhalten der App.  Diese App-Einstellungen sind roamingfähig, der Benutzer erhält also dieselbe Oberfläche, ganz gleich, mit welchem Gerät er sich bei der App anmeldet.  Hier sehen Sie, wie die Roamingprofilinformationen zu einer Benutzerressource hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="5e13d-p104">The user signs in to the app and configures the look and feel of the app.  These app settings should roam so that the user gets the same experience on whatever device they sign in to the app from.  Here we'll see how to add the roaming profile information to a user resource.</span></span>

##### <a name="request"></a><span data-ttu-id="5e13d-121">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e13d-121">Request</span></span>
```http
POST https://graph.microsoft.com/v1.0/me/extensions
Content-type: application/json
{
    "@odata.type":"microsoft.graph.openTypeExtension",
    "extensionName":"com.contoso.roamingSettings",
    "theme":"dark",
    "color":"purple",
    "lang":"Japanese"
}
```
##### <a name="response"></a><span data-ttu-id="5e13d-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e13d-122">Response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420

{
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "extensionName": "com.contoso.roamingSettings",
    "id": "com.contoso.roamingSettings",
    "theme": "dark",
    "color": "purple",
    "lang": "Japanese"
}
```

## <a name="2-retrieve-roaming-profile-information"></a><span data-ttu-id="5e13d-123">2. Abrufen von Roamingprofilinformationen</span><span class="sxs-lookup"><span data-stu-id="5e13d-123">2. Retrieve roaming profile information</span></span>
<span data-ttu-id="5e13d-p105">Wenn sich der Benutzer von einem anderen Gerät aus bei der App anmeldet, kann die App die Profildetails des Benutzers und auch die Roamingeinstellungen abrufen. Dies kann durch Abrufen der Benutzerressource und Erweitern der Erweiterungsnavigationseigenschaft erfolgen.</span><span class="sxs-lookup"><span data-stu-id="5e13d-p105">When the user signs in to the app from another device, the app can retrieve the user's profile details as well as their roaming settings. This can be done by getting the user's resource and expanding the extension navigation property.</span></span>

##### <a name="request"></a><span data-ttu-id="5e13d-126">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e13d-126">Request</span></span>
```http
GET https://graph.microsoft.com/v1.0/me?$select=id,displayName,mail,mobilePhone&$expand=extensions
```
##### <a name="response"></a><span data-ttu-id="5e13d-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e13d-127">Response</span></span>
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 420

{
    "id": "84b80893-8749-40a3-97b7-68513b600544",
    "displayName": "John Smith",
    "mail": "john@contoso.com",
    "mobilePhone": "1-555-6589",
    "extensions": [
        {
            "@odata.type": "#microsoft.graph.openTypeExtension",
            "extensionName": "com.contoso.roamingSettings",
            "id": "com.contoso.roamingSettings",
            "theme": "dark",
            "color": "purple",
            "lang": "Japanese"
        }
    ]
}
```
><span data-ttu-id="5e13d-128">**Hinweis:** Wenn Sie mehrere Erweiterungen haben, können Sie nach der *ID* filtern, um die gewünschte Erweiterung zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="5e13d-128">**Note:** If you have multiple extensions, you can filter on the *id* to get the extension that you are interested in.</span></span>

## <a name="3-change-roaming-profile-information"></a><span data-ttu-id="5e13d-129">3. Ändern der Roamingprofilinformationen</span><span class="sxs-lookup"><span data-stu-id="5e13d-129">3. Change roaming profile information</span></span>
<span data-ttu-id="5e13d-p106">Der Benutzer kann seine Roamingprofilinformationen ändern.  Diese Aktualisierung kann über eine ```PATCH``` im Wert der offenen Erweiterung erfolgen.</span><span class="sxs-lookup"><span data-stu-id="5e13d-p106">The user may choose to change their roaming profile information.  This update can be done with a ```PATCH``` on the open extension value.</span></span> 

##### <a name="request"></a><span data-ttu-id="5e13d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e13d-132">Request</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
Content-type: application/json
{
    "theme":"light",
    "color":"yellow",
    "lang":"Swahili"
}
```

##### <a name="response"></a><span data-ttu-id="5e13d-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e13d-133">Response</span></span>
```
HTTP/1.1 204 No content
```

## <a name="4-delete-a-users-roaming-profile"></a><span data-ttu-id="5e13d-134">4. Löschen der Roamingprofilinformationen eines Benutzers</span><span class="sxs-lookup"><span data-stu-id="5e13d-134">4. Delete a user's roaming profile</span></span>
<span data-ttu-id="5e13d-p107">Der Benutzer entscheidet, dass er kein Roamingprofil mehr benötigt, und löscht es. Dies kann über eine ```DELETE```-Anforderung im Wert der offenen Erweiterung erfolgen.</span><span class="sxs-lookup"><span data-stu-id="5e13d-p107">The user decides that they don't want a roaming profile anymore, so they delete it. This can be done with a ```DELETE``` request on the open extension value.</span></span>

##### <a name="request"></a><span data-ttu-id="5e13d-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e13d-137">Request</span></span>
```http
DELETE https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
```

##### <a name="response"></a><span data-ttu-id="5e13d-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e13d-138">Response</span></span>
```
HTTP/1.1 204 No content
```

## <a name="see-also"></a><span data-ttu-id="5e13d-139">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="5e13d-139">See also</span></span>

- [<span data-ttu-id="5e13d-140">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="5e13d-140">Add custom data to resources using extensions</span></span>](extensibility-overview.md)
- [<span data-ttu-id="5e13d-141">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="5e13d-141">Add custom data to groups using schema extensions</span></span>](extensibility-schema-groups.md)
- [<span data-ttu-id="5e13d-142">openTypeExtension-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5e13d-142">openTypeExtension resource type</span></span>](/graph/api/resources/opentypeextension?view=graph-rest-1.0)
- [<span data-ttu-id="5e13d-143">Offene Erweiterung erstellen</span><span class="sxs-lookup"><span data-stu-id="5e13d-143">Create open extension</span></span>](/graph/api/opentypeextension-post-opentypeextension?view=graph-rest-1.0)
- [<span data-ttu-id="5e13d-144">Offene Erweiterung abrufen</span><span class="sxs-lookup"><span data-stu-id="5e13d-144">Get open extension</span></span>](/graph/api/opentypeextension-get?view=graph-rest-1.0)
- [<span data-ttu-id="5e13d-145">Offene Erweiterung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5e13d-145">Update open extension</span></span>](/graph/api/opentypeextension-update?view=graph-rest-1.0)
- [<span data-ttu-id="5e13d-146">Offene Erweiterung löschen</span><span class="sxs-lookup"><span data-stu-id="5e13d-146">Delete open extension</span></span>](/graph/api/opentypeextension-delete?view=graph-rest-1.0)