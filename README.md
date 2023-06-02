***4ο Δημοτικό Σχoλείο Καλαμαριάς***

*Arduino Air Quality Monitoring System*
                                                                       
 Περιεχόμενα:
 
 1)Εισαγωγη

 2)Προτεινόμενη Λύση  
 
 3)Σχεδιασμός
 
 4)Υλικά
 
 5)Σενάριο Χρήσης
 
 6)Στόχος Εφαρμογής
 
 7)Σενάριο Δραστηριότητας
 
 8)Φάση Προετοιμασίας
 
 9)Σχεδιασμός
 
 10)Υλοποίηση
 
 11)Φάση Δοκιμών
 
 12)Πλατφόρμες που χρησιμοποιήθηκαν
 
 13)Κώδικας
 
 14)Δυσκολίες που αντιμετωπίσαμε 
 
 15)Μελλοντικές Εξελίξεις
 
 16)Συμπέρασμα
 
 17)Κύκλωμα
           
           
           
 Εισαγωγή

Ένας πολύ σημαντικός παράγοντας της κλιματικής αλλαγής στον πλανήτης μας, είναι τα αυξημένα επίπεδα ρύπανσης που εμφανίζονται τόσο σε αστικά επιβαρυμένα περιβάλλοντα όσο και σε βιομηχανικές ή περιφερειακές αναπτυσσόμενες ζώνες. Οι περιοχές αυτές πλήττονται από ραγδαία αύξηση την χρήσης των φυσικών πόρων με στόχο την εκβιομηχάνιση και «ανάπτυξη» χωρίς όμως όρους και προϋποθέσεις που θα έκαναν την ανάπτυξη βιώσιμη.

Δυστυχώς μεγάλο μέρος του πληθυσμού που ζει ή εργάζεται σε τέτοιες περιοχές αντιμετωπίζει προβλήματα υγείας λόγω της ρύπανσης. Η κατάσταση αυτή , δημιουργεί την ανάγκη καταγραφής και ανάλυσης της ποιότητας του αέρα σε πραγματικό χρόνο.              


ΠΡΟΤΕΙΝΟΜΕΝΗ ΛΥΣΗ

Η λύση που προτείνεται για την παρακολούθηση της ατμοσφαιρικής ρύπανσης, βασίζεται στο μικροελεγκτή Arduino με το οποίο μετριέται η ποιότητα αέρα, και τα δεδομένα ανεβαίνουν σε έναν διακομιστή web που χρησιμοποιεί το Διαδίκτυο. Με τον τρόπο αυτό κατά περίπτωση και όταν επιδεινώνεται η ρύπανση μιας περιοχής θα προτείνονται ενέργειες βελτίωσης της ποιότητας της ατμόσφαιρας. Για την μέτρηση των ρυπογόνων επιβλαβών σωματιδίων θα χρησιμοποιηθούν αισθητήρες αερίου που μετρούν την περιεκτικότητα του αέρα στα διάφορα επιβλαβή αέρια. Η πληροφορία της ποιότητας του αέρα μπορεί να είναι ανοιχτή και προσβάσιμη σε οποιονδήποτε χρησιμοποιώντας υπολογιστή ή εφαρμογή για κινητές συσκευές.
)ΣΧΕΔΙΑΣΗ

Η συσκευή που θέλουμε να υλοποιήσουμε θα αποτελείται από διάφορους αισθητήρες ποιότητας αέρα οι οποίοι χρησιμοποιούνται για την μέτρηση της συγκέντρωσης διαφόρων ατμοσφαιρικών ρύπων και συγκεκριμένα του CO , LPG και της γενικότερης ποιότητας του αέρα. Ειδικότερα θα γίνει χρήση του μικροελεγκτή Arduino Uno, μιας μονάδας Bluetooth, αισθητήρες αερίου MQ135, MQ5, MQ7 . Όλοι οι αισθητήρες θα είναι διασυνδεδεμένοι με μια πλατφόρμα με την βοήθεια του διαδικτύου ώστε να είναι προσβάσιμη σε όλους. 

ΥΛΙΚΑ

Περιγραφή	Ποσότητα

ESP8266	1                                 
Jumper Wires 40pcs	1
MQ135  1
                                     
                                         
Σενάριο χρήσης.

Το Air Quality monitor παίρνει πληροφορίες από τους αισθητήρες και τις επεξεργαζόμαστε μέσο του προγράμματος ARDUINO IDE. Από εκεί βλέπουμε πόσο καθαρός ή βρόμικος είναι ο αέρας.

 Στόχος Εφαρμογής 

Ο στόχος αυτής της εφαρμογής είναι να μετράμε ποσό καθαρός ή μολυσμένος είναι ο αέρας. 

Δυστυχώς μεγάλο μέρος του πληθυσμού που ζει ή εργάζεται σε τέτοιες περιοχές αντιμετωπίζει προβλήματα υγείας λόγω της ρύπανσης. Η κατάσταση αυτή , δημιουργεί την ανάγκη καταγραφής και ανάλυσης της ποιότητας του αέρα σε πραγματικό χρόνο.

 Σενάριο Δραστηριότητας
Αριθμός μαθητών: 5
Αριθμός  ομάδων:1
Αριθμός ατόμων :5
 Είδος Δραστηριότητας :  Ομαδοσυνεργατική
Ρόλοι : Δεν υπάρχουν διακριτικοί ρόλοι στην ομάδα
Ηλικιακή Ομάδα: 10-12

Φάση Προετοιμασίας:

 ·         Βρήκαμε την ιδέα
·         Ορίσαμε τις προδιαγραφές της εφαρμογής
·         Σκεφτήκαμε τις λειτουργίες της εφαρμογής
·         Καταγράψαμε τις ανάγκες για υλικά
·         Παραγγείλαμε τα υλικά
·         Ορίσαμε τις εργασίες που πρέπει να κάνει κάθε μέλος της ομάδας
·         Προετοιμάσαμε τα κείμενα για την συμμετοχή μας στον διαγωνισμό
·         Αποστείλαμε την περίληψη της συμμετοχής μας στον διαγωνισμό
                             9.Σχεδιασμός

Η συσκευή που θέλουμε να υλοποιήσουμε θα αποτελείται από διάφορους αισθητήρες ποιότητας αέρα οι οποίοι χρησιμοποιούνται για την μέτρηση της συγκέντρωσης διαφόρων ατμοσφαιρικών ρύπων και συγκεκριμένα του CO , LPG και της γενικότερης ποιότητας του αέρα. Ειδικότερα θα γίνει χρήση του μικροελεγκτή Arduino Uno, μιας μονάδας Bluetooth, αισθητήρες αερίου MQ135, MQ5, MQ7 . Όλοι οι αισθητήρες θα είναι διασυνδεδεμένοι με μια πλατφόρμα με την βοήθεια του διαδικτύου ώστε να είναι προσβάσιμη σε όλους.

Δυσκολίες που αντιμετωπίσαμε

Μερικές από τις δυσκολίες που αντιμετωπίσαμε ήταν η εύρεση και εγκατάσταση των βιβλιοθηκών (Libraries) καθώς και η ανατομία του κυκλώματος. Άλλη μία δυσκολία ήταν ο μειωμένος χρόνος εργασίας, καθώς είχαμε πολύ λίγο χρόνο στην διάθεσή μας.  

 Υλοποίηση.

·         Υλοποιήσαμε ξεχωριστά τις λειτουργικότητες
·         Συνδέσαμε όλες τις λειτουργικότητες μαζί σε ένα project
·         Βρήκαμε τον κώδικα
·        Φτιάξαμε το κύκλωμα
·         Φτιάξαμε την παρουσίαση στο Prezi 

  Φάση Δοκιμών 

·         Εγκαταστήσαμε την εφαρμογή Arduino IDE.
·         Δοκιμάσαμε τις λειτουργικότητες του μετρητή
 του αέρα(Gas Sensor).
·         Διορθώσαμε τα προβλήματα των εφαρμογών.
·         Ολοκληρώσαμε την φάση δοκιμών. 

 Πλατφόρμες που χρησιμοποιήθηκαν. 

- Arduino IDE
- Github 

 Κώδικας

#include <ESP8266WiFi.h>
#include <SPI.h>
#include <Wire.h>
#include "MQ135.h"
#include <Adafruit_GFX.h>
#include <Adafruit_SSD1306.h>

#define SCREEN_WIDTH 128    
#define SCREEN_HEIGHT 64    
#define OLED_RESET -1       
Adafruit_SSD1306 display(SCREEN_WIDTH, SCREEN_HEIGHT, &Wire, OLED_RESET);

String apiKey = "3GXEV3B944KWTGQU"; 
const char* ssid = "justDo";  
const char* password = "pratik123";   
const char* server = "api.thingspeak.com";

WiFiClient client;


void setup ()
{
  Serial.begin(115200);
  display.begin(SSD1306_SWITCHCAPVCC, 0x3C); 
  display.clearDisplay();
  delay(10);

  Serial.println("Connecting to ");
  Serial.println(ssid);
  
  display.clearDisplay();
  display.setCursor(0,0);  
  display.setTextSize(1);
  display.setTextColor(WHITE);
  display.println("Connecting to ");
  display.setTextSize(2);
  display.print(ssid);
  display.display();
  
  WiFi.begin(ssid, password);

  while (WiFi.status() != WL_CONNECTED)
  {
    delay(500);
    Serial.print(".");
  }
    Serial.println("");
    Serial.println("WiFi connected");
    
    display.clearDisplay();
    display.setCursor(0,0);  
    display.setTextSize(1);
    display.setTextColor(WHITE);
    display.print("WiFi connected");
    display.display();
    delay (4000);
}


  void loop()
  {
    MQ135 gasSensor = MQ135(A0);
    float air_quality = gasSensor.getPPM();
    Serial.print("Air Quality: ");  
    Serial.print(air_quality);
    Serial.println("  PPM");   
    Serial.println();

    display.clearDisplay();
    display.setCursor(0,0);  
    display.setTextSize(1);
    display.setTextColor(WHITE);
    display. println("Air Quality Index");
    
  
    display.setCursor(0,20);  
    display.setTextSize(2);
    display.setTextColor(WHITE);
    display.print(air_quality);
    display.setTextSize(1);
    display.setTextColor(WHITE);
    display.println(" PPM");
    display.display();


    if (client.connect(server, 80))
  {
    String postStr = apiKey;
    postStr += "&field1=";
    postStr += String(air_quality);
    postStr += "r\n";
    
    client.print("POST /update HTTP/1.1\n");
    client.print("Host: api.thingspeak.com\n");
    client.print("Connection: close\n");
    client.print("X-THINGSPEAKAPIKEY: " + apiKey + "\n");
    client.print("Content-Type: application/x-www-form-urlencoded\n");
    client.print("Content-Length: ");
    client.print(postStr.length());
    client.print("\n\n");
    client.print(postStr);
    
    Serial.println("Data Send to Thingspeak");
  }
    client.stop();
    Serial.println("Waiting...");

    delay(2000);      
    
    Δυσκολίες που αντιμετωπίσαμε.
Οι θήρες του υπολογιστή δεν συνδέονταν με το καλώδιο.


  Μελλοντικές Εξελίξεις

Το  συγκεκριμένο μηχάνημα θα χρησιμοποιηθεί από πολλούς ανθρώπους στο μέλλον για την πρόγνωση της καθαριότητας του αέρα .


16)Συμπέρασμα

Όλον  αυτόν το καιρό που δουλεύουμε το συγκεκριμένο project έχουμε αναπτύξει την συνεργατικότητα και την ομαδικότητα καθώς έχουμε μάθει πως να φτιάχνουμε ένα κύκλωμα , τον κώδικα και να κατεβάζουμε libraries. 

17)Κύκλωμα
 
![image](https://github.com/gzaxar/Arduino_Air_Quality_Monitoring_System/assets/78252867/4af989fa-f747-4974-97eb-70d4c8a8133f)

