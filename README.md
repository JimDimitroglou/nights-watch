# night shift
Αποθετήριο της ομάδας Δημήτρη-Ειρήνης "Mad Scientists" για στην συμμετοχή στον Διαγωνισμό Ρομποτικής Ανοιχτών Τεχνολογιών

   To project το οποίο σκοπεύουμε να σας παρουσιάσουμε αφορά μία συσκευή η οποία είναι σχεδιασμένη για να χρησιμοποιηθεί  σε νοσοκομειακές μονάδες. Πρόκειται για ένα project με arduino το οποίο χρησιμοποιεί αισθητήρες:
   
   -μέτρησης καρδιακών παλμών,
   
   -οξύμετρο 
   
   -θερμοκρασίας σώματος
   
   Οι προαναφερθέντες αισθητήρες θα τοποθετούνται με την βοήθεια μερικών επιπλέον εξαρτημάτων(κυρίως υφάσματος) πάνω στους ασθενείς και θα λαμβάνουν διαρκώς τις αντίστοιχες τιμές. Παράλληλα όταν οι τιμές που λαμβάνουν οι αισθητήρες είναι εντός των φυσιολογικών ορίων θα παραμένει αναμμένο ένα πράσινο led ενώ όταν θα είναι εκτός των φυσιολογικών ορίων θα ενεργοποιείται ένας ηχητικός συναγερμός και θα αναβοσβήνει ένα κόκκινο led.
  Χάρη στο διαδίκτυο των πραγμάτων τα δεδομένα θα στέλνονται σε έναν (ή περισσότερους) υπολογιστές- φορητές συσκευές από τους οποίους οι επιβλέποντες θα μπορούν να ελέγχουν τους καρδιακούς παλμούς, την πίεση του αίματος, το ποσοστό οξυγόνου που κυκλοφορεί στο αίμα και την θερμοκρασία του σώματος του κάθε ασθενή με πολύ λιγότερο κόπο τη στιγμή που το προσωπικό στο νοσοκομείο θα είναι περιορισμένο, όπως συμβαίνει συνήθως στη νυχτερινή βάρδια. 
  Θα θέλαμε να επιμείνουμε στο γεγονός ότι τα δεδομένα θα μπορούν να μεταφερθούν σε άλλο υπολογιστή αλλά και το ότι οι ασθενείς θα μπορούν να ελέγχονται εξ’ αποστάσεως και διαρκώς ώστε να γίνει ασφαλέστερη η παραμονή τούς στο νοσοκομείο.    
 
Για την υλοποίηση του project θα χρησιμοποιηθεί Arduino (Arduino Uno/Nano ή Lilypad) και οι αισθητήρες:

-MAX30100, για μέτρηση καρδιακών παλμών και οξύγόνωσης αίματος

-DHT11: για τη θερμοκρασία του σώματος 

-IOT module: esp8266 

Ακόμη θα χρησιμοποιηθεί και ένα piezo buzzer για να παράγει ηχητικό σήμα και led για να δίνει οπτικό σήμα (allert) στο προσωπικό που ενδεχομένως βρίσκεται κοντά στον ασθενή σε περίπτωση μη φυσιολογικών τιμών στις μετρήσεις

Από τον αισθητήρα ΜΑΧ30100 θα αφαιρεθούν με κοπίδι οι αντιστάσεις των 4.7kOhm και θα αντικατασταθούν με εξωτερικές, γιατί το Arduino δουλεύει με ρεύμα τάσης 5V ή 3.3V ενώ οι αντιστάσεις αυτές ρίχνουν την τάση στο 1.8V.
Επομένως η τάση δεν είναι αρκετή για να τη "διαβάσει" το arduino. 
