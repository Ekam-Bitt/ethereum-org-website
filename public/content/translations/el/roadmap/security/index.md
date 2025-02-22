---
title: Ένα ποιο ασφαλές Ethereum
description: Το Ethereum είναι η πιο ασφαλής και αποκεντρωμένη πλατφόρμα έξυπνων συμβολαίων που υπάρχει. Ωστόσο, υπάρχουν ακόμα βελτιώσεις που μπορούν να γίνουν έτσι ώστε το Ethereum να παραμείνει ανθεκτικό σε οποιοδήποτε επίπεδο επίθεσης για πολύ καιρό στο μέλλον.
lang: el
image: /images/roadmap/roadmap-security.png
alt: "Οδικός χάρτης"
template: roadmap
---

Το **Ethereum είναι ήδη μια πολύ ασφαλής** και αποκεντρωμένη πλατφόρμα [έξυπνων συμβολαίων](/glossary/#smart-contract). Ωστόσο, υπάρχουν ακόμα περιθώρια βελτίωσης ώστε το Ethereum να παραμείνει ανθεκτικό σε κάθε είδους επίθεση και στο μακρινό μέλλον. Αυτές οι βελτιώσεις περιλαμβάνουν μικρές αλλαγές στον τρόπο με τον οποίο οι [εφαρμογές πελάτη Ethereum](/glossary/#consensus-client) διαχειρίζονται την ολοκλήρωση των [μπλοκ](/glossary/#block), καθώς και την αύξηση της ταχύτητας με την οποία το δίκτυο θεωρεί τα μπλοκ ως [οριστικοποιημένα](/developers/docs/consensus-mechanisms/pos/#finality) (δηλαδή δεν μπορούν να αλλάξουν χωρίς εξαιρετικά οικονομικές απώλειες για έναν επιτιθέμενο).

Υπάρχουν επίσης βελτιώσεις που δυσκολεύουν πολύ περισσότερο τη λογοκρισία συναλλαγών, κάνοντας αυτούς που προτείνουν νέο μπλοκ να μην μπορούν να δουν το πραγματικό περιεχόμενο των μπλοκ τους, καθώς και νέους τρόπους για τον εντοπισμό πελατών που λογοκρίνουν. Συνολικά, αυτές οι βελτιώσεις θα αναβαθμίσουν το πρωτόκολλο [Απόδειξης συμμετοχής](/glossary/#pos) έτσι ώστε οι χρήστες, από άτομα έως εταιρείες, να έχουν άμεση εμπιστοσύνη στις εφαρμογές, τα δεδομένα και τα περιουσιακά τους στοιχεία στο Ethereum.

## Αναλήψεις από αποθηκευμένο κεφάλαιο {#staking-withdrawals}

Η μετάβαση από την [απόδειξη εργασίας](/glossary/#pow) σε απόδειξη συμμετοχής ξεκίνησε με τους πρωτοπόρους του Ethereum να «αποθηκεύουν» (staking) τα ETH τους σε ένα ειδικό έξυπνο συμβόλαιο. Αυτά τα ETH χρησιμοποιείται για την προστασία του δικτύου. Στις 12 Απριλίου 2023 υπήρξε μια δεύτερη αναβάθμιση που επιτρέπει την ανάληψη των «αποθηκευμένων» ETH. Από τότε, οι επικυρωτές μπορούν ελεύθερα να «αποθηκεύσουν» ή να αποσύρουν τα ETH τους.

<ButtonLink variant="outline-color" to="/staking/withdrawals/">Δείτε περισσότερα για τις αναλήψεις</ButtonLink>

## Άμυνα κατά των επιθέσεων {#defending-against-attacks}

Μπορούν να γίνουν βελτιώσεις στο πρωτόκολλο απόδειξης συμμετοχής του Ethereum. Μία από αυτές είναι γνωστή ως [view-merge](https://ethresear.ch/t/view-merge-as-a-replacement-for-proposer-boost/13739), ένας πιο ασφαλής αλγόριθμος επιλογής διακλάδωσης [(fork-choice)](/glossary/#fork) που δυσκολεύει ορισμένους πολύπλοκους τύπους επίθεσης.

Η μείωση του χρόνου που απαιτεί το Ethereum για την [οριστικοποίηση](/glossary/#finality) των μπλοκ θα παρέδιδε μια καλύτερη εμπειρία χρήστη και θα απέτρεπε περίπλοκες επιθέσεις «reorg» όπου οι επιτιθέμενοι προσπαθούν να ανακατατάξουν πολύ πρόσφατα μπλοκ για να αποκομίσουν κέρδος ή να λογοκρίνουν ορισμένες συναλλαγές. [**Το Single Slot Finality (SSF)**](/roadmap/single-slot-finality/) είναι ένας **τρόπος ελαχιστοποίησης της καθυστέρησης οριστικοποίησης**. Αυτή τη στιγμή υπάρχουν 15 λεπτά «worth of blocks» που ένας επιτιθέμενος θα μπορούσε θεωρητικά να πείσει άλλους επικυρωτές να αναδιαμορφώσουν. Με το SSF, αυτός ο χρόνος είναι 0. Οι χρήστες, από άτομα έως εφαρμογές και ανταλλακτήρια, ωφελούνται από τη γρήγορη διαβεβαίωση ότι οι συναλλαγές τους δε θα αναστραφούν και το δίκτυο ωφελείται από τον τερματισμό ολόκληρης κατηγορίας επιθέσεων.

<ButtonLink variant="outline-color" to="/roadmap/single-slot-finality/">Διαβάστε περισσότερα για την οριστικοποίηση απλής θέσης</ButtonLink>

## Άμυνα κατά της λογοκρισίας {#defending-against-censorship}

Η αποκέντρωση εμποδίζει άτομα ή μικρές ομάδες [επικυρωτών](/glossary/#validator) να αποκτήσουν υπερβολική επιρροή. Νέες τεχνολογίες αποθήκευσης μπορούν να βοηθήσουν στη διασφάλιση της μέγιστης δυνατής αποκέντρωσης των επικυρωτών του Ethereum, ενώ παράλληλα τους υπερασπίζονται από αποτυχίες υλικού, λογισμικού και δικτύου. Αυτό περιλαμβάνει λογισμικό που μοιράζει τις ευθύνες των επικυρωτών σε πολλούς [κόμβους](/glossary/#node). Αυτό είναι γνωστό ως **τεχνολογία κατανεμημένου επικυρωτή (Distributed Validator Technology - DVT)**. Οι [Δεξαμενές αποθήκευσης](/glossary/#staking-pool) έχουν κίνητρο να χρησιμοποιούν το DVT επειδή επιτρέπει σε πολλούς υπολογιστές να συμμετέχουν συλλογικά στην επικύρωση, προσθέτοντας εφεδρεία και ανθεκτικότητα σε σφάλματα. Επίσης, διαχωρίζει τα κλειδιά επικυρωτή σε διάφορα συστήματα, αντί να έχει μεμονωμένους χειριστές να εκτελούν πολλούς επικυρωτές. Αυτό δυσκολεύει τους ανέντιμους χειριστές να συντονίσουν επιθέσεις στο Ethereum. Συνολικά, η ιδέα είναι να αποκτηθούν οφέλη ασφαλείας με τη λειτουργία των επικυρωτών ως _κοινότητες_ και όχι ως άτομα.

<ButtonLink variant="outline-color" to="/staking/dvt/">Διαβάστε περισσότερα για την τεχνολογία κατανεμημένου επικυρωτή</ButtonLink>

Η εφαρμογή διαχωρισμού **φορέα πρότασης και δημιουργού μπλοκ (proposer-builder separation - PBS)** θα βελτιώσει δραστικά τις ενσωματωμένες άμυνες του Ethereum κατά της λογοκρισίας. Το PBS επιτρέπει σε έναν επικυρωτή να δημιουργεί ένα μπλοκ και σε έναν άλλον να το μεταδώσει σε ολόκληρο το δίκτυο Ethereum. Αυτό εξασφαλίζει ότι τα οφέλη από τους επαγγελματικούς αλγόριθμους δημιουργίας μπλοκ που μεγιστοποιούν τα κέρδη μοιράζονται πιο δίκαια σε όλο το δίκτυο, **αποτρέποντας τη μακροπρόθεσμη συγκέντρωση του αποθηκευμένου κεφαλαίου** στους πιο αποδοτικούς θεσμικούς χρήστες με αποθηκευμένο κεφάλαιο. Ο χρήστης που προτείνει νέο μπλοκ επιλέγει το πιο επικερδές μπλοκ που του προσφέρεται από μια αγορά δημιουργών μπλοκ. Για να λογοκρίνει, ένας χρήστης που προτείνει μπλοκ θα έπρεπε συχνά να επιλέξει ένα λιγότερο επικερδές μπλοκ, κάτι που θα ήταν **οικονομικά παράλογο και επίσης προφανές στους υπόλοιπους επικυρωτές** του δικτύου.

Υπάρχουν πιθανά πρόσθετα στο PBS, όπως κρυπτογραφημένες συναλλαγές και λίστες συμπερίληψης, που θα μπορούσαν να βελτιώσουν περαιτέρω την ανθεκτικότητα του Ethereum στη λογοκρισία. Αυτά καθιστούν τον δημιουργό και τον φορέα πρότασης μπλοκ τυφλούς στις πραγματικές συναλλαγές που περιλαμβάνονται στα μπλοκ τους.

<ButtonLink variant="outline-color" to="/roadmap/pbs/">Διαβάστε περισσότερα για τον διαχωρισμό χρήστη πρότασης και δημιουργού μπλοκ</ButtonLink>

## Προστασία επικυρωτών {#protecting-validators}

Είναι πιθανό ένας προχωρημένος χρήστης που επιτίθεται να μπορέσει να εντοπίσει τους επόμενους επικυρωτές και να τους στείλει ανεπιθύμητα μηνύματα για να τους εμποδίσει να προτείνουν μπλοκ. Αυτό είναι γνωστό ως επίθεση **άρνησης υπηρεσίας (DoS)**. Η εφαρμογή της [**μυστικής εκλογής αρχηγού (secret leader election - SLE)**](/roadmap/secret-leader-election) θα προστατεύσει από αυτόν τον τύπο επίθεσης, αποτρέποντας την εκ των προτέρων γνώση των φορέων πρότασης μπλοκ. Αυτό λειτουργεί με τη συνεχή ανάμειξη ενός συνόλου κρυπτογραφικών δεσμεύσεων που αντιπροσωπεύουν υποψήφιους χρήστες πρότασης μπλοκ και χρησιμοποιώντας τη σειρά τους για να καθοριστεί ποιος επικυρωτής επιλέγεται με τέτοιο τρόπο ώστε μόνο οι ίδιοι οι επικυρωτές να γνωρίζουν εκ των προτέρων τη σειρά τους.

<ButtonLink variant="outline-color" to="/roadmap/secret-leader-election">Διαβάστε περισσότερα για τη μυστική εκλογή αρχηγού</ButtonLink>

## Τρέχουσα πρόοδος {#current-progress}

Οι **αναβαθμίσεις ασφαλείας στο οδικό χάρτη βρίσκονται σε προχωρημένα στάδια έρευνας**, αλλά δεν αναμένεται να εφαρμοστούν για αρκετό καιρό. Τα επόμενα βήματα για το view-merge, PBS, SSF και SLE είναι να οριστικοποιηθεί μια προδιαγραφή και να ξεκινήσει η κατασκευή πρωτοτύπων.
