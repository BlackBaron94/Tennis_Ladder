# Tennis Ladder Project
## Περιγραφή
Η εφαρμογή διατηρεί κι επεξεργάζεται δεδομένα κατάταξης Τέννις. Οι δυνατότητες περιλαμβάνουν προσθήκη, 
διαγραφή παίκτη, τυχαιοποιημένη αρχική εισαγωγή παικτών, έλεγχο και καταγραφή πρόκλησης και 
αποτελεσμάτων αγώνων. Επιπλέον, υπάρχει λειτουργία ελέγχου αδράνειας (1 μήνας) με μείωση θέσης.

## Table of Contents
- [Εγκατάσταση](#οδηγίες-εγκατάστασης)
- [Εγχειρίδιο Χρήσης](#εγχειρίδιο-χρήσης)
- [Χρήση](#χρήση)
- [Επικοινωνία](#επικοινωνία)

## Οδηγίες Εγκατάστασης
    -Κώδικας
        Για να τρέξει ο κώδικας χρειάζεται εγκατεστημένη έκδοση 3. Python καθώς και τις βιβλιοθήκες tkinter, 
        sqlite3, datetime(included), random(included)
    -Executable
        Για να τρέξει το onefile .exe δεν χρειάζεται τίποτα από τα παραπάνω.


## Εγχειρίδιο Χρήσης
    Εγχειρίδο Χρήσης Εφαρμογής “Tennis Ladder”


        Ξεκινώντας, ανοίγοντας το αρχείο “Tennis Ladder.exe” θα δημιουργηθεί στο φάκελο που βρίσκεται ένα 
        νέο αρχείο ονόματι “tennis_club.db”. Αυτό το αρχείο είναι βασικό για την αποθήκευση της κατάταξής
        σας και τη σωστή λειτουργία του προγράμματος. Σε περίπτωση μετακίνησης του αρχείου 
        “Tennis Ladder.exe”, θα πρέπει να μετακινείται και το “tennis_club.db”, εξασφαλίζοντας 
        έτσι πλήρη φορητότητα.

    Μενού Προγράμματος

        Ξεκινώντας το πρόγραμμα βρίσκεστε στο κύριο μενού του προγράμματος. Εδώ, πατάτε κάποια από τις 
        επιλογές. Οι επιλογές "Διαγραφή Παίκτη", "Έλεγχος κατάταξης για αδρανείς παίκτες" και 
        "Εμφάνιση κατάταξης" δεν είναι διαθέσιμες αν δεν υπάρχουν παίκτες στην κατάταξη. Επιπλέον, για 
        την επιλογή "Έλεγχος και καταγραφή αποτελέσματος πρόκλησης" πρέπει να υπάρχουν τουλάχιστον 
        2 παίκτες στην κατάταξη.


    1. Αρχικοποίηση κατάταξης:

        Αυτή η επιλογή δίνει τη δυνατότητα για τυχαιοποιημένη πρώτη εισαγωγή παικτών σε άδεια κατάταξη. 
        Θα σας ζητηθεί να δώσετε όνομα και επίθετο παίκτη. Εισάγετε τα στοιχεία και το πρόγραμμα θα 
        αναγνωρίσει την πρώτη λέξη ως όνομα και τη δεύτερη λέξη ως επίθετο. Χωρίστε τα δύο με κενό. 
        Αν εισάγετε μόνο μία λέξη ή πάνω από δύο λέξεις το πρόγραμμα δεν θα εισάγει τον παίκτη και 
        θα σας ειδοποιήσει με σχετικό μήνυμα. Πατώντας "Καταχώρηση Παίκτη", αυτός εισάγεται στη λίστα 
        παικτών που εμφανίζεται στο κάτω μέρος του παραθύρου. Σε περίπτωση λάθους συνεχίστε κανονικά με
        τα υπόλοιπα μέλη και μπορείτε να διαγράψετε τη λάθος εισαγωγή μετά τη λήξη της διαδικασίας 
        αρχικοποίησης. Όταν θέλετε να ολοκληρώσετε την εισαγωγή, πιέστε "Τέλος Καταχωρήσεων". 
        Το πρόγραμμα θα τυχαιοποιήσει τη σειρά των παικτών που δώσατε και θα τους εισάγει στην κατάταξη.
        Η αρχικοποίηση της κατάταξης δε γίνεται αν δεν εισαχθεί κανένα όνομα ή αν η κατάταξη περιέχει 
        έστω κι έναν παίκτη. Σε αυτές τις περιπτώσεις ειδοποιείστε με το ανάλογο μήνυμα.

    2. Προσθήκη παίκτη:

        Μέσω αυτής της επιλογής μπορείτε να προσθέσετε έναν παίκτη είτε σε συγκεκριμένη θέση είτε 
        στο τέλος της κατάταξης. Η χρήση της συγκεκριμένης λειτουργίας μπορεί να γίνει είτε σε κενή 
        κατάταξη είτε σε κατάταξη που περιέχει ήδη παίκτες. Η εισαγωγή παίκτη προκαλεί αύξηση του 
        μεγέθους της κατάταξης κατά μία θέση. Πρώτα θα ερωτηθείτε αν θέλετε να εισάγετε σε συγκεκριμένη 
        θέση τον παίκτη. Στη συνέχεια, εισάγετε όνομα κι επίθετο ακολουθώντας τις οδηγίες και συμβουλές 
        που δόθηκαν και παραπάνω (βλ. 1., παράγραφος 2). Αν επιλέξατε συγκεκριμένη θέση θα σας ζητηθεί 
        τώρα. Όταν εισάγετε παίκτη σε συγκεκριμένη θέση, το άτομο που την κατείχε μέχρι τώρα θα 
        μετακινηθεί κατά μία θέση κάτω. Το ίδιο θα συμβεί και σε όλους τους χαμηλότερους σε κατάταξη 
        παίκτες. Για παράδειγμα, αν βάλετε τον παίκτη στη θέση 6, ο παίκτης που ήταν 6ος θα γίνει 7ος, 
        ο 7ος θα γίνει 8ος κ.ο.κ. 
        Αν προσπαθήσετε να εισάγετε παίκτη σε θέση μεγαλύτερη της επόμενη της τελευταίας θέσης θα 
        ειδοποιηθείτε με σχετικό μήνυμα. 
        Για παράδειγμα, αν η κατάταξη περιέχει 15 παίκτες, μπορείτε να εισάγετε παίκτη στη θέση 16, αλλά 
        όχι στη θέση 17 καθώς αυτό θα άφηνε τη θέση 16 κενή. 
        Στο τέλος της διαδικασίας, θα ενημερωθείτε με μήνυμα πως ο παίκτης προστέθηκε επιτυχώς είτε στη 
        θέση που επιλέξατε είτε στην τελευταία θέση.

    3. Διαγραφή παίκτη:

        Η επιλογή αυτή σας επιτρέπει να διαγράψετε έναν παίκτη. Όταν επιλεχθεί, θα σας ζητήσει να 
        εισάγετε τη θέση του παίκτη που θέλετε να διαγράψετε.
        Η διαγραφή παίκτη μειώνει το μέγεθος της κατάταξης κατά 1 θέση. Αν διαγραφεί παίκτης που 
        έχει άλλους παίκτες χαμηλότερα στην κατάταξη, θα προκληθεί άνοδος των παικτών αυτών κατά 
        μία θέση.
        Αν η κατάταξη είναι κενή ή αν επιλέξετε θέση προς διαγραφή που είναι κενή θα 
        ενημερωθείτε με σχετικό μήνυμα.


        ΠΡΟΣΟΧΗ!!! Η διαγραφή παίκτη είναι οριστική και αμετάκλητη, που σημαίνει πως δεδομένα 
        όπως αριθμός νικών, ηττών και τελευταία ημερομηνία δραστηριότητας που διατηρούνται από το
        πρόγραμμα θα χαθούν ΟΡΙΣΤΙΚΆ χωρίς δυνατότητα επανεισαγωγής τους ακόμα κι αν αυτές οι τιμές 
        είναι γνωστές.
        Για τον παραπάνω λόγο θα σας ζητηθεί να επιβεβαιώσετε τη διαγραφή του παίκτη.
        Προτείνεται να διασταυρώσετε αν το όνομα που σας δίνεται τώρα είναι του παίκτη που θέλετε 
        όντως να διαγράψετε. Αν απαντήσετε όχι, η διαγραφή ματαιώνεται χωρίς καμία αλλαγή.

    4. Έλεγχος και καταγραφή αποτελέσματος πρόκλησης:
        
        Με αυτή την επιλογή ελέγχεται αν η πρόκληση σε αγώνα είναι αποδεκτή βάσει των παρακάτω 
        κανόνων πρόκλησης:
            Η πρόκληση γίνεται αποδεκτή μόνο από παίκτη χαμηλότερης θέσης προς παίκτη υψηλότερης θέσης.
            Οι παίκτες θέσεων 1-9 μπορούν να προκαλέσουν παίκτη μέχρι 3 θέσεις πάνω.
            Οι παίκτες θέσεων 10 και κάτω μπορούν να προκαλέσουν παίκτη μέχρι 4 θέσεις πάνω.
        Σας ζητάται η θέση του παίκτη που θέτει την πρόκληση κι έπειτα η θέση του παίκτη που δέχεται 
        την πρόκληση. Σε αυτό το σημείο θα ειδοποιηθείτε με μήνυμα σχετικά με το αν η πρόκληση είναι 
        αποδεκτή η άκυρη.
        Έπειτα, εισάγετε το αποτέλεσμα του παιχνιδιού, απαντώντας στην ερώτηση αν ο παίκτης της 
        χαμηλότερης θέσης νίκησε τον παίκτη της υψηλότερης θέσης.
        Εαν απαντήσετε ναι, ο παίκτης που έκανε την πρόκληση και νίκησε θα πάρει τη θέση του παίκτη που 
        έχασε, μετακινώντας τον ηττημένο κι όλους του παίκτες ανάμεσα στις θέσεις νικητή κι ηττημένου μία 
        θέση κάτω. Για παράδειγμα, αν ο παίκτης #15 νικήσει τον παίκτη #13, 
        ο παίκτης #15 γίνεται #13, ο #13 γίνεται #14 και ο #14 γίνεται #15. Ο παίκτης #16 δε θα υποστεί 
        κάποια αλλαγή.
        Εαν απαντήσετε με όχι δε γίνεται κάποια αλλαγή στην κατάταξη.
        
        Και στις δύο περιπτώσεις, οι νίκες και ήττες προσαυξάνονται φυσιολογικά. 
        Αν προσπαθήσετε να καταγράψετε πρόκληση που περιλαμβάνει παίκτη εκτός ορίων κατάταξης θα 
        ειδοποιηθείτε με σχετικό μήνυμα αφότου υποβάλλετε και τα δύο δεδομένα θέσεων.
        Αν η κατάταξη είναι κενή ή περιέχει μόνο έναν παίκτη θα ειδοποιηθείτε με σχετικό μήνυμα. 

    5. Έλεγχος κατάταξης για αδρανείς παίκτες:

        Το πρόγραμμα διατηρεί δεδομένα σχετικά με την δραστηριότητα των παικτών. Επιλέγοντας αυτή τη 
        λειτουργία το πρόγραμμα θα ελέγξει αν υπάρχει κάποιος παίκτης που δεν είχε δραστηριότητα τον 
        τελευταίο μήνα. Όταν βρεθεί τέτοιος παίκτης μετακινείται κατά μία θέση κάτω στην κατάταξη, με 
        τον κάτω παίκτη να παίρνει τη θέση του. 
        Μόλις επιλεχθεί η λειτουργία αυτή θα ενημερωθείτε με μήνυμα αν υπήρχαν ή όχι παίκτες που ήταν 
        αδρανείς και αλλάξαν θέση και καθώς ποιες θέσεις είχαν.
        Αν η κατάταξη είναι άδεια, θα ειδοποιηθείτε με σχετικό μήνυμα.
        Αν ο τελευταίος παίκτης της κατάταξης είναι αδρανής, δε γίνεται καμία αλλαγή στη θέση του. 
        Ημερομηνίες τελευταίας δραστηριότητας είναι:
            Ημερομηνία ένταξης (επιλογές 1. και 2.)
            Ημερομηνία νίκης ή ήττας (επιλογή 4.)
            Ημερομηνία που ο παίκτης υπέστη πτώση θέσης λόγω αδράνειας (επιλογή 5.) Αυτό σημαίνει πως ο 
            ίδιος παίκτης που πέφτει λόγω αδράνειας δε μπορεί να το ξαναπάθει για 1 ακόμα μήνα.
        ΣΗΜΕΙΩΣΗ: η τελευταία ημερομηνία δραστηριότητας διατηρείται από το πρόγραμμα αλλά δε μπορεί να 
        προβληθεί εντός του προγράμματος

    6. Εμφάνιση κατάταξης:

        Εμφανίζει την κατάταξη. Τα στοιχεία που προβάλλονται είναι η θέση, το όνομα, το επίθετο, οι 
        νίκες και ήττες. 
        Αν η κατάταξη είναι κενή θα ειδοποιηθείτε με σχετικό μήνυμα. 
        Δεν εμφανίζεται η ημερομηνία τελευταίας δραστηριότητας, παρότι διατηρείται ανά παίκτη από 
        το πρόγραμμα.

    7. Έξοδος:

        Τερματίζει το πρόγραμμα και κλείνει το παράθυρο. 
        Όσες αλλαγές έχουν γίνει θα μείνουν αποθηκευμένες και θα είναι προσβάσιμες όταν 
        ξανα-ανοίξετε το πρόγραμμα εφόσον το αρχείο “tennis_club.db” μείνει ανεπηρέαστο.

    Γενικές Υποσημειώσεις

        Μην κλείνετε το παράθυρο του προγράμματος κατά τη λειτουργία του καθώς αυτό μπορεί να 
        οδηγήσει σε απρόσμενα σφάλματα επεξεργασίας των δεδομένων σας, προκαλώντας οριστική 
        αλλοίωσή τους. 
        
## Χρήση
    Παρακάτω φαίνονται παραδείγματα χρήσης με εικόνες.
    Αυτό είναι το κύριο μενού της εφαρμογής.
    ![App Main Menu](https://github.com/BlackBaron94/images/blob/main/Tennis-Main-Menu.jpg)

## Επικοινωνία
    Μπορείτε να επικοινωνήσετε με τον προγραμματιστή στο e-mail black_baron94@hotmail.com