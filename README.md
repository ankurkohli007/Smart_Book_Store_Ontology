# Smart Book Store Ontology

This is the assignment proposed during the course [Ambient Intelligence](https://corsi.unige.it/en/off.f/2022/ins/59431?codcla=10635) (AmI) held at [University of Genova (UniGe), Itlay](https://unige.it/en) in [M.Sc Robotics Engineering](https://corsi.unige.it/en/corsi/10635).

## Abstarct ##
This assignment is about the Ontology in Ambient Intelligence to determine about the Ambient Intelligence application, in the Ambient Intelligence (AmI) world. The goal in this case is that to focused on environ- mental intelligence rather than "robots." Also, focused on people and how they can interact with the environment and/or take benefit from it which includes sensors in the AmI. In this ontology, TBox and ABox are defined, Object and Data properties were also included and used in the TBox, individual and property assertions taken in consideration which were added to ABox, and last but not the least SWRL rules also invloved in this ontology preparation.

## Introduction ## 

This report introduces _Protégé 5_ for creating OWL ontology as well as various plugins. Here, _**Ambient Intelligence (AmI)**_ based _**Smart Book Store Ontology**_ is prepared and discussed in this report. The idea is to create a smart AmI environment where readers can buy books in a fast and delight way. The objective behind this Ambient Intelligence application is that buyers encountered with many issues while buying books from the libraries or general book store. This incurs in the waste of time for the readers. the seller in the store or library is not full of knowledge for all the books and buyers deals with them in long queries to get the more information about the books. Also, in these libraries and stores the supervision is irregular and having the chance of stealing the books and vandalized the property. To overcome these problems, Ambient Intelligence (AmI) application is proposed in this _**OWL ontology**_. The problems were solved by this ontology are as follows:

* Due to the lack of knowledge of the seller in the store or libraries, buyer can simply scan the bar-code which is on the book cover, and this bar-code is embedded with the RFID antenna. Also, this RFID antenna easily scan by the buyer’s cellphone.
* In many book stores or libraries there were no connection between the rooms and book shelves. To resolve this problem, a good connection between the rooms is included in this Ontology. Furthermore, buyers can directly search the book of their own choice which they want to buy and directly reach to that particular shelves. This is done by a stereo camera that capture buyer’s image, elaborates data and send them to a computer that through an algorithm displays which room is in line with the buyers. The choice is done by selecting the icon on a screen at the door. Once selected the room, buyers can go directly to the wished one. Lastly, at the door there is a switch which is used for open it.
* Some unwanted activities such as robberies, vandalism, book’s placed on incorrect shelves, and so can be incurred in any store or library. To conquer this issue stereo camera and PIR sensor is installed for the observation which will reacts to humans who are part of such kind of activities. Cases are mounted on shelves that can be opened only by switching an interrupt near them.

## Methodology ##

As aforementioned all rooms in the store or library were interconnected with each other. In the starting at the entrance all the rooms were closed. Here, all the rooms having different colours of book shelves to categorize different books. Also, at the main entrance PIR sensor and Stereo Camera sensor were installed. Therefore, buyer will imitates the purchasing process from the entrance of the store or library. As mentioned above the PIR sensor and Stereo Camera will monitor the entrance of the buyers. The camera will grabs the picture of the person who entered the store or library. This will not only helps in security measures but also helps in guiding the person which room is vacant and which room is containing which type of books and in which shelf is is placed. Once near it, the person selects the place and will open the door by switching the button on the side; in this way also the selected room’s door is opened, drawing a path to the desired chamber. In the room the buyer can browse book and buy them according to its need. This activity will be done by reading the bar-code from their cellphone.

### Installation of _Protégé 5_ ###

To install _Protégé 5_ follow the steps on the given [link](https://protege.stanford.edu/).

_Protégé 5_ software is available for Windows OS X, macOS X, and aslo for Linux. When you will visit the aforementioned link the system will automatically recognize the Operating System you are using and in which you want to install Protégé.

## Requirements of the assignments ##

1. At least 3 top Classes are required in the TBox (i.e., immediately below Thing).
2. At least 4 Object Properties and 4 Data Properties should be created and used in the TBox.
3. At least 6 Individual Assertions and 6 Property Assertions should be added in the ABox.
4. Add at least two SWRL rules to try how rules work.

## Architecture of the proposed ontology ##

Below shows the architecture of the proposed ontology. It comprises of TBox with top classes, classes with their sub-classes, some sub-classes having their sub-classes, and so on.

<p align="center">
  <img width="500" height="800" src="https://github.com/ankurkohli007/Smart_Book_Store_Ontology/blob/7c2795630599a03cf25b4a1904ab8948f999cb7c/image1.png">
</p>

Also, ABox which describes the object and data properties of the proposed ontology. 

<p align="center">
  <img width="900" height="500" src="https://github.com/ankurkohli007/Smart_Book_Store_Ontology/blob/9d19bda5f906c299fd9fb556ad5e4219a8d6f586/image2.png">
</p>

## SWRL Rule ##

For avoiding an huge enhancement of the ontology **SWRL** rule is implemented in this proposed ontology. After considering a real scenario, it is possible to has a discount of 10% on books, if a person can buy more than two. For instance, _**Person(?p)**_ ∧ _**hasBoughtBook(?p, ?nb)**_ ∧ _**swrlb:greaterThan(?nb, 2)**_ -> _**hasDiscount(?p, 0.1)**_.
