#API Doc

Unified Authorization Method
===

   + Attach token to the  http header `Authorization` 
   + Example: `Authorization`: `token`

1. Account
====
(1)`api/user/account/register`

   + method: POST
   + body: {"mail":" ", "name":" ", "phone:" ", password:" "}

(2)`api/user/account/login` 

   + method: POST
   + body: {"mail/name/phone":" ", password:" "}

2.  Friends
====
(1) `api/user/friend/request`

   + description: send a friend request
   + method: POST
   + body: {"friendId": " "}

(2) `api/user/friend/request`

   + description: agree a friend request
   + method: PUT
   + body: {"friendId": " "}


(3) `api/user/friend/request`

   + description: get the list of the friend request
   + method: GET
 
(4) `api/user/friend/list`

   + description: get the friend list
   + method: GET

(5) `api/user/friend/delete`

   + description: delete a friend
   + method: DELETE
   + body:  {"friendId": " "}

   
3. Sheet
====
 (1) `api/music/sheet/create`
   + description: creare a sheet
   + method: POST
   + body:  {name: " ", privilege: " "}
   + privilege has 3 types: public, private and friend
