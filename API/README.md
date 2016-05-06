#API Doc

1. Account
====
(1)`/api/user/account/register`

   + method: POST
   + body: {"mail":" ", "name":" ", "phone:" ", password:" "}

(2)`/api/user/account/login` 

   + method: POST
   + body: {"mail/name/phone":" ", password:" "}

2.  Friends
====
(1) `/api/user/friend/request`

   + description: send a friend request
   + method: POST
   + body: {"fromId": " ", "toId": " ", "token": " "}

(2) `/api/user/friend/request`

   + description: agree a friend request
   + method: PUT
   + body: {"fromId": " ", "toId": " ", "token": " "}


(3) `/api/user/friend/request`

   + description: get the list of the friend request
   + method: GET
   + query: ?id= & token=
 
(4) `/api/user/friend/list`

   + description: get the friend list
   + method: GET
   + query: ?id= & token=

(5) `/api/user/friend/delete`

   + description: delete a friend
   + method: DELETE
   + body:  {"fromId": " ", "toId": " ", "token": " "}