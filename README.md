# Zealand

School project for Zealand Køge




<img width="782" height="252" alt="image" src="https://github.com/user-attachments/assets/a62f5a3f-1055-49b7-9803-4214da171f80" />
<img width="640" height="1098" alt="image" src="https://github.com/user-attachments/assets/13d380a6-3a40-4cb1-845b-f40211d94e5d" />
<img width="661" height="551" alt="image" src="https://github.com/user-attachments/assets/581fcb98-0c59-4461-853a-711bbee6987b" />
**Decicion test table**

| Rolle     | Object         | Create | Read | Update | Delete | LIST | Handling                                                         |
|-----------|----------------|--------|------|--------|--------|------|------------------------------------------------------------------|
| Manager   | Project        | Yes    | Yes  | Yes    | Yes    | Yes  | Kontrol over selveste projectet                                  |
| Developer | Project        |        | Yes  | Yes    |        | Yes  | Kan kun arbejde med projectet de er blevet tildelt               |
| Admin     | Access control | Yes    | Yes  | Yes    | Yes    | Yes  | StÃ¥r for fordeling af access rettigheder til forskellige objects |
| Guest     | Projectet      |        | Yes  |        |        |      | Read only                                                        |
| HR-leder  | Ansatte        | Yes    | Yes  | Yes    | Yes    | Yes  | Kan kun arbejde med ansatte og deres information, ikke projectet |


Eksemplet hører unde rbåde Role and permission test: da rollerne kun kan de du skulle kunne. og autorisasition mellem systmer testet, da der ikke er en super user for alle objekterne.



Test pyramide

Bottom to top

Unit test
Tester om rolle baserert access control virker
Tester om CRUD virker
tester om conditions såsom Ansatte only virker
tester om edge cases såsom udifineret roller ikke har fri adgang.


Integration

Tæster permission med data modeller og database

Ansat prøver at opdatere en anden ansats timetabel -> nægtet
HR prover at tilgå projekt -> nægtet

End-to end

Aktuel CRUD testing gennem API
Manager kreere projet gennem API -> success og log i Databasen.







Data driven
<img width="669" height="526" alt="image" src="https://github.com/user-attachments/assets/e95a179d-70a6-4aec-9e09-1d21b61f6164" />




