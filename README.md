![wizard](https://github.com/iee-ihu-gr-course1941/ADISE23_WizardCardGame/assets/57770693/e847f688-f9e9-451e-b795-39560aca1d4b)


## Table of Contents
- [Περιγραφή](#Περιγραφή)
- [Κανόνες](#Κανόνες)
- [Υλοποίηση](#Υλοποίηση)
- [Αποτίμηση](#Αποτίμηση)

## Περιγραφή

Πρόκειται για ένα επιτραπέζιο παιχνίδι καρτών από τον Ken Fisher, 1984 Καναδάς. Υπάρχουν 4 φυλές (13 ${\color{blue}Άνθρωποι}$, 13 ${\color{red}Νάνοι}$, 13 ${\color{yellow}Γίγαντες}$, 13 ${\color{green}Ξωτικά}$), 4 Μάγοι (Υψηλότερο χαρτί) και 4 Γελωτοποίοι (Μπαλαντέρ), συνολικά 60 κάρτες. Οι μάγοι και οι γελωτοποίοι δεν έχουν χρώμα.

## Κανόνες

Ο κάθε παίκτης ανταγωνίζεται τους υπόλοιπους, με σκοπό να κερδίσει τις περισσότερες παρτίδες σε κάθε γύρα (ο αριθμός των γυρών καθορίζεται από το πλήθος των παικτών). <br>
Για τη **ν-οστή** γύρα παίζονται **ν παρτίδες**, ο κάθε παίκτης παίρνει **ν κάρτες** και ορίζεται από μια άλλη κάρτα το ατού (πιο δυνατό χρώμα) της γύρας<sup>1</sup>. Στην τελευταία γύρα δεν υπάρχει ατού. <br>
Πριν ξεκινήσει η γύρα και αφού έχουν δει όλοι οι παίκτες τα φύλλα τους και το ατού, στοιχηματίζουν πόσες παρτίδες **k** θα πάρουν. <br>
Εάν πέσουν μέσα στο i=**k**, πέρνουν +10 για όσες είπαν και +20. Εάν δηλώσαν **k** = 0, παίρνουν +20. Τέλος, αν κέρδισαν περισσότερες ή λιγότερες από **k**, -10 για κάθε παιχνίδι. <br>
Συνοπτικά ο τύπος είναι ο εξής: <br>
$` y_{n} = y_{n-1} + 10k + 20 `$ , για i=**k**. , <br>
$` y_{n} = y_{n-1} - 10|i-k| `$ , για i≠**k**. <br>
Κατά τη διάρκεια μιας παρτίδας, ο πρώτος παίκτης θα πετάξει ένα φύλλο, οι υπόλοιποι **αναγκστικά** ακολουθούν το χρώμα (φυλή)<sup>2</sup>, το μεγαλύτερο φύλλο κερδίζει<sup>3</sup>. <br>
Ο νικητής της παρτίδας, ξεκινά πρώτος στην επόμενη. <br>
Στο τέλος της γύρας βγαίνουν οι κερδισμένοι και (αν υπάρχουν) χαμένοι. <br>
<sup>1</sup> Εάν βγει μάγος το ατού, το ατού επιλέγεται ξανά στην τύχη. Αν βγει γελωτοποιός, δεν υπάρχει ατού για αυτή τη γύρα. <br>
<sup>2</sup> Εάν κάποιος παίκτης δεν έχει το χρώμα που έπαιξε ο πρώτος, απλώς παίζει κάποιο άλλο. Εάν κάποιος παίκτης έχει μάγο ή γελωτοποιό, μπορεί άμα θέλει να μη πετάξει το χρώμα του 1ου και να πετάξει μάγο/γελωτοποιό. Σε περίπτωση που ο πρώτος έχει πετάξει μάγο ή γελωτοποιό, οι υπόλοιποι παίκτες πετάνε ό,τι θέλουν ή ο αμέσως επόμενος επιβάλλει το χρώμα στους άλλους αντίστοιχα. <br>
<sup>3</sup> Η ιεραρχία είναι 1ος μάγος που θα παιχτεί -> Μεγαλύτερο ατού φύλλο -> Μεγαλύτερο χρώμα παρτίδας φύλλο.<br>
[Περιγραφή παιχνιδιού από την Κάισσα](https://youtu.be/gYILYQgS5_o?si=mdzMl9aZ71mZYcaT&t=59)
## Υλοποίηση

## Αποτίμηση
