---
title: Δημιουργήστε ένα email αλιευμάτων όλα
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286193"
---
# <a name="create-an-email-catch-all"></a>Δημιουργήστε ένα email αλιευμάτων όλα

Η χρήση ενός αλιεύματος όλα αποθαρρύνεται έντονα. Είναι καλύτερα να παρέχει μια αναπήδηση πίσω στον αποστολέα αφήνοντας τους αποστολείς γνωρίζουν το μήνυμά τους δεν θα μπορούσε να παραδοθεί ως απευθύνεται έτσι ώστε να μπορούν να αναλάβουν δράση. Μπορείτε επίσης να περιορίσετε την εποπτευόμενη γραμματοκιβώτιο για να πιάσει μόνο πρώην έγκυρες διευθύνσεις ηλεκτρονικού ταχυδρομείου. 

Κάθε αλιευμάτων όλα τα γραμματοκιβώτια θα λάβουν μια καλή συμφωνία των spam και μπορεί τελικά να συμπληρώσετε αν δεν παρακολουθούνται στενά. (Υπάρχουν όρια παραλαβής.) 

Εάν αποφασίσετε να συνεχίσετε, ακολουθήστε τα εξής βήματα:

1. Δημιουργήστε μια δυναμική ομάδα διανομής & συμπεριλάβετε "όλους τους τύπους παραληπτών."

2. Δημιουργήστε ένα αποκλειστικό γραμματοκιβώτιο για να πιάσει τα ηλεκτρονικά ταχυδρομεία, για παράδειγμα, catchall@domain.com.

3. Για το συγκεκριμένο τομέα, ρυθμίστε το DomainType σε "InternalRelay". Εάν αργότερα αφαιρέσετε τα αλιεύματα όλα, φροντίστε να ρυθμίσετε τον τομέα πίσω σε έγκυρες.

4. Δημιουργήστε έναν κανόνα μεταφοράς Mailflow ως εξής:

    - Εάν ο αποστολέας είναι "εκτός του οργανισμού"
    - Ανακατεύθυνση του μηνύματος σε Catchall@domain.com
    - Εκτός αν ο παραλήπτης είναι μέλος της allusers@domain.com (ομάδα διανομής περιέχει όλα τα μέλη)
    - Βεβαιωθείτε για την επικύρωση ότι νέα γραμματοκιβώτια προστίθενται στη δυναμική ομάδα διανομής
