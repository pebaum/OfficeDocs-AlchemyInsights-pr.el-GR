---
title: Ορισμός αυτόματων απαντήσεων για το γραμματοκιβώτιο ενός χρήστη
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506518"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Ορισμός αυτόματων απαντήσεων για το γραμματοκιβώτιο ενός χρήστη

**Μέθοδος 1**

1. Είσοδος στην πύλη του Office 365.

2. Μεταβείτε στην επιλογή **Χρήστες > Ενεργοί χρήστες** (ή **Ομάδες > Κοινόχρηστα γραμματοκιβώτια** εάν έχετε κάνει αυτή τη ρύθμιση σε ένα κοινόχρηστο γραμματοκιβώτιο).

3. Επιλέξτε έναν χρήστη που έχει γραμματοκιβώτιο του Microsoft Exchange.

4. Στο αναδυόμενο μενού στα δεξιά, μεταβείτε στις **Ρυθμίσεις αλληλογραφίας > Αυτόματες απαντήσεις** (εάν πρόκειται για ένα κοινόχρηστο γραμματοκιβώτιο, απλώς κάντε κλικ στην επιλογή **Αυτόματες απαντήσεις** στο αναδυόμενο μενού).

**Μέθοδος 2**

1. Πραγματοποιήστε είσοδο στην πύλη διαχείρισης του Office 365, χρησιμοποιώντας τα διαπιστευτήρια διαχειριστή.

2. Αναπτύξτε τα **Κέντρα διαχείρισης** και, στη συνέχεια, κάντε κλικ στην επιλογή **Ανταλλαγή**.

3. Κάντε κλικ στην εικόνα στην επάνω δεξιά γωνία, κάντε κλικ στην επιλογή **Άλλος χρήστης** και, στη συνέχεια, επιλέξτε το γραμματοκιβώτιο χρήστη που θέλετε να αλλάξετε.

4. Στην αριστερή πλευρά, επιλέξτε **Επιλογές**, κάντε κλικ στην επιλογή **Οργάνωση ηλεκτρονικού ταχυδρομείου** και, στη συνέχεια, κάντε κλικ στην επιλογή **Αυτόματες απαντήσεις.**

**Μέθοδος 3**

Εκτελέστε το ακόλουθο cmdlet στο Exchange Online PowerShell:

PowerShellCopy

    Set-MailboxAutoReplyConfiguration

Για περισσότερες πληροφορίες σχετικά με αυτό το cmdlet, ανατρέξτε στο θέμα [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).