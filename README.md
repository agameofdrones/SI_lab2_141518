Група 1

https://i.imgur.com/2Vvz6XE.png Слика од CFG

Test Cases 

TC1 User(Username1, Password1, user@mail.com) - Ги исполнува сите услови

TC3 User(Username3, Password3, user.com) - Не содржи @

TC2 User(Username2, Password2, user@mail) - Не содржи .

TC5 null - User = null

TC6 User(null, Password, user@mail) - Username = null

TC7 User(Username, Password2, null) - Email = null


Every Statement Criterium

A if (user!=null)

B if (user.getUsername()!=null ...

C boolean atChar = false, dotChar = false; 

D for (int i=0;i<user.getEmail().length();i++)

E if (user.getEmail().charAt(i)=='@')

F atChar = true;

G if (atChar && user.getEmail().charAt(i)=='.')

H dotChar = true;

I }

J if (atChar && dotChar)

K return true;

L return false;


CFG Complexity

V (G) = P + 1
P - број на јазли во кои има condition = 9
V (G) = 9 + 1 = 10
10 можни патеки кои се покриени со тестови
