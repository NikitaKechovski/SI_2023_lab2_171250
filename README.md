# SI_2023_lab2_171250
2. Control flow diagram 
  ![image](https://github.com/NikitaKechovski/SI_2023_lab2_171250/assets/81694941/5d5a2bc9-8f87-4a9e-b7e1-cfc1af47b127)
3. Цикломатската комплексност на овој граф изнесува 11. Овој резултат е добиен според формулата v = P + 1, каде P се бројот предиканти јазли, односно 10. Истото може да се потврди со формулата V = e - n + 2, каде е претставуваат рабови во овој случај 33, а n претставуваат јазли односно 24.
4. Тест случаеви според критериум Every Branch
    1. Nodes 1,2,3,25
      user : null
    allUsers = anything
    2. Nodes 1,2,4,5,6,7,8,9,10,11,13,16,9,10,11,12,13,14,16,9,15,17,18,25
      user{
    username : null
    password: 123
    email: test@finki.com
    }
    allUsers = [ {username : Test
    password: anything
    email: test1@finki.com } , {username : test@finki.com
    password: anything
    email: test@finki.com } ]
    3. Nodes 1,2,4,6,7,15,17,19,20,21,23,20,21,22,25
      user{
    username : "name "
    password: "123456789#"
    email: " testmail"
    }
    allUsers = anything
    4. Nodes 1,2,4,6,7,15,17,19,24,25
      user{
    username : "name "
    password: "1234   56789#"
    email: " testmail"
    }
    allUsers = anything

    5. Nodes 1,2,4,6,7,15,17,19,{20,21,23}20,24,25
      user{
    username : "name "
    password: "123456789"
    email: " testmail"
    }
    allUsers = anything

5. Тест случаеви според Multiple Condition критериум
       if (user==null || user.getPassword()==null || user.getEmail()==null)
       
       T || X || X  - user=null, ( password=anything, email=anything)
       
       F || T || X     user{
        username : "name "
        password: null
        email: anything
        }
        
        F || F || T  	user{
          username : "name "
          password: "123456789"
        email: null
        }

        F || F || F 	user{
        username : "name "
          password: "123456789"
        email: " testmail"
        }
       
