---
title: Παράκαμψη λόμπι
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889082"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Έλεγχος των ρυθμίσεων του λόμπι και του επιπέδου συμμετοχής σε ομάδες

Αν θέλετε να επιτρέψετε σε όλους, συμπεριλαμβανομένων των τηλεφωνικών κλήσεων, των εξωτερικών και των ανώνυμων χρηστών, να **παρακάμπτουν το λόμπι**, χρησιμοποιήστε το PowerShell για να ολοκληρώσετε αυτήν την εργασία. Ακολουθούν ένα παράδειγμα τροποποίησης της καθολικής σύσκεψης πολιτικής για τον οργανισμό σας.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Αυτό το cmdlet απαιτεί αυτήν τη στιγμή τη χρήση του Skype για επαγγελματική PowerShell λειτουργική μονάδα. Για να ρυθμίσετε για να χρησιμοποιήσετε αυτό το cmdlet, ελέγξτε τη [Διαχείριση πολιτικών μέσω PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Αφού ορίσετε μια πολιτική, θα πρέπει να την εφαρμόσετε στους χρήστες. ή, εάν τροποποιήσατε την καθολική πολιτική, θα ισχύει αυτόματα για τους χρήστες. Για οποιαδήποτε αλλαγή πολιτικής, πρέπει να περιμένετε τουλάχιστον **4 ώρες έως και 24 ώρες** για να ισχύσουν οι πολιτικές. 

Βεβαιωθείτε ότι έχετε επανεξετάσει την τεκμηρίωση παρακάτω πριν κάνετε αυτές τις αλλαγές για να καταλάβετε ακριβώς τι επιτρέπει αυτό.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Κατανόηση των ομάδων που πληρούν τους ελέγχους πολιτικής του λόμπι

Αυτές οι ρυθμίσεις ελέγχουν ποιοι συμμετέχοντες στη σύσκεψη περιμένουν στο λόμπι πριν γίνουν δεκτοί στη σύσκεψη και το επίπεδο συμμετοχής που τους επιτρέπεται σε μια σύσκεψη. Μπορείτε να χρησιμοποιήσετε το PowerShell για να ενημερώσετε τις ρυθμίσεις πολιτικής σύσκεψης που δεν έχουν ακόμη υλοποιηθεί (με την ένδειξη "προσεχώς") στο κέντρο διαχείρισης ομάδων. Δείτε παρακάτω για ένα παράδειγμα cmdlet PowerShell που επιτρέπει σε όλους τους χρήστες να παρακάμψετε το λόμπι.

- Η αυτόματη ένταξη των [ατόμων](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) είναι μια πολιτική ανά διοργανωτή που ελέγχει αν τα άτομα συμμετέχουν σε μια σύσκεψη απευθείας ή περιμένουν στο λόμπι μέχρι να εισαχθούν από έναν εξουσιοδοτημένο χρήστη.

- [Να επιτρέψετε σε ανώνυμους χρήστες να ξεκινήσουν μια σύσκεψη](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) είναι μια πολιτική ανά διοργανωτή που ελέγχει αν τα ανώνυμα άτομα, συμπεριλαμβανομένων των χρηστών Β2Β και ομόσπονδων, μπορούν να ενταχθούν στη σύσκεψη του χρήστη χωρίς έλεγχο ταυτότητας χρήστη από τον οργανισμό στην παρουσία.

- [Να επιτρέπεται στους χρήστες τηλεφωνικών κλήσεων να παρακάμπτουν το λόμπι](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(προσεχώς**) είναι μια πολιτική ανά διοργανωτή που ελέγχει αν τα άτομα που κάνουν κλήση μέσω τηλεφώνου συμμετέχουν στη σύσκεψη απευθείας ή περιμένουν στο λόμπι, ανεξάρτητα από την **Αυτόματη** αποδοχή των χρηστών.

- [Επιτρέψτε στους διοργανωτές να παρακάμπτουν τις ρυθμίσεις του λόμπι](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**προσεχώς**) είναι μια πολιτική ανά διοργανωτή που ελέγχει αν ο οργανωτής της σύσκεψης μπορεί να παρακάμψει τις ρυθμίσεις του λόμπι που ένας διαχειριστής έχει ορίσει να δέχεται **αυτόματα άτομα** και **να επιτρέπει στους χρήστες εισερχόμενων κλήσεων να παρακάμπτουν το λόμπι** όταν προγραμματίσουν μια νέα σύσκεψη.

**Σημείωση:** Διαβάστε την [ενότητα Διαχείριση πολιτικών συσκέψεων στις ομάδες](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) για μια πλήρη επισκόπηση των πολιτικών συσκέψεων των ομάδων της Microsoft.
