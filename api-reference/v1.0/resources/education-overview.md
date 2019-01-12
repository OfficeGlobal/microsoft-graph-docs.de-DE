---
title: Arbeiten mit Education-APIs in Microsoft Graph
description: Mit Education-APIs in Microsoft Graph werden Office 365-Ressourcen und -Daten mithilfe von Informationen optimiert, die für Bildungsszenarien, u. a. Schulen, Schüler, Studenten, Lehrer, Kurse und Anmeldungen relevant sind. Dies erleichtert das Erstellen von Lösungen, die in Bildungsressourcen integriert werden.
localization_priority: Priority
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 1b12910899ce5645d8d3f69f96cb7a8f61ba0df5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975848"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a><span data-ttu-id="9cc4e-104">Arbeiten mit Education-APIs in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9cc4e-104">Working with education APIs in Microsoft Graph</span></span>

<span data-ttu-id="9cc4e-105">Mit Education-APIs in Microsoft Graph werden Office 365-Ressourcen und -Daten mithilfe von Informationen optimiert, die für Bildungsszenarien, u. a. Schulen, Schüler, Studenten, Lehrer, Kurse und Anmeldungen relevant sind.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-105">The education APIs in Microsoft Graph enhance Office 365 resources and data with information that is relevant for education scenarios, including schools, students, teachers, classes, and enrollments.</span></span> <span data-ttu-id="9cc4e-106">Dies erleichtert das Erstellen von Lösungen, die in Bildungsressourcen integriert werden.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-106">This makes it easy for you to build solutions that integrate with educational resources.</span></span>

<span data-ttu-id="9cc4e-107">Education-APIs umfassen Ressourcen für Listenerstellung und Zuordnungen, die Sie für die Kommunikation mit Listenerstellungsdiensten in Microsoft Teams verwenden können.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-107">The education APIs include rostering resources and assignments resources that you can use to interact with the rostering services in Microsoft Teams.</span></span> <span data-ttu-id="9cc4e-108">Sie können diese Ressourcen zum Verwalten von Schulplänen verwenden.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-108">You can use these resources to manage a school roster.</span></span>

## <a name="authorization"></a><span data-ttu-id="9cc4e-109">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9cc4e-109">Authorization</span></span>

<span data-ttu-id="9cc4e-110">Damit die Education-APIs in Microsoft Graph aufgerufen werden können, muss Ihre App ein Zugriffstoken erwerben.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-110">To call the education APIs in Microsoft Graph, your app will need to acquire an access token.</span></span> <span data-ttu-id="9cc4e-111">Weitere Informationen zu Zugriffstoken finden Sie unter [Abrufen von Zugriffstoken zum Aufrufen von Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span><span class="sxs-lookup"><span data-stu-id="9cc4e-111">For details about access tokens, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="9cc4e-112">Zudem muss Ihre App über die entsprechenden Berechtigungen verfügen.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-112">Your app will also need the appropriate permissions.</span></span> <span data-ttu-id="9cc4e-113">Weitere Informationen finden Sie unter [Education-Berechtigungen](/graph/permissions-reference#education-permissions).</span><span class="sxs-lookup"><span data-stu-id="9cc4e-113">For more information, see [Education permissions](/graph/permissions-reference#education-permissions).</span></span> 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a><span data-ttu-id="9cc4e-114">App-Berechtigungen zum Aktivieren der Zustimmung von Schul-IT-Administratoren</span><span class="sxs-lookup"><span data-stu-id="9cc4e-114">App permissions to enable school IT admins to consent</span></span> 

<span data-ttu-id="9cc4e-115">Um Apps bereitzustellen, die in Education-APIs in Microsoft Graph integriert sind, müssen Schul-IT-Administratoren zunächst ihre Zustimmung für die von der App angeforderten Berechtigungen erteilen.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-115">To deploy apps that are integrated with the Education APIs in Microsoft Graph, school IT admins must first grant consent to the permissions requested by the app.</span></span> <span data-ttu-id="9cc4e-116">Diese Zustimmung muss nur einmal erteilt werden, sofern sich die Berechtigungen nicht ändern.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-116">This consent has to be granted only once, unless the permissions change.</span></span> <span data-ttu-id="9cc4e-117">Nachdem der Administrator seine Zustimmung erteilt hat, wird die App für alle Benutzer im Mandanten bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-117">After the admin consents, the app is provisioned for all users in the tenant.</span></span>

<span data-ttu-id="9cc4e-118">Verwenden Sie den folgenden REST-Aufruf, um ein Dialogfeld für die Zustimmung anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-118">To show a consent dialog box, use the following REST call.</span></span>

```
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

|<span data-ttu-id="9cc4e-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="9cc4e-119">Parameter</span></span>|<span data-ttu-id="9cc4e-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9cc4e-120">Description</span></span>|
|:--------|:----------|
|<span data-ttu-id="9cc4e-121">Mandant</span><span class="sxs-lookup"><span data-stu-id="9cc4e-121">Tenant</span></span>|<span data-ttu-id="9cc4e-122">Mandanten-ID der Schule.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-122">Tenant ID of the school.</span></span> <span data-ttu-id="9cc4e-123">Verwenden Sie die vollständige-ID, die „onmicrosoft.com“ enthält.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-123">Use the full ID, which includes onmicrosoft.com.</span></span>|
|<span data-ttu-id="9cc4e-124">clientId</span><span class="sxs-lookup"><span data-stu-id="9cc4e-124">clientId</span></span>|<span data-ttu-id="9cc4e-125">Client-ID der App.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-125">Client ID of the app.</span></span>|
|<span data-ttu-id="9cc4e-126">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="9cc4e-126">redirectUrl</span></span>|<span data-ttu-id="9cc4e-127">App-Umleitungs-URL.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-127">App redirect URL.</span></span>|


## <a name="rostering"></a><span data-ttu-id="9cc4e-128">Listenerstellung</span><span class="sxs-lookup"><span data-stu-id="9cc4e-128">Rostering</span></span>

<span data-ttu-id="9cc4e-129">Mit Listenerstellungs-APIs können Sie Daten von einem Office 365-Mandanten der Schule extrahieren, der mit [Microsoft School Data Sync](https://sds.microsoft.com/) bereitgestellt wurde. Diese APIs bieten Zugriff auf Informationen zu Schulen, Abschnitten, Lehrern, Schülern, Studenten und Listen.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-129">The rostering APIs enable you to extract data from a school's Office 365 tenant provisioned with [Microsoft School Data Sync](https://sds.microsoft.com/). These APIs provide access to information about schools, sections, teachers, students, and rosters.</span></span> <span data-ttu-id="9cc4e-130">Die APIs unterstützen sowohl Szenarien vom Typ „Nur App“ (Synchronisierung) als auch vom Typ „App und Benutzer“ (interaktiv).</span><span class="sxs-lookup"><span data-stu-id="9cc4e-130">The APIs support both app-only (sync) scenarios, and app + user (interactive) scenarios.</span></span> <span data-ttu-id="9cc4e-131">APIs, die interaktive Szenarien unterstützen, erzwingen auf Grundlage der Benutzerrolle, die die API aufruft, regionsspezifische RBAC-Richtlinien.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-131">The APIs that support interactive scenarios enforce region-appropriate RBAC policies based on the user role calling the API.</span></span> <span data-ttu-id="9cc4e-132">Dies ermöglicht eine konsistente API und eine minimale Richtlinienoberfläche, unabhängig von der Verwaltungskonfiguration innerhalb der Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-132">This provides a consistent API and minimal policy surface, regardless of the administrative configuration within tenants.</span></span> <span data-ttu-id="9cc4e-133">Die APIs bieten darüber hinaus auch bildungsspezifische Berechtigungen, um sicherzustellen, dass der richtige Benutzer auf die Daten zugreifen kann.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-133">In addition, the APIs also provide education-specific permissions to ensure that the right user has access to the data.</span></span>

<span data-ttu-id="9cc4e-134">Mithilfe von Listenerstellungs-APIs erhält der App-Benutzer Antworten auf die folgenden Fragen:</span><span class="sxs-lookup"><span data-stu-id="9cc4e-134">You can use the rostering APIs to enable an app user to know:</span></span>

- <span data-ttu-id="9cc4e-135">Wer bin ich?</span><span class="sxs-lookup"><span data-stu-id="9cc4e-135">Who I am</span></span>
- <span data-ttu-id="9cc4e-136">An welchen Kursen nehme ich teil bzw. welche Kurse unterrichte ich?</span><span class="sxs-lookup"><span data-stu-id="9cc4e-136">What classes I attend or teach</span></span>
- <span data-ttu-id="9cc4e-137">Was muss ich wann tun?</span><span class="sxs-lookup"><span data-stu-id="9cc4e-137">What I need to do and by when</span></span>

<span data-ttu-id="9cc4e-138">Die Listenerstellungs-APIs bieten die folgenden zentralen Ressourcen:</span><span class="sxs-lookup"><span data-stu-id="9cc4e-138">The rostering APIs provide the following key resources:</span></span>

- <span data-ttu-id="9cc4e-139">[educationSchool](educationschool.md): Schule.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-139">[educationSchool](educationschool.md) - Represents the school.</span></span>
- <span data-ttu-id="9cc4e-140">[educationClass](educationclass.md): Kurs in einer Schule.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-140">[educationClass](educationclass.md) - Represents a class within a school.</span></span>
- <span data-ttu-id="9cc4e-141">[educationTerm](educationterm.md): Ein festgelegter Teil des akademischen Jahres.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-141">[educationTerm](educationterm.md) - Represents a designated portion of the academic year.</span></span>
- <span data-ttu-id="9cc4e-142">[educationTeacher](educationteacher.md): Ein Benutzer mit der primären Rolle „Lehrer“.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-142">[educationTeacher](educationteacher.md) - Represents a users with the primary role of 'Teacher'.</span></span>
- <span data-ttu-id="9cc4e-143">[educationStudent](educationstudent.md): Ein Benutzer mit der primären Rolle „Schüler/Student“.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-143">[educationStudent](educationstudent.md) - Represents a users with the primary role of 'student'.</span></span>

<span data-ttu-id="9cc4e-144">Die Listenerstellungs-APIs unterstützen die folgenden Szenarien:</span><span class="sxs-lookup"><span data-stu-id="9cc4e-144">The rostering APIs support the following scenarios:</span></span>

- [<span data-ttu-id="9cc4e-145">Auflisten aller Schulen</span><span class="sxs-lookup"><span data-stu-id="9cc4e-145">List all schools</span></span>](../api/educationroot-list-schools.md) 
- [<span data-ttu-id="9cc4e-146">Auflisten von Schulen, in denen ein Kurs unterrichtet wird</span><span class="sxs-lookup"><span data-stu-id="9cc4e-146">List schools in which a class is taught</span></span>](../api/educationclass-list-schools.md)
- [<span data-ttu-id="9cc4e-147">Auflisten von Schulen für einen Benutzer</span><span class="sxs-lookup"><span data-stu-id="9cc4e-147">List schools for a user</span></span>](../api/educationuser-list-schools.md)
- [<span data-ttu-id="9cc4e-148">Abrufen aller Kurse</span><span class="sxs-lookup"><span data-stu-id="9cc4e-148">Get all classes</span></span>](../api/educationroot-list-classes.md)
- [<span data-ttu-id="9cc4e-149">Abrufen von Kursen einer Schule</span><span class="sxs-lookup"><span data-stu-id="9cc4e-149">Get classes in a school</span></span>](../api/educationschool-list-classes.md)
- [<span data-ttu-id="9cc4e-150">Auflisten von Kursen für einen Benutzer</span><span class="sxs-lookup"><span data-stu-id="9cc4e-150">List classes for a user</span></span>](../api/educationuser-list-classes.md)
- [<span data-ttu-id="9cc4e-151">Hinzufügen von Kursen zu einer Schule</span><span class="sxs-lookup"><span data-stu-id="9cc4e-151">Add classes to a school</span></span>](../api/educationschool-post-classes.md)
- [<span data-ttu-id="9cc4e-152">Abrufen von Schülern/Studenten und Lehrern für einen Kurs</span><span class="sxs-lookup"><span data-stu-id="9cc4e-152">Get students and teachers for a class</span></span>](../api/educationclass-list-members.md)
- [<span data-ttu-id="9cc4e-153">Hinzufügen von Mitgliedern zu einem Kurs</span><span class="sxs-lookup"><span data-stu-id="9cc4e-153">Add members to a class</span></span>](../api/educationclass-post-members.md) 
- [<span data-ttu-id="9cc4e-154">Auflisten von Lehrern für einen Kurs</span><span class="sxs-lookup"><span data-stu-id="9cc4e-154">List teachers for a class</span></span>](../api/educationclass-list-teachers.md)
- [<span data-ttu-id="9cc4e-155">Abrufen von Benutzern in einer Schule</span><span class="sxs-lookup"><span data-stu-id="9cc4e-155">Get users in a school</span></span>](../api/educationschool-list-users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="next-steps"></a><span data-ttu-id="9cc4e-156">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="9cc4e-156">Next steps</span></span>
<span data-ttu-id="9cc4e-157">Verwenden Sie die Microsoft Graph-Education-APIs zum Erstellen von Lösungen für Bildungseinrichtungen, die auf Schulpläne zugreifen.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-157">Use the Microsoft Graph education APIs to build education solutions that access school rosters.</span></span> <span data-ttu-id="9cc4e-158">So erhalten Sie weitere Informationen:</span><span class="sxs-lookup"><span data-stu-id="9cc4e-158">To learn more:</span></span>

- <span data-ttu-id="9cc4e-159">Erfahren Sie, welche Ressourcen und Methoden für Ihr Szenario am besten geeignet sind.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-159">Explore the resources and methods that are most helpful to your scenario.</span></span>
- <span data-ttu-id="9cc4e-160">Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus.</span><span class="sxs-lookup"><span data-stu-id="9cc4e-160">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

